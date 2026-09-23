# 🟢 OpenAI — Model Cards

> **Last updated:** 2026-09-23
> **Source:** https://developers.openai.com/api/docs/pricing · https://developers.openai.com/api/docs/models · https://developers.openai.com/api/docs/deprecations · https://openai.com/index/gpt-6-astra/ · https://openai.com/index/introducing-gpt-6-sol-and-luna/ · https://openai.com/index/better-prompt-caching-for-gpt-6/ · https://openai.com/news
> **Scraped / verified:** 2026-09-23 — ✅ Re-confirmed GPT-6 Astra/Sol/Luna pricing (launched/expanded Sept 3 and Sept 22, 2026) is unchanged. 🆕 **NEW this cycle: confirmed via the official Deprecations page that the Videos API, `sora-2`, and `sora-2-pro` (+ dated snapshots) are deprecated and shut down September 24, 2026 — one day after this refresh, with no replacement model listed.** ✅ **Directly verified GPT-5.6 Terra's dedicated model page: it remains fully active and unchanged** at $2.00/$12.00 per MTok, still labeled "Default" on OpenAI's model catalog — there is still no GPT-6 Terra equivalent.

All prices are **USD per million tokens (MTok)** unless noted. Batch/Flex API gives a flat **50% discount** on all models. Cached input tokens get **50–90% off** depending on model.

> **Context tiers for GPT-6, GPT-5.6, GPT-5.5, and GPT-5.4:** Standard ("short context") pricing applies for prompts **under ~272K tokens**. The long-context tier applies **2× input / 1.5× output** vs. short-context rates.
>
> **Service tiers:** Priority/Fast mode (2× standard price), Standard (default), Batch, and Flex (50% off standard).

> 🆕 **September 22, 2026 — GPT-6 Sol and GPT-6 Luna launched**, expanding the GPT-6 family alongside GPT-6 Astra (launched Sept 3). Both trained with methods similar to Astra, bringing its professional-work, factuality, coding, computer-use, and alignment gains to cheaper, faster models — **at 50% lower API prices than their GPT-5.6 promotional-era predecessors**:
>
> | Model | Input | Output | Change |
> |---|---|---|---|
> | GPT-5.6 Sol → **GPT-6 Sol** | $4 → **$2** | $20 → **$10** | 50% cheaper |
> | GPT-5.6 Luna → **GPT-6 Luna** | $0.20 → **$0.10** | $1.20 → **$0.50** | 50% cheaper |
>
> **GPT-6 Astra remains OpenAI's best model overall**, unchanged at $10/$50. **There is no GPT-6 Terra** — GPT-5.6 Terra ($2.00/$12.00 per MTok) is confirmed unchanged and remains the live, un-replaced mid-tier model, still labeled "Default" on the live model catalog. GPT-6 Sol and Luna are available in ChatGPT Work, Codex, and the API (`gpt-6-sol`, `gpt-6-luna`); Free/Go users get GPT-6 Luna in the desktop app. GPT-5.6 Sol and Luna remain fully priced and active at their prior (promotional) rates with no announced shutdown date — `gpt-5.6-sol` also continues to back the `gpt-daybreak-blue-latest` alias and the `gpt-5.6-cyber` pricing baseline.
>
> 🆕 **September 22, 2026 — Better prompt caching for GPT-6.** Higher default cache-hit rates, a 30-minute eligibility window for reused shared prefixes, a new Prompt Caching Dashboard and cache-miss diagnostics tool, and the ability to change `reasoning_effort` or tools mid-conversation without breaking the cache via `configuration_update`. GitHub reports this cut the share of prompt tokens requiring fresh processing by more than 50% across billions of requests. This is a caching-mechanics improvement, not a price change.
>
> ⚠️ **NEW — Videos API, Sora-2, and Sora-2-Pro deprecated, shutting down September 24, 2026.** Confirmed via the official Deprecations page (notice issued March 24, 2026): the Videos API, `sora-2`, `sora-2-pro`, and their dated snapshots (`sora-2-2025-10-06`, `sora-2-2025-12-08`, `sora-2-pro-2025-10-06`) are all removed from the API on **September 24, 2026** — one day after this refresh, with **no replacement model listed**. Treat as immediately actionable for any video-generation workloads.
>
> ⚠️ **`o3`, `o3-pro`, and the original GPT-5 launch snapshot family shut down December 11, 2026** — a separate, later wave than the October 23, 2026 cull (notice issued June 11, 2026). All map to `gpt-5.6-sol`/`terra`/`luna` per OpenAI's official mapping.
>
> 🆕 **September 15, 2026 — GPT-5.5 retires from ChatGPT, ChatGPT Work, and Codex on October 14, 2026 (API unaffected).**
>
> 🆕 **~September 17, 2026 — "Astra for Law" launched** — a GPT-6-Astra-based legal vertical for law firms/legal-tech (Harvey, Legora); billed at standard GPT-6 Astra rates, not a new SKU.

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
| **Batch/Flex (short: input/cached/write/output)** | $5.00 / $0.50 / $6.25 / $25.00 |
| **Context window** | 1,050,000 tokens |
| **Max output** | 128,000 tokens |
| **Knowledge cutoff** | April 30, 2026 |
| **Reasoning effort** | `low`, `medium`, `high`, `xhigh`, `max` — **`none` not supported** |
| **Availability** | ChatGPT Plus/Pro/Business/Enterprise · GPT-6 Astra Pro · OpenAI API · Microsoft Azure/Foundry · AWS Bedrock |

