# Weekly pricing update: how the GitHub Action and the managed agent fit together

Last updated: 2026-09-23

## Moving parts

| Piece | Where it lives | What it does |
|---|---|---|
| `.github/workflows/main.yml` | this repo | Runs every Monday 09:00 UTC (and on manual dispatch). Installs the `anthropic` SDK and runs the embedded `run_agent.py`. |
| `run_agent.py` (embedded in the workflow) | this repo | Thin client. Creates a session on the managed agent, sends the task message, streams events to the job log, exits when the session goes idle. |
| Managed agent `agent_011CZwijZihnPvZcL6HjQo9F` | Anthropic Console | The actual worker. Runs in a sandbox on Anthropic's side, does the web research, edits the markdown files, commits to `main`. |
| Environment `env_01B6Hn4X4d7soRPUNnjmoT4A` | Anthropic Console | Sandbox config. Limited networking, no direct github.com egress. |
| Vault `vlt_011CZwiqKEjCEEq7PfdLYt3Y` | Anthropic Console | Holds the OAuth credential for the GitHub MCP server (`api.githubcopilot.com/mcp/`). |
| Secret `ANTHROPIC_API_KEY` | GitHub repo secrets | Lets the runner call the Anthropic API. |
| Secret `AGENT_GITHUB_TOKEN` | GitHub repo secrets | Fine-grained PAT, Contents: Read and write, scoped to this repo. Used to mount the repo into the session. |

The GitHub runner never has the model card files. The agent commits straight to remote `main` from its sandbox. The runner only checks afterwards whether `main` moved.

## Two ways the agent can push

1. **Repo mount (current, fast).** When `AGENT_GITHUB_TOKEN` is set, the session is created with a `github_repository` resource. The repo is cloned at `/workspace/effective-invention` and the agent runs plain `git commit` / `git push`. Auth is injected by Anthropic's git proxy after the request leaves the sandbox; the token never enters the container. A full run takes about 11 minutes.
2. **GitHub MCP push-by-content (fallback, slow).** When the secret is missing or empty, the script logs `AGENT_GITHUB_TOKEN not set` and the agent falls back to the MCP `create_or_update_file` tool. The model has to re-emit each 20–30 KB file as tool arguments, roughly 3 minutes per file. A full run takes 25–30 minutes.

Commits pushed through the git proxy are authored as "Claude". That is intentional.

## Reading a failed run

- **Cancelled after N minutes** means the runner hit `timeout-minutes`. The session is durable and keeps working after the runner dies, so commits usually land a few minutes later. Check `git log origin/main` before assuming the update failed. The verify step prints a warning for this case.
- **`AGENT_GITHUB_TOKEN not set` in the log** means the secret is empty or expired. The run still works on the fallback path, just slowly. Regenerate the PAT and re-set the secret.
- **Verify step red with "could NOT push"** means the agent finished with `end_turn` but `main` did not move and the log has push-failure markers. Usually the MCP credential in the vault has expired.
- **`FATAL:` line** is a client-side exception in `run_agent.py`, typically an API or auth error before the agent started.

## Maintenance

- The PAT behind `AGENT_GITHUB_TOKEN` has an expiry date set when it was created. When it lapses, runs silently go back to the slow path. Rotate it at `https://github.com/settings/personal-access-tokens` and re-set the secret.
- To set a secret from inside Claude Code, use `gh secret set AGENT_GITHUB_TOKEN --repo Chili36/effective-invention --body "$(pbpaste)"`. The interactive paste prompt does not work there because there is no TTY.
- `pip install anthropic` in the workflow is unpinned. The script was verified against SDK 1.8.0 on 2026-09-23. If a run starts failing with `AttributeError` or unexpected event types, pin the version.
- Manual test: `gh workflow run main.yml --ref <branch>`.

## History

See `docs/worklog/` for dated entries.
