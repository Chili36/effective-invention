# 🟢 OpenAI — Model Cards

> **Last updated:** 2026-10-07
> **Source:** https://developers.openai.com/api/docs/pricing · https://developers.openai.com/api/docs/models · https://developers.openai.com/api/docs/deprecations · https://openai.com/index/devday-2026-recap/ · https://openai.com/index/introducing-gpt-6-1-sol/ · https://openai.com/index/gpt-6-astra/ · https://openai.com/news
> **Scraped / verified:** 2026-10-07 — ✅ Re-fetched the live `developers.openai.com/api/docs/pricing` and `/api/docs/models` pages directly. **No pricing changes found since the October 5 refresh** — GPT-6 Astra ($10/$50), GPT-6.1 Sol ($2/$10), GPT-6 Luna ($0.10/$0.50), GPT-5.6 Terra/Sol/Luna, GPT-5.6 Cyber, and GPT-Rosalind Research all confirmed unchanged. 🆕 **October 5, 2026 — Decisions API launched in public beta**, powered by `gpt-6-luna`: a fast model/tool/action-selection endpoint (predicates, choices, scores) billed **input-tokens only** at $0.10/MTok — no cache-write, cache-read, or output-token charges. ℹ️ **October 5–7, 2026 — "Codex speed" infrastructure rollout:** OpenAI shipped a default ~50% output-speed increase for GPT-6 Astra and GPT-6.1 Sol across ChatGPT/Codex/Sign-in-with-ChatGPT partners (OpenCode, Pi, Amp, Devin) — an infrastructure optimization with **no price or model change**. ✅ **Re-confirmed: `GPT-6 Cyber` still has not been officially announced, priced, or dated by OpenAI** — remains discovery-only per this tracker's policy; `gpt-5.6-cyber` is still OpenAI's most advanced priced cyber model.

All prices are **USD per million tokens (MTok)** unless noted. Batch/Flex API gives a flat **50% discount** on all models. Cached input tokens get **50–95% off** depending on model.

> **Context tiers for GPT-6, GPT-5.6, GPT-5.5, and GPT-5.4:** Standard ("short context") pricing applies for prompts **under ~272K tokens**. The long-context tier applies **2× input / 1.5× output** vs. short-context rates.
>
> **Service tiers:** Ultrafast (6× standard, GPT-6 Astra only so far), Fast mode (2× standard; renamed from "Priority processing" on July 30, 2026), Standard (default), Batch, and Flex (50% off standard).