---

### 🆕 GPT-6 Sol *(Released September 22, 2026 — Best Price/Performance)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-6-sol` |
| **Status** | ✅ Active — replaces GPT-5.6 Sol as the "balance intelligence and cost" tier |
| **Input (short ctx)** | 📉 **$2.00** / MTok *(was GPT-5.6 Sol's $4.00 promo — 50% cheaper)* |
| **Cached input (short)** | $0.20 / MTok |
| **Output (short ctx)** | 📉 **$10.00** / MTok *(was $20.00)* |
| **Input (long ctx)** | $4.00 / MTok |
| **Output (long ctx)** | $15.00 / MTok |
| **Fast mode (short: input/cached/write/output)** | $4.00 / $0.40 / $5.00 / $20.00 |
| **Batch/Flex (short input/output)** | $1.00 / $5.00 |
| **Context window** | 1,050,000 tokens |
| **Max output** | 128,000 tokens |
| **Knowledge cutoff** | April 20, 2026 |
| **Reasoning effort** | `none`, `low`, `medium`, `high`, `xhigh`, `max` |
| **Availability** | ChatGPT Work, Codex (Plus/Pro/Business/Enterprise/Edu) · OpenAI API — **not yet in plain ChatGPT Chat** |
| **Notable** | On AutomationBench, beats Claude Opus 5 (max effort) at 9% of its cost per task at `xhigh` effort; on DeepSWE v1.1, scores 68.8% at max effort — within 1.1 points of Claude Fable 5's best score at ~80% lower cost per task |

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

### GPT-5.6 Sol *(⚠️ Superseded for general use by GPT-6 Sol — still active, backs Daybreak Blue alias)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.6-sol` |
| **Status** | ⚠️ 🔄 Replaced by GPT-6 Sol for general use — still active; also backs `gpt-daybreak-blue-latest` and the `gpt-5.6-cyber` pricing baseline |
| **Input (short ctx)** | $4.00 / MTok |
| **Output (short ctx)** | $20.00 / MTok |
| **Migration (general use)** | → **`gpt-6-sol`** ($2/$10 — 50% cheaper) |

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
| `gpt-realtime-2.1-mini` | Audio | $10.00 | $0.30 | $20.00 |
| | Text | $0.60 | $0.06 | $2.40 |

### GPT-Image-2.5 Sunburst / Flare *(Flagship Image Models)*

Image $8.00 in / $2.00 cached / $30.00 out · Text $5.00 in / $1.25 cached (per MTok)

### GPT-Image-2 *(Value Tier — Repriced 50% Cheaper)*

Image $4.00 in / $1.00 cached / $15.00 out · Text $2.50 in / $0.625 cached (per MTok)

### ⚠️ Video generation — Sora-2 / Sora-2-Pro *(🆕 DEPRECATED — shuts down September 24, 2026)*

> **New this refresh:** Confirmed via the official Deprecations page (notice issued March 24, 2026): the **Videos API**, `sora-2`, `sora-2-pro`, and dated snapshots `sora-2-2025-10-06`, `sora-2-2025-12-08`, `sora-2-pro-2025-10-06` are all removed from the API on **September 24, 2026**. **No replacement model is listed** ("---" for recommended replacement in OpenAI's own table). This is only one day after this refresh — treat as urgent for any workload depending on Sora-2 video generation.

| Model | Size | Price/sec (standard) | Price/sec (batch) | Shutdown |
|---|---|---|---|---|
| `sora-2` | 720p | $0.10 | $0.05 | **Sept 24, 2026** |
| `sora-2-pro` | 720p/1024p/1080p | $0.30 / $0.50 / $0.70 | $0.15 / $0.25 / $0.35 | **Sept 24, 2026** |

### Transcription Models

| Model | Pricing |
|---|---|
| `gpt-transcribe` | $0.0045 / minute |
| `gpt-live-transcribe` | $0.017 / minute |
| `gpt-4o-transcribe` / `gpt-4o-mini-transcribe` / `whisper-1` | ⚠️ deprecated Aug 26, 2026, shut down Feb 26, 2027 |

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

---

## 💰 Fine-tuning *(platform winding down)*

| Date | Update |
|---|---|
| May 7, 2026 | New-user fine-tuning creation restricted |
| July 2, 2026 | Job creation restricted to orgs with fine-tuned-model inference in the past 60 days |
| **January 6, 2027** | Active existing customers can no longer create new fine-tuning jobs. Inference on fine-tuned models continues until the underlying base model is deprecated. |

---

## ⚠️ Legacy / Deprecated / Retired Models

### 🆕 ⚠️ DEPRECATED — Videos API, Sora-2, Sora-2-Pro *(shuts down September 24, 2026)*

| Model / system | Shutdown | Replacement |
|---|---|---|
| Videos API | Sept 24, 2026 | — (none listed) |
| `sora-2` (+ dated snapshots) | Sept 24, 2026 | — (none listed) |
| `sora-2-pro` (+ dated snapshots) | Sept 24, 2026 | — (none listed) |

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

### ⚠️ DEPRECATED — Legacy audio/realtime/transcription *(shuts down January 20, 2027 / February 26, 2027)*

| Model family | Shutdown | Replacement |
|---|---|---|
| `gpt-realtime`, `gpt-4o-realtime` | Jan 20, 2027 | `gpt-realtime-2.1` |
| `gpt-realtime-mini`, `gpt-4o-mini-realtime` | Jan 20, 2027 | `gpt-realtime-2.1-mini` |
| `gpt-audio`, `gpt-4o-audio`, `gpt-audio-mini`, `gpt-4o-mini-audio` | Jan 20, 2027 | `gpt-audio-1.5` |
| `whisper-1`, `gpt-4o-transcribe`, `gpt-4o-mini-transcribe`, `gpt-4o-transcribe-diarize` | Feb 26, 2027 | `gpt-live-transcribe` or `gpt-transcribe` |

### 🆕 ⚠️ PRODUCT-SURFACE RETIREMENT — GPT-5.5 leaves ChatGPT/Codex October 14, 2026 *(API unaffected)*

### 🔄 REPLACED — GPT-5.6 Sol / GPT-5.6 Luna *(replaced by GPT-6 Sol/Luna, Sept 22, 2026 — still active)*

| Model | Migration |
|---|---|
| GPT-5.6 Sol | → GPT-6 Sol ($2/$10, 50% cheaper) for general use; retained for Daybreak Blue alias |
| GPT-5.6 Luna | → GPT-6 Luna ($0.10/$0.50, 50% cheaper) |

### ⚠️ LEGACY — GPT-5.3 / Codex, GPT-5.2, GPT-5.1, GPT-4o, GPT-4o mini, GPT-4 Turbo/3.5 Turbo family

| Model | Status | Migration |
|---|---|---|
| `gpt-5.3` / `gpt-5.3-codex` | LEGACY | → GPT-5.6 Terra or GPT-6 Sol |
| `gpt-5.2` | LEGACY — retired from ChatGPT June 12, 2026 | → GPT-5.6 Terra or GPT-5.4 |
| `gpt-5.1` (all variants) | RETIRED March 11, 2026 | → GPT-6 family |
| `gpt-4o` | LEGACY — dated snapshot shuts down Oct 23, 2026 | → GPT-4.1 or GPT-6 Sol |
| `gpt-4o-mini` | LEGACY | → GPT-6 Luna or GPT-4.1 nano *(also deprecated)* |
| GPT-4 Turbo / GPT-3.5 Turbo family | Shuts down Oct 23, 2026 / Sept 28, 2026 | → GPT-6 Sol / GPT-6 Luna |

---

## 💡 Cost Optimization Notes

| Feature | Savings |
|---|---|
| **GPT-6 Sol/Luna are 50% cheaper than GPT-5.6 Sol/Luna** | Sol: $4→$2 in / $20→$10 out. Luna: $0.20→$0.10 in / $1.20→$0.50 out |
| **GPT-6 caching now hits more often by default** | 30-minute reuse window, `configuration_update` lets you change reasoning effort or tools mid-conversation without losing cache |
| **GPT-6 Astra is still the premium ceiling** | $10/$50 short ctx — unchanged |
| **GPT-5.6 Terra confirmed unchanged** | $2.00/$12.00, still "Default" on the model catalog — no GPT-6 equivalent yet; official migration target for `o4-mini` |
| **⚠️ Sora-2 / Sora-2-Pro / Videos API shut down Sept 24, 2026** | No replacement listed — urgent for any video-generation workloads |
| **⚠️ o3/o3-pro/GPT-5 snapshots shut down Dec 11, 2026; o1/o3-mini/o1-pro/o4-mini/gpt-4.1-nano/gpt-image-1 shut down Oct 23, 2026** | Migrate well ahead of both waves |
| **GPT-5.5 leaves ChatGPT/Codex Oct 14, 2026 — API unaffected** | Only ChatGPT-authenticated sessions affected |
| **Fine-tuning platform winding down** | New jobs blocked entirely from Jan 6, 2027 |
| **Regional processing** | +10% uplift for GPT-6/5.6/5.5/5.4 family data-residency endpoints |

---

*Sources last verified: September 23, 2026 against `developers.openai.com/api/docs/pricing`, `.../api/docs/models`, `.../api/docs/models/gpt-5.6-terra`, `.../api/docs/deprecations`, and `openai.com/news`. **This cycle's finding:** confirmed a new deprecation — the Videos API, Sora-2, and Sora-2-Pro shut down September 24, 2026 with no replacement model listed. Also directly verified GPT-5.6 Terra's own model page: it is unchanged and remains the active, un-replaced "Default" mid-tier model at $2.00/$12.00. GPT-6 Astra/Sol/Luna pricing (launched Sept 3 and Sept 22, 2026) is confirmed unchanged. All other active and legacy model prices were re-confirmed unchanged.*
