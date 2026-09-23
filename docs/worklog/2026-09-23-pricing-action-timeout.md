# 2026-09-23: weekly pricing action kept timing out

Issue #4, PR #5.

## Symptom

The scheduled `LLM Pricing Update` runs on 2026-09-14 and 2026-09-21 ended **cancelled** after 20m18s. The verify step printed "rotate the GitHub PAT". The initial suspicion was that the managed agent itself was not capable enough.

## What the logs actually showed

- The agent was doing the job. On 2026-09-21 all four files landed on `main` (Mistral 17:30, Anthropic 17:37, OpenAI 17:45, README 17:50 CEST). The runner was cancelled at 17:43. The session kept running after the runner died and finished on its own.
- The only prior green run (2026-09-07, manual dispatch) took 17m13s, so the 20-minute cap was always marginal.
- Most wall time was spent pushing through the GitHub MCP tool, which takes whole file contents as an argument. Roughly 3 minutes per file to re-emit 20–30 KB of markdown.
- The verify step runs `if: always()`, so on cancellation it compared remote `main` before the late commits arrived and blamed the PAT.
- The Aug 17 to Sep 7 failures were a different, already-fixed problem: no push credential in the sandbox, agent left a bundle in `/mnt/session/outputs`.

## Changes (PR #5, squash-merged as 49b2e16)

1. `timeout-minutes` 20 to 45.
2. Session now mounts the repo as a `github_repository` resource when `AGENT_GITHUB_TOKEN` is set, and the task message tells the agent to `git push` from the sandbox. Falls back to the MCP path when the secret is absent.
3. Verify step distinguishes a cancelled job from a genuine push failure.

## Setup done

- Created a fine-grained PAT (Contents: Read and write, repo-scoped) and stored it as repo secret `AGENT_GITHUB_TOKEN`. First attempt via `gh secret set` inside Claude Code stored an empty value because there is no TTY for the paste prompt; fixed with `--body "$(pbpaste)"`.

## Verification

- Test run 35830906686 on the feature branch: success in 11m28s. Log shows `Mounting https://github.com/Chili36/effective-invention ... (git push via proxy)`, four commits landed via git, verify step reported `OK: the agent pushed a new commit to main`.
- The first, cancelled test run (35830670887) confirmed the fallback path and the new cancellation warning. Its orphaned session later pushed a duplicate re-verification to `main` via MCP. Harmless.

## Open items

- PAT expiry. When it lapses, runs go back to the slow path with `AGENT_GITHUB_TOKEN not set` in the log.
- `anthropic` SDK is installed unpinned in the workflow. Verified working on 1.8.0.