> 🆕 **September 29, 2026 — GPT-6.1 Sol launched at OpenAI DevDay 2026, replacing GPT-6 Sol after just 7 days.** OpenAI describes it as delivering "near-Astra intelligence... at one-fifth of Astra's standard input and output token prices." Standard API pricing is **unchanged from GPT-6 Sol** at $2.00 input / $10.00 output per MTok, but **cached input drops 50% to $0.10/MTok** (a 95% discount vs. standard input, up from GPT-6 Sol's 90%). Available immediately to all Plus, Pro, Business, Enterprise, and Edu users in ChatGPT Work and Codex (not yet in plain ChatGPT Chat), and via the API as `gpt-6.1-sol`. On DeepSWE v1.1, it matches GPT-6 Astra at roughly one-fifth of the cost while beating GPT-6 Sol's best score by 6.4 points. Third-party benchmarking (Artificial Analysis) puts it 31% cheaper per task than GPT-6 Sol and 64% cheaper than GPT-5.6 Sol. A **GPT-6.1 Sol · Ultrafast** variant (up to 8× faster token generation in Codex) is "coming soon," unpriced as of this refresh. GPT-6 Sol itself has been fully removed from OpenAI's live pricing and model catalog pages — see Legacy section.
>
> 🆕 **September 29, 2026 — Ultrafast tier priced for GPT-6 Astra.** A new premium speed tier above Fast mode, offering up to 8× faster token generation in Codex and up to 6× in the API. GPT-6 Astra Ultrafast pricing: $60.00 input / $6.00 cached / $75.00 cache write / $300.00 output per MTok (short context), doubling for long context. Available now in the API and in ChatGPT Work/Codex on Pro 500 and Enterprise plans.
>
> 🆕 **September 29, 2026 — Dots launched**, OpenAI's new "always-on" agent product — "remarkably capable, always-on agents built to handle everything," persisting work and context beyond a single chat session. Available on ChatGPT Pro and Business Premium in eligible markets (Enterprise/Edu/Healthcare in opt-in beta). Billed through the ChatGPT subscription, not separately metered per token at this time.
>
> 🆕 **September 29, 2026 — New Pro 500 ChatGPT plan** launched, offering 25× the ChatGPT Plus usage allowance and bundled access to Ultrafast.
>
> 🆕 **September 29, 2026 — OpenAI Private Intelligence announced.** Zero Data Retention with Private Safety Processing is now live, enabling automated safety reviews without giving OpenAI personnel access to underlying content; a Private Inference preview (confidential computing with verifiable controls) is "coming this fall."
>
> ⚠️ **`GPT-6 Cyber` did NOT materialize at DevDay.** Despite Fortune's September 24 report that OpenAI was preparing to preview a fourth cybersecurity model at DevDay, the official `openai.com/index/devday-2026-recap/` announcement list contains no mention of it. **GPT-6 Cyber remains unconfirmed and unpriced** — still discovery-only per this tracker's policy; `gpt-5.6-cyber` (Aug 2026) remains OpenAI's most advanced priced cyber model.
>
> 🆕 **September 22, 2026 — GPT-6 Sol and GPT-6 Luna launched**, expanding the GPT-6 family alongside GPT-6 Astra (launched Sept 3) — both **50% cheaper** than their GPT-5.6 promotional-era predecessors. GPT-6 Sol was itself replaced by GPT-6.1 Sol just 7 days later (see above). **GPT-6 Astra remains OpenAI's best model overall**, unchanged at $10/$50. **There is no GPT-6 Terra** — GPT-5.6 Terra ($2.00/$12.00 per MTok) is confirmed unchanged and remains the live, un-replaced mid-tier "Default" model, directly re-verified via its own model page this refresh. GPT-5.6 Sol's promotional pricing is now confirmed by OpenAI's pricing page to run **"at least through November 21, 2026."**
>
> ⚠️ **Videos API, Sora-2, and Sora-2-Pro have SHUT DOWN (September 24, 2026).** Confirmed via the official Deprecations page: the Videos API, `sora-2`, `sora-2-pro`, and their dated snapshots were all removed from the API on **September 24, 2026**, with **no replacement model listed**.
>
> ⚠️ **`o3`, `o3-pro`, and the original GPT-5 launch snapshot family shut down December 11, 2026.** All map to `gpt-5.6-sol`/`terra`/`luna` per OpenAI's official mapping.
>
> 🆕 **October 1, 2026 — new deprecation wave.** `gpt-5.3-codex`, `gpt-5.1`, and `gpt-5.4-nano` are now deprecated, shutting down **April 1, 2027** (6 months' notice) — migrate to `gpt-6-sol` (codex, 5.1) or `gpt-6-luna` (nano). Legacy text-to-speech models `tts-1`, `tts-1-hd`, and two older `gpt-4o-mini-tts` snapshots are deprecated, shutting down **January 6, 2027** — migrate to `gpt-realtime-2.1-mini`.
>
> 🆕 **September 15, 2026 — GPT-5.5 retires from ChatGPT, ChatGPT Work, and Codex on October 14, 2026 (API unaffected).**

---

## ✅ Active / Recommended Models

### GPT-6 Astra *(Flagship — unchanged)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-6-astra` |
| **Status** | ✅ Active — **Flagship / best model across the board** |
| **Input price (short ctx <272K)** | $10.00 / MTok |
| **Cached input (short)** | $1.00 / MTok |
| **Cache write (short, 1.25×)** | $12.50 / MTok |
| **Output (short ctx)** | $50.00 / MTok |
| **Input price (long ctx >272K)** | $20.00 / MTok |
| **Cached input (long)** | $2.00 / MTok |
| **Output (long ctx)** | $75.00 / MTok |
| **Fast mode (short: input/cached/write/output)** | $20.00 / $2.00 / $25.00 / $100.00 |
| **🆕 Ultrafast (short: input/cached/write/output)** | $60.00 / $6.00 / $75.00 / $300.00 — up to 6× API speed / 8× in Codex |
| **Batch/Flex (short: input/cached/write/output)** | $5.00 / $0.50 / $6.25 / $25.00 |
| **Context window** | 1,050,000 tokens |
| **Max output** | 128,000 tokens |
| **Knowledge cutoff** | April 30, 2026 |
| **Reasoning effort** | `low`, `medium`, `high`, `xhigh`, `max` — **`none` not supported** |
| **Availability** | ChatGPT Plus/Pro/Business/Enterprise · GPT-6 Astra Pro · OpenAI API · Microsoft Azure/Foundry · AWS Bedrock |

---

### 🆕 GPT-6.1 Sol *(Released September 29, 2026 at DevDay — Replaces GPT-6 Sol after just 7 days)*

> Near-Astra intelligence for agentic coding, computer use, and professional work at one-fifth of Astra's standard token prices. Headline per-token price is unchanged from GPT-6 Sol, but cached input is 50% cheaper and the model substantially closes the gap to GPT-6 Astra on coding and document-understanding benchmarks.

| Field | Value |
|---|---|
| **Model ID** | `gpt-6.1-sol` |
| **Status** | ✅ Active — replaces GPT-6 Sol as the "balance intelligence and cost" tier (GPT-6 Sol removed from pricing/model catalog) |
| **Input (short ctx)** | $2.00 / MTok *(unchanged from GPT-6 Sol)* |
| **Cached input (short)** | 📉 **$0.10** / MTok *(was GPT-6 Sol's $0.20 — 95% off standard input, up from 90%)* |
| **Cache write (short, 1.25×)** | $2.50 / MTok |
| **Output (short ctx)** | $10.00 / MTok *(unchanged from GPT-6 Sol)* |
| **Input (long ctx)** | $4.00 / MTok |
| **Cached input (long)** | $0.20 / MTok |
| **Output (long ctx)** | $15.00 / MTok |
| **Batch/Flex (short: input/cached/write/output)** | $1.00 / $0.05 / $1.25 / $5.00 |
| **Fast mode (short: input/cached/write/output)** | $4.00 / $0.20 / $5.00 / $20.00 |
| **Ultrafast** | "Coming soon" — unpriced as of this refresh |
| **Context window** | 1,050,000 tokens |
| **Max output** | 128,000 tokens |
| **Knowledge cutoff** | April 30, 2026 |
| **Reasoning effort** | `low`, `medium`, `high`, `xhigh`, `max` |
| **Availability** | ChatGPT Work, Codex (Plus/Pro/Business/Enterprise/Edu) · OpenAI API (`gpt-6.1-sol`) — **not yet in plain ChatGPT Chat**; also GA in GitHub Copilot (Pro+/Max/Business/Enterprise) |
| **Rate limits** | Tier 1: 500 req/min, 500K TPM · Tier 5: 15,000 req/min, 40M TPM |
| **Notable** | Matches GPT-6 Astra on DeepSWE v1.1 at ~⅕ the cost, beating GPT-6 Sol's best score by 6.4 points; scores higher than Opus 5.5-with-fallbacks on GDP.pdf at under half the cost; Artificial Analysis measures it 31% cheaper per task than GPT-6 Sol and 64% cheaper than GPT-5.6 Sol at max effort; supports Multi-agent subagent spawning with no documented limit |

---

### 🆕 GPT-6 Luna *(Released September 22, 2026 — Cost-Sensitive, High-Volume)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-6-luna` |
| **Status** | ✅ Active — cost-sensitive, high-volume workloads; default for ChatGPT Free/Go desktop app |
| **Input (short ctx)** | 📉 **$0.10** / MTok *(was GPT-5.6 Luna's $0.20 — 50% cheaper)* |
| **Cached input (short)** | $0.01 / MTok |
| **Output (short ctx)** | 📉 **$0.50** / MTok *(was $1.20 — 58% cheaper)* |
| **Input (long ctx)** | $0.20 / MTok |
| **Output (long ctx)** | $0.75 / MTok |
| **Batch/Flex (short input/output)** | $0.05 / $0.25 |
| **Context window** | 1,050,000 tokens |
| **Max output** | 128,000 tokens |
| **Knowledge cutoff** | May 18, 2026 |
| **Reasoning effort** | `none`, `low`, `medium`, `high`, `xhigh`, `max` |
| **Availability** | ChatGPT Free/Go (desktop app) · ChatGPT Work · Codex · OpenAI API |
| **Notable** | At max effort, DeepSWE v1.1 score of 66.6% — comparable to Claude Opus 5/Fable 5 at medium effort, at 93%/96% lower cost respectively |

---

### GPT-5.6 Terra *(✅ Confirmed unchanged — mid-tier "Default" model, no GPT-6 equivalent yet)*

> **Directly verified via its dedicated model page (`developers.openai.com/api/docs/models/gpt-5.6-terra`) as of this refresh:** Terra remains fully active and unchanged, still labeled **"Default"** on OpenAI's model catalog. There is no GPT-6 Terra — this model has no successor yet.

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.6-terra` |
| **Status** | ✅ Active — **Default; balances intelligence and cost; no GPT-6 equivalent** |
| **Input price** | $2.00 / MTok |
| **Cached input** | $0.20 / MTok |
| **Output price** | $12.00 / MTok |
| **Context window** | 1,050,000 tokens |
| **Max output** | 128,000 tokens |
| **Knowledge cutoff** | February 16, 2026 |
| **Reasoning effort** | `none`, `low`, `medium` (default), `high`, `xhigh`, `max` |
| **Notable** | "Roughly corresponds to the mini model tier used in earlier GPT-5 families." Still the official migration target for the deprecated `o4-mini` |

---

### GPT-5.6 Sol *(⚠️ Superseded for general use by GPT-6.1 Sol — still active, backs Daybreak Blue alias)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.6-sol` |
| **Status** | ⚠️ 🔄 Replaced by GPT-6.1 Sol for general use — still active; also backs `gpt-daybreak-blue-latest` and the `gpt-5.6-cyber` pricing baseline |
| **Input (short ctx)** | $4.00 / MTok |
| **Output (short ctx)** | $20.00 / MTok |
| **Promotional pricing window** | 🆕 Confirmed by OpenAI's pricing page to run **"at least through November 21, 2026"** |
| **Migration (general use)** | → **`gpt-6.1-sol`** ($2/$10 — 50% cheaper, plus 95%-off cached input) |

### GPT-5.6 Luna *(🔄 Replaced by GPT-6 Luna — still active)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.6-luna` |
| **Input/Output price** | $0.20 / $1.20 per MTok |
| **Migration** | → **`gpt-6-luna`** ($0.10/$0.50) |

---

### 🆕 GPT-5.6 Cyber *(Daybreak Program)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.6-cyber` |
| **Status** | ✅ Active — Daybreak Red alias target; vetted-access cybersecurity model |
| **Input price (short ctx)** | $12.50 / MTok |
| **Output (short ctx)** | $75.00 / MTok |
| **Aliases** | `gpt-daybreak-red-latest` → `gpt-5.6-cyber` · `gpt-daybreak-blue-latest` → `gpt-5.6-sol` |

---

### GPT-Rosalind (Research) *(Life Sciences — Trusted Access)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-rosalind-research` |
| **Status** | ✅ Active — Trusted access only; billing starts Oct 5, 2026 |
| **Input price** | $5.00 / MTok · **Output:** $25.00 / MTok · **Cached:** $0.50 / MTok |

---

### GPT-5.5 *(still fully active in the API — retiring from ChatGPT/Codex Oct 14, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.5` |
| **Status** | ✅ Active on the API — ⚠️ retiring from ChatGPT, ChatGPT Work, and Codex October 14, 2026 (API-key access unaffected) |
| **Input price (std/long ctx)** | $5.00 / $10.00 per MTok |
| **Output price (std/long ctx)** | $30.00 / $45.00 per MTok |
| **Context window** | 1,000,000 tokens |
| **Notable** | Now priced higher than GPT-6 Sol ($5/$30 vs. Sol's $2/$10) |

### GPT-5.5 Pro / GPT-5.4 family / GPT-4.1 family / o3 / o3-pro

| Model | Input (std/long) | Output (std/long) | Context | Notes |
|---|---|---|---|---|
| `gpt-5.5-pro` | $30.00 / $60.00 | $180.00 / $270.00 | 1,000,000 | Ultra-Premium |
| `gpt-5.4` | $2.50 / $5.00 | $15.00 / $22.50 | 1,000,000 | Value mid-tier |
| `gpt-5.4-pro` | $30.00 / $60.00 | $180.00 / $270.00 | 1,050,000 | Superseded by GPT-5.5 Pro at same price |
| `gpt-5.4-mini` | $0.75 | $4.50 | 400,000 | GPT-6 Luna undercuts it dramatically |
| `gpt-5.4-nano` | $0.20 | $1.25 | 400,000 | Budget/high-volume |
| `gpt-4.1` | $2.00 | $8.00 | 1,040,000 | Recommended for long-context |
| `gpt-4.1-mini` | $0.40 | $1.60 | 1,000,000 | Balanced, long-context budget |
| `o3` | $2.00 | $8.00 | 200,000 | ⚠️ `o3-2025-04-16` shuts down Dec 11, 2026 → `gpt-6-sol` |
| `o3-pro` | $20.00 | $80.00 | 200,000 | ⚠️ `o3-pro-2025-06-10` shuts down Dec 11, 2026 → `gpt-6-sol` (`reasoning.mode: pro`) |

---

## 🎙️ Multimodal, Realtime & Specialized Models

### GPT-Live-1 *(Full-Duplex Voice)*

$0.05/minute, billed per second. Backend reasoning/tool-calling model billed separately at standard token rates.

### GPT-Realtime-2.1 / GPT-Realtime-2.1-mini

| Model | Modality | Input | Cached | Output |
|---|---|---|---|---|
| `gpt-realtime-2.1` | Audio | $32.00 | $0.40 | $64.00 |
| | Text | $4.00 | $0.40 | $24.00 |
| | 🆕 Image | $5.00 | $0.50 | — |
| `gpt-realtime-2.1-mini` | Audio | $10.00 | $0.30 | $20.00 |
| | Text | $0.60 | $0.06 | $2.40 |
| | 🆕 Image | $0.80 | $0.08 | — |

### 🆕 GPT-Realtime-Translate *(Streaming speech-to-speech translation)*

$0.034 / minute — new model confirmed on the official pricing page this refresh.

### GPT-Image-2.5 Sunburst / Flare *(Flagship Image Models)*

Image $8.00 in / $2.00 cached / $30.00 out · Text $5.00 in / $1.25 cached (per MTok)

### GPT-Image-2 *(Value Tier — Repriced 50% Cheaper)*

Image $4.00 in / $1.00 cached / $15.00 out · Text $2.50 in / $0.625 cached (per MTok)

### ⚠️ Video generation — Sora-2 / Sora-2-Pro *(❌ SHUT DOWN September 24, 2026)*

> Confirmed via the official Deprecations page (notice issued March 24, 2026): the **Videos API**, `sora-2`, `sora-2-pro`, and dated snapshots `sora-2-2025-10-06`, `sora-2-2025-12-08`, `sora-2-pro-2025-10-06` were all removed from the API on **September 24, 2026**. **No replacement model is listed** ("---" for recommended replacement in OpenAI's own table). This date has now passed — any workload still calling these model IDs is broken.

| Model | Size | Price/sec (standard) | Price/sec (batch) | Shutdown |
|---|---|---|---|---|
| `sora-2` | 720p | $0.10 | $0.05 | ❌ **Sept 24, 2026 (passed)** |
| `sora-2-pro` | 720p/1024p/1080p | $0.30 / $0.50 / $0.70 | $0.15 / $0.25 / $0.35 | ❌ **Sept 24, 2026 (passed)** |

### Transcription Models

| Model | Pricing |
|---|---|
| `gpt-transcribe` | $0.0045 / minute |
| `gpt-live-transcribe` | $0.017 / minute |
| 🆕 `gpt-realtime-whisper` | $0.017 / minute — streaming speech-to-text, distinct from legacy `whisper-1` |
| `gpt-4o-transcribe` | $2.50 input / $10.00 output per MTok (~$0.006/min) — ⚠️ deprecated Aug 26, 2026, shuts down Feb 26, 2027 |
| `gpt-4o-mini-transcribe` | $1.25 input / $5.00 output per MTok (~$0.003/min) — ⚠️ deprecated Aug 26, 2026, shuts down Feb 26, 2027 |
| `whisper-1` | ⚠️ deprecated Aug 26, 2026, shuts down Feb 26, 2027 → `gpt-live-transcribe` or `gpt-transcribe` |

### Deep Research / Computer Use / Codex

| Model | Input | Output |
|---|---|---|
| `o3-deep-research` | $5.00 | $20.00 |
| `o4-mini-deep-research` | $1.00 | $4.00 |
| `computer-use-preview` | $1.50 | $6.00 |
| `gpt-5.3-codex` | $1.75 (cached $0.175) | $14.00 |

---

## 🔧 Tools Pricing

| Tool | Pricing |
|---|---|
| **Web search** (all models) | $10.00 / 1K calls + search content tokens at model rates |
| **Web search preview** (non-reasoning, non-preview) | $25.00 / 1K calls; content tokens free |
| **Containers** | $0.03 (1GB) / $0.12 (4GB) / $0.48 (16GB) / $1.92 (64GB) per 20-min session |
| **File search storage / tool call** | $0.10 / GB-day · $2.50 / 1K calls |
| **GPT-Live-1 voice sessions** | $0.05 / minute |
| **Agents API** | No additional fee — standard token/tool rates apply |
| 🆕 **Decisions API** (public beta, Oct 5, 2026) | Powered by `gpt-6-luna` — $0.10/MTok input only; no cache-read, cache-write, or output-token charges |

---

## 💰 Fine-tuning *(platform winding down)*

| Date | Update |
|---|---|
| May 7, 2026 | New-user fine-tuning creation restricted |
| July 2, 2026 | Job creation restricted to orgs with fine-tuned-model inference in the past 60 days |
| **January 6, 2027** | Active existing customers can no longer create new fine-tuning jobs. Inference on fine-tuned models continues until the underlying base model is deprecated. |

---

## ⚠️ Legacy / Deprecated / Retired Models

### ❌ SHUT DOWN — Videos API, Sora-2, Sora-2-Pro *(shut down September 24, 2026)*

| Model / system | Shutdown | Replacement |
|---|---|---|
| Videos API | ❌ Sept 24, 2026 (passed) | — (none listed) |
| `sora-2` (+ dated snapshots) | ❌ Sept 24, 2026 (passed) | — (none listed) |
| `sora-2-pro` (+ dated snapshots) | ❌ Sept 24, 2026 (passed) | — (none listed) |

### ⚠️ DEPRECATED — GPT-5 snapshot family, o3, and o3-pro *(shuts down December 11, 2026)*

| Model ID | Migration |
|---|---|
| `gpt-5-2025-08-07` | → `gpt-5.6-sol` / `gpt-6-sol` |
| `gpt-5-mini-2025-08-07` | → `gpt-5.6-terra` |
| `gpt-5-nano-2025-08-07` | → `gpt-5.6-luna` / `gpt-6-luna` |
| `gpt-5-pro-2025-10-06` | → `gpt-5.6-sol` (`reasoning.mode: pro`) |
| `o3-2025-04-16` | → `gpt-5.6-sol` / `gpt-6-sol` |
| `o3-pro-2025-06-10` | → `gpt-5.6-sol` (`reasoning.mode: pro`) |

### ⚠️ DEPRECATED — October 23, 2026 wave

| Model ID | Migration |
|---|---|
| `o4-mini` | → `gpt-5.6-terra` |
| `gpt-4.1-nano` | → `gpt-5.6-luna` / `gpt-6-luna` |
| `o1` | → `gpt-5.6-sol` / `gpt-6-sol` |
| `o3-mini` | → `gpt-5.6-sol` / `gpt-6-sol` |
| `o1-pro` | → `gpt-5.6-sol` (`reasoning.mode: pro`) |
| `gpt-image-1` | → `gpt-image-2` |
| `gpt-3.5-turbo-0125`, `gpt-4-0613`, `gpt-4-1106-preview`, `gpt-4-turbo`, `gpt-4o-2024-05-13` | → `gpt-5.6-sol`/`gpt-6-sol` or `gpt-5.6-terra` |

### ⚠️ DEPRECATED — gpt-5.4-cyber *(shuts down October 1, 2026)* → `gpt-5.6-cyber`

### 🆕 ⚠️ DEPRECATED — October 1, 2026 wave *(shuts down April 1, 2027 — 6 months' notice)*

| Model ID | Migration |
|---|---|
| `gpt-5.3-codex` | → `gpt-6-sol` |
| `gpt-5.1` | → `gpt-6-sol` |
| `gpt-5.4-nano` | → `gpt-6-luna` |

### 🆕 ⚠️ DEPRECATED — Legacy text-to-speech *(shuts down January 6, 2027)*

| Model ID | Migration |
|---|---|
| `tts-1` | → `gpt-realtime-2.1-mini` |
| `tts-1-hd` | → `gpt-realtime-2.1-mini` |
| `gpt-4o-mini-tts-2025-03-20` | → `gpt-realtime-2.1-mini` |
| `gpt-4o-mini-tts-2025-12-15` | → `gpt-realtime-2.1-mini` |

### ⚠️ DEPRECATED — Legacy audio/realtime/transcription *(shuts down January 20, 2027 / February 26, 2027)*

| Model family | Shutdown | Replacement |
|---|---|---|
| `gpt-realtime`, `gpt-4o-realtime` | Jan 20, 2027 | `gpt-realtime-2.1` |
| `gpt-realtime-mini`, `gpt-4o-mini-realtime` | Jan 20, 2027 | `gpt-realtime-2.1-mini` |
| `gpt-audio`, `gpt-4o-audio`, `gpt-audio-mini`, `gpt-4o-mini-audio` | Jan 20, 2027 | `gpt-audio-1.5` |
| `whisper-1`, `gpt-4o-transcribe`, `gpt-4o-mini-transcribe`, `gpt-4o-transcribe-diarize` | Feb 26, 2027 | `gpt-live-transcribe` or `gpt-transcribe` |

### 🆕 ⚠️ PRODUCT-SURFACE RETIREMENT — GPT-5.5 leaves ChatGPT/Codex October 14, 2026 *(API unaffected)*

### 🔄 REPLACED — GPT-6 Sol *(Superseded by GPT-6.1 Sol, Sept 29, 2026 — removed from pricing/model catalog after 7 days)*

| Field | Value |
|---|---|
| **Pricing (while active)** | $2.00 / MTok input · $10.00 / MTok output · $0.20/MTok cached input |
| **Migration** | → **`gpt-6.1-sol`** — identical headline price, cached input now $0.10/MTok (95% off vs. 90%) |

### 🔄 REPLACED — GPT-5.6 Sol / GPT-5.6 Luna *(replaced by GPT-6.1 Sol / GPT-6 Luna — still active)*

| Model | Migration |
|---|---|
| GPT-5.6 Sol | → GPT-6.1 Sol ($2/$10, 50% cheaper); promo pricing confirmed to run at least through Nov 21, 2026; retained for Daybreak Blue alias |
| GPT-5.6 Luna | → GPT-6 Luna ($0.10/$0.50, 50% cheaper) |

### ⚠️ LEGACY — GPT-5.3 / Codex, GPT-5.2, GPT-5.1, GPT-4o, GPT-4o mini, GPT-4 Turbo/3.5 Turbo family

| Model | Status | Migration |
|---|---|---|
| `gpt-5.3-codex` | ⚠️ DEPRECATED Oct 1, 2026 — shuts down **April 1, 2027** | → GPT-6.1 Sol / GPT-6 Sol |
| `gpt-5.3` | LEGACY | → GPT-5.6 Terra or GPT-6.1 Sol |
| `gpt-5.2` | LEGACY — retired from ChatGPT June 12, 2026 | → GPT-5.6 Terra or GPT-5.4 |
| `gpt-5.1` (API model) | ⚠️ DEPRECATED Oct 1, 2026 — shuts down **April 1, 2027** | → GPT-6.1 Sol / GPT-6 Sol |
| `gpt-5.4-nano` | ⚠️ DEPRECATED Oct 1, 2026 — shuts down **April 1, 2027** | → GPT-6 Luna |
| `gpt-4o` | LEGACY — dated snapshot shuts down Oct 23, 2026 | → GPT-4.1 or GPT-6.1 Sol |
| `gpt-4o-mini` | LEGACY | → GPT-6 Luna or GPT-4.1 nano *(also deprecated)* |
| GPT-4 Turbo / GPT-3.5 Turbo family | Shuts down Oct 23, 2026 / Sept 28, 2026 | → GPT-6.1 Sol / GPT-6 Luna |

---

## 💡 Cost Optimization Notes

| Feature | Savings |
|---|---|
| **🆕 GPT-6.1 Sol replaces GPT-6 Sol at the same headline price** | $2/$10 unchanged; cached input drops to $0.10/MTok (95% off, was 90%) — released just 7 days after GPT-6 Sol |
| **🆕 Ultrafast tier now priced for GPT-6 Astra** | 6× standard price ($60/$300 short ctx) for up to 6× API / 8× Codex speed; GPT-6.1 Sol Ultrafast "coming soon" |
| **GPT-6 Luna is 50% cheaper than GPT-5.6 Luna** | $0.20→$0.10 in / $1.20→$0.50 out |
| **GPT-6 caching now hits more often by default** | 30-minute reuse window, `configuration_update` lets you change reasoning effort or tools mid-conversation without losing cache |
| **GPT-6 Astra is still the premium ceiling** | $10/$50 short ctx — unchanged |
| **GPT-5.6 Terra confirmed unchanged** | $2.00/$12.00, still "Default" on the model catalog — no GPT-6 equivalent yet; official migration target for `o4-mini` |
| **GPT-5.6 Sol promotional pricing extended** | Confirmed by OpenAI's pricing page to run at least through **November 21, 2026** |
| **⚠️ Sora-2 / Sora-2-Pro / Videos API SHUT DOWN Sept 24, 2026 (passed)** | No replacement listed — any workload still calling these model IDs is now broken |
| ⚠️ **`GPT-6 Cyber` did NOT appear at DevDay (Sept 29)** | Despite pre-event reporting, OpenAI's official DevDay recap has no mention of it — remains discovery-only, unpriced |
| 🆕 **New deprecation wave (Oct 1, 2026)**: `gpt-5.3-codex`, `gpt-5.1`, `gpt-5.4-nano` shut down **Apr 1, 2027**; legacy TTS (`tts-1`, `tts-1-hd`, old `gpt-4o-mini-tts` snapshots) shut down **Jan 6, 2027** | Migrate to GPT-6.1 Sol / GPT-6 Luna / `gpt-realtime-2.1-mini` respectively |
| **⚠️ o3/o3-pro/GPT-5 snapshots shut down Dec 11, 2026; o1/o3-mini/o1-pro/o4-mini/gpt-4.1-nano/gpt-image-1 shut down Oct 23, 2026** | Migrate well ahead of both waves |
| **GPT-5.5 leaves ChatGPT/Codex Oct 14, 2026 — API unaffected** | Only ChatGPT-authenticated sessions affected |
| **🆕 GPT-Rosalind Research billing now live (Oct 5, 2026)** | $5/$25 per MTok, trusted-access only |
| **Fine-tuning platform winding down** | New jobs blocked entirely from Jan 6, 2027 |
| **Regional processing** | +10% uplift for GPT-6/5.6/5.5/5.4 family data-residency endpoints |

---

*Sources last verified: October 7, 2026 against `developers.openai.com/api/docs/pricing`, `.../api/docs/models`, `.../api/docs/deprecations`, and `openai.com/news/`. **This refresh:** no pricing or lineup changes found since October 5 — GPT-6 Astra, GPT-6.1 Sol, GPT-6 Luna, GPT-5.6 Terra/Sol/Luna/Cyber, and GPT-Rosalind Research pricing all re-confirmed unchanged. New: Decisions API launched in public beta (Oct 5, 2026), powered by `gpt-6-luna`, billed at $0.10/MTok input only (no output/cache charges). Noted a non-pricing infrastructure rollout (~50% default output-speed increase for GPT-6 Astra/GPT-6.1 Sol via subscriptions, Oct 5–7, 2026). Re-confirmed `GPT-6 Cyber` remains unannounced by OpenAI — no official pricing, model ID, or launch date published. The October 1, 2026 deprecation wave (`gpt-5.3-codex`/`gpt-5.1`/`gpt-5.4-nano`, legacy TTS) remains unchanged.*
