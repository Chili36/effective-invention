# 🤖 LLM Pricing Tracker

Up-to-date pricing and specifications for large language models from **Anthropic**, **OpenAI**, **Google Gemini**, **Mistral AI**, and top **OpenRouter picks**.

> **Last updated:** 2026-09-14 (refresh #32)
> **Sources:** Official provider pricing pages — scraped/verified on date above.

---

## 📋 Quick-Reference Index — Active Models

### 🟠 Tier 1 — Anthropic Claude

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Max Output | Availability |
|---|---|---|---|---|---|
| 🆕 **Claude Fable 5.1** *(Released Sept 1, 2026 — Most Advanced Model)* | $10.00 | $50.00 | **1M tokens** | 128k | Claude API, Claude.ai, Claude Code, Claude Cowork, AWS, Google Cloud, Azure |
| 🔒 **Claude Mythos 5.1** *(Trusted Access — Sept 1, 2026)* | $10.00 | $50.00 | **1M tokens** | 128k | CVP / LSVP trusted-access programs |
| **Claude Opus 5** *(Default on Max / strongest on Pro)* | $5.00 | $25.00 | **1M tokens** | 128k sync / 300k Batch | API, AWS Bedrock, Claude Platform on AWS, Google Cloud, MS Foundry |
| **Claude Opus 4.8** *(🔄 replaced by Opus 5 — still active)* | $5.00 | $25.00 | **1M tokens** | 128k sync / 300k Batch | API, AWS Bedrock (Messages API), Vertex AI, MS Foundry (200k ctx) |
| ✅ **Claude Sonnet 5** *(Default Sonnet-tier — $2/$10 now PERMANENT)* | $2.00 | $10.00 | **1M tokens** | 128k sync / 300k Batch | API, Claude.ai, Claude Code, AWS Bedrock, Google Cloud, MS Foundry |
| **Claude Sonnet 4.6** *(🔄 replaced by Sonnet 5 as default)* | $3.00 | $15.00 | **1M tokens** | 64k sync / 300k Batch | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Haiku 4.5** | $1.00 | $5.00 | 200K tokens | 64k | API, AWS Bedrock (all regions), Vertex AI, MS Foundry |

> 💡 Batch API: 50% off · Prompt caching: up to 90% off (up to **97.5% off** cache reads on Fable 5.1/Mythos 5.1)
> ✅ **September 14, 2026 refresh:** Every Anthropic price point re-verified against the live `platform.claude.com/docs/en/about-claude/pricing` and `claude.com/pricing` pages — **zero changes** since Sept 7. Only new item: a Sept 10, 2026 Threat Intelligence report (non-pricing).
> 🆕 Claude Fable 5.1 and Mythos 5.1 launched Sept 1, 2026 — same $10/$50 base price as Fable 5/Mythos 5, but cache-read pricing cut 75% (to $0.25/MTok), cutting typical workload costs by ~25% and highly agentic workload costs by up to ~45%.
> ✅ Claude Sonnet 5's $2/$10 pricing is confirmed **permanent** — the scheduled Sept 1 increase to $3/$15 did not occur.

---

### 🟢 Tier 1 — OpenAI (Proprietary)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|---|
| 🆕 **GPT-6 Astra** *(New Flagship — Released Sept 3, 2026)* | $10.00 / $20.00* | $1.00 / $2.00* | $50.00 / $75.00* | **1.05M tokens** | ChatGPT, API, Azure/Foundry, AWS Bedrock |
| 📉 **GPT-5.6 Sol** *(🔄 replaced as flagship — now promotionally priced)* | $4.00 / $8.00* | $0.40 / $0.80* | $20.00 / $30.00* | **~1.05M tokens** | ChatGPT, Codex, API — self-serve |
| **GPT-5.6 Terra** *(Best price/performance)* | $2.00 / $4.00* | $0.20 / $0.40* | $12.00 / $18.00* | **~1.05M tokens** | ChatGPT, Codex, API — self-serve |
| **GPT-5.6 Luna** *(Fastest/cheapest tier — default for ChatGPT Free/Go)* | $0.20 / $0.40* | $0.02 / $0.04* | $1.20 / $1.80* | **~1.05M tokens** | ChatGPT, Codex, API — self-serve |
| **GPT-5.6 Cyber** *(Daybreak program)* | $12.50 | $1.25 | $75.00 | ~1.05M tokens | Vetted access (Daybreak) |
| 🆕 **GPT-Rosalind (Research)** *(Life Sciences, trusted access — billing from Oct 5, 2026)* | $5.00 | $0.50 | $25.00 | — | Trusted-access program only |
| **GPT-5.5** *(still active, same price)* | $5.00 / $10.00* | $0.50 / $1.00* | $30.00 / $45.00* | **1M tokens** | API |
| **GPT-5.5 Pro** | $30.00 / $60.00* | — | $180.00 / $270.00* | 1M tokens | API |
| GPT-5.4 *(prev flagship)* | $2.50 / $5.00† | $0.25 / $0.50† | $15.00 / $22.50† | 1M tokens | API |
| GPT-5.4 Pro | $30.00 / $60.00* | — | $180.00 / $270.00* | 1.05M tokens | API |
| **GPT-5.4 mini** | $0.75 | $0.075 | $4.50 | 400K tokens | API |
| **GPT-5.4 nano** | $0.20 | $0.020 | $1.25 | 400K tokens | API |
| GPT-4.1 | $2.00 | $0.50 | $8.00 | 1.04M tokens | API |
| **GPT-4.1 mini** | $0.40 | $0.10 | $1.60 | 1.00M tokens | API |
| o3 *(reasoning)* | $2.00 | $0.50 | $8.00 | 200K tokens | API |
| o3-pro *(reasoning)* | $20.00 | — | $80.00 | 200K tokens | API |

> ⚠️ **`o4-mini` and `GPT-4.1 nano` are now DEPRECATED** (confirmed Sept 14, 2026 via the official Deprecations page) — both **shut down October 23, 2026**. Removed from this active table; see the Legacy section below for migration targets (`gpt-5.6-terra` and `gpt-5.6-luna` respectively).
> 💡 Batch/Flex API: 50% off all models · Cached inputs: 50–90% off · Regional processing: +10% on GPT-6 Astra/5.6/5.5/5.4 family
> 🆕 **GPT-Live-1 launched in the API (Sept 10, 2026)** at **$0.05/minute** for the voice layer — previously ChatGPT-only/unpriced. Backend model + tools billed separately at standard rates.
> 🆕 **Agents API launched in public beta (Sept 10, 2026)** — a managed Codex-harness agent runtime with **no additional fees**; billed at standard token/tool rates.
> 🆕 **GPT-Image-2.5 Sunburst/Flare** are the new flagship image models ($8/$2/$30 image, $5/$1.25 text) — the same price GPT-Image-2 used to carry. **GPT-Image-2 was repriced 50% cheaper** ($4/$1/$15 image, $2.50/$0.625 text) and is now the value-tier active option (not deprecated).
> 🆕 **`gpt-rosalind-research`** (Life Sciences, trusted access) gained published pricing — billing begins October 5, 2026.
> 🆕 **GPT-6 Astra launched September 3, 2026** — OpenAI's new flagship, "our most intelligent model yet," and OpenAI's first model to reach the **"Critical"** cybersecurity capability threshold under its Preparedness Framework. 1.05M context, 128K max output, Apr 30 2026 knowledge cutoff.
> 📉 **GPT-5.6 Sol demoted to promotional pricing (Sept 3, 2026):** $5.00/$30.00 → **$4.00/$20.00** (short context), available at least through November 21, 2026, as GPT-6 Astra takes over as flagship.
> *GPT-6 Astra / GPT-5.6 / GPT-5.5 / GPT-5.5 Pro / GPT-5.4 Pro long-context pricing (>~270–272K tokens): standard × 2 input / × 1.5 output (× 2 for Pro models)
> †GPT-5.4 tiered pricing: short ctx (<~270K) / long ctx (>~270K)
> 🔧 **Tools pricing confirmed unchanged:** Web Search $10/1K calls (all models + reasoning-preview) or $25/1K calls (non-reasoning preview, free content tokens) · Computer Use (`computer-use-preview`) $1.50/$6.00 · Containers $0.03–$1.92 per 20-min session · File Search $0.10/GB-day storage + $2.50/1K tool calls · 🆕 GPT-Live-1 sessions $0.05/min · 🆕 Agents API no extra fee.
> ✅ Re-verified September 14, 2026 against the live `developers.openai.com/api/docs/pricing`, `developers.openai.com/api/docs/models`, and `developers.openai.com/api/docs/deprecations`. GPT-6 Astra / GPT-5.6 family pricing unchanged; GPT-5.5, GPT-5.4, GPT-4.1, o3/o3-pro individually spot-checked and confirmed still active.

**Multimodal / Specialized:**

| Model | Pricing |
|---|---|
| 🆕 GPT-Live-1 | **Now priced: $0.05/minute** (API, Sept 10, 2026) — backend model/tools billed separately |
| GPT-Live-1 mini | Referenced in ChatGPT; no confirmed standalone API price yet |
| gpt-realtime-2.1 | Audio $32/$64 · Text $4/$24 · Image $5 input (per MTok) |
| gpt-realtime-2.1-mini | Audio $10/$20 · Text $0.60/$2.40 · Image $0.80 input (per MTok) |
| gpt-realtime-translate | $0.034 / minute |
| gpt-realtime-whisper | $0.017 / minute |
| gpt-live-transcribe | $0.017 / minute |
| gpt-transcribe | $0.0045 / minute |
| ⚠️ gpt-4o-transcribe / gpt-4o-mini-transcribe / whisper-1 | DEPRECATED Aug 26, 2026 — shut down Feb 26, 2027 → gpt-live-transcribe or gpt-transcribe |
| 🆕 gpt-image-2.5-sunburst / gpt-image-2.5-flare | **New flagship image models** — Image $8 input/$2 cached/$30 output · Text $5 input/$1.25 cached (per MTok) |
| gpt-image-2 | 📉 **Repriced 50% cheaper** — Image $4 input/$1 cached/$15 output · Text $2.50 input/$0.625 cached (per MTok) — now value tier, not flagship |
| ⚠️ gpt-image-1.5 | DEPRECATED — shutdown Dec 1, 2026 → migrate to gpt-image-2 |
| ⚠️ gpt-image-1-mini | DEPRECATED — shutdown Dec 1, 2026 → migrate to gpt-image-2 |
| ⚠️ gpt-image-1 | DEPRECATED — shutdown **Oct 23, 2026** → migrate to gpt-image-2 |
| ⚠️ gpt-4o-mini-tts | DEPRECATED |
| sora-2 | $0.10 / sec (720p) |
| sora-2-pro | $0.30–$0.70 / sec (720p–1080p) |
| o3-deep-research | $5.00 input / $20.00 output per MTok |
| o4-mini-deep-research | $1.00 input / $4.00 output per MTok |
| **computer-use-preview** | $1.50 input / $6.00 output per MTok |
| 🆕 **gpt-rosalind-research** | $5.00 input / $0.50 cached / $25.00 output per MTok (billing from Oct 5, 2026) |

---

### 🔵 Tier 1 — Google Gemini

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Notes |
|---|---|---|---|---|
| **Gemini 3.5 Flash** *(Flagship — May 19, 2026)* | $1.50 | $9.00 | **1M tokens** | GA Stable; thinking supported |
| **Gemini 3.1 Pro Preview** | $2.00 / $4.00* | $12.00 / $18.00* | **1M tokens** | *Tiered at >200K; Preview |
| **Gemini 3.1 Flash-Lite** *(Stable GA)* | $0.25 | $1.50 | **1M tokens** | GA Stable (May 2026) |
| **Gemini 2.5 Pro** | $1.25 / $2.50* | $10.00 / $15.00* | **1M tokens** | *Tiered at >200K; GA |
| **Gemini 2.5 Flash** | $0.30 | $2.50 | **1M tokens** | GA; optional thinking mode |
| **Gemini 2.5 Flash-Lite** | $0.10 | $0.40 | **1M tokens** | GA; cheapest Gemini |
| ~~Gemini 2.0 Flash~~ ⚠️ | $0.10 | $0.40 | 1M tokens | ⚠️ **DEPRECATED — Shutdown June 1, 2026** |

> 💡 Batch API: 50% off · Context caching: 90% off repeated prefixes · Free tier via AI Studio
> ℹ️ Gemini pricing not re-verified in this update cycle (out of scope for this refresh — see `gemini.md` for last confirmed figures).

---

### 🟡 Tier 1 — Mistral AI

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Z.ai GLM-5.2** *(First third-party model on Mistral — Aug 11, 2026)* | $1.40 | $4.40 | **1M tokens** | Mistral AI Studio |
| **Mistral Medium 3.5** *(Apr 29, 2026)* | $1.50 | $7.50 | 256K tokens | API |
| **Mistral Large 3 (2512)** | $0.50 | $1.50 | 256K tokens | API |
| **Magistral Medium** *(latest)* | $2.00 | $5.00 | 128K tokens | API |
| Magistral Small *(latest)* | $0.50 | $1.50 | 128K tokens | API |
| **Mistral Small 4** | $0.15 | $0.60 | **256K tokens** | API |
| Codestral 2508 | $0.30 | $0.90 | 256K tokens | API |
| **Devstral 2** *(devstral-medium-latest)* | $0.40 | $2.00 | 256K tokens | API |
| **Devstral Small 2** [Labs] | $0.10 | $0.30 | **256K tokens** | API |
| **Leanstral 1.5** [Labs] ⚠️ *(retiring Sep 30, 2026)* | Free | Free | 256K tokens | API (`leanstral-1-5`) |
| Voxtral Small 24B | $0.004/min (audio) | $0.40 | 128K tokens | API |
| **Voxtral Mini Transcribe 2** (Premier) | $0.003/min | — | — | API |
| **Voxtral Mini Transcribe Realtime** (Open) | $0.006/min | — | — | API |
| Voxtral TTS | $0.016/1K chars | — | — | API |
| **OCR 4.1** *(flagship OCR)* | $4.00/1K pages | $2.00/1K pages (Batch) · $5.00/1K pages (DocAI) | — | API |
| **Classifier API 3B** | $0.10 + $1/MTok training | $0.10 | — | API |
| **Classifier API 8B** | $0.04 + $1/MTok training | $0.04 | — | API |
| **Codestral Embed** *(Premier)* | $0.15 (input only) | — | — | API |
| **Mistral Embed** | $0.10 (input only) | — | — | API |
| **Mistral Moderation 2** | $0.10 (input only) | — | — | API |
| Mistral Nemo | $0.15 | $0.15 | 128K tokens | API |
| Ministral 3 14B | $0.20 | $0.20 | 256K tokens | API |
| Ministral 3 8B | $0.15 | $0.15 | 256K tokens | API |
| Ministral 3 3B | $0.10 | $0.10 | 256K tokens | API |
| Mixtral 8x22B *(legacy API)* | $2.00 | $6.00 | 64K tokens | API |
| Mixtral 8x7B *(legacy API)* | $0.70 | $0.70 | 32K tokens | API |

> 💡 Batch API: 50% off · EU/US Regional Endpoints (GA, +10% surcharge) · Mistral Priority Tier (public preview, SLA-backed)
> ✅ **September 14, 2026 refresh:** Every Mistral price point re-verified against the live `mistral.ai/pricing/api` page — **zero changes** since Sept 7. Only new item: Mistral raised a €3B Series D funding round (Sept 8, 2026) — a company milestone with no pricing impact.
> 🆕 **Z.ai GLM-5.2** — Mistral's **first third-party hosted open model** (Aug 11, 2026): 1M-context, long-context agentic/coding specialist, priced $1.40/$4.40 per MTok with **$0.14/MTok cached input (90% off)**.
> 🆕 **OCR 4.1** supersedes OCR 4.0 as flagship OCR — identical pricing, adds block-level confidence scores.
> 🆕 **Mistral Regional Endpoints reached GA** (EU/US choice, +10% surcharge) and **Mistral Priority Tier entered public preview** (SLA-backed committed service levels).
> 🆕 **Leanstral 1.5** has a published retirement date: September 30, 2026 — now ~2 weeks out; no successor announced yet.
> 🔭 **Discovery-only (not priced, not tracked as full models):** Shieldstral 1.0 (open-weight safety classifier) and Robostral Navigate (embodied-navigation robotics) — both unpriced, self-host only.
> 🔧 **Agent API tool pricing confirmed:** Libraries OCR $3/1K pages, Indexing $1/MTok, Call $0.01/call · Code execution $30/1K calls · Web search $30/1K calls · Image generation $100/1K images · Premium news $50/1K calls · Data capture $0.04/MTok.

---

### 🟣 Tier 2 — OpenRouter Picks (One Best Model Per Provider)

| Provider | Model | Input ($/MTok) | Output ($/MTok) | Context Window |
|---|---|---|---|---|
| **OpenAI open-weight** | gpt-oss-120b | $0.039 | $0.190 | 131K tokens |
| **DeepSeek** | DeepSeek V3.2 | $0.26 | $0.38 | 163K tokens |
| **Qwen (Alibaba)** | Qwen3.6 Plus | Free (preview)* | Free (preview)* | **1M tokens** |
| **Nvidia** | Nemotron 3 Super 120B | $0.10 | $0.50 | 262K tokens |
| **MiniMax** | MiniMax M2.7 | $0.30 | $1.20 | 205K tokens |
| **xAI (Grok)** | Grok 4.1 Fast | $0.20 | $0.50 | **2M tokens** |

> 💡 *Qwen3.6 Plus free preview ended ~April 7, 2026. Paid pricing TBD. Fallback: Qwen3.5 Plus at $0.26/$1.56.
> ℹ️ OpenRouter picks not re-verified in this update cycle (out of scope) — see `openrouter-picks.md` for last confirmed figures.

---

## 📁 Model Card Files

| Provider | Tier | File | Description |
|---|---|---|---|
| Anthropic | 1 | [anthropic.md](./anthropic.md) | Full model cards — re-verified Sept 14, 2026, **zero pricing changes** since Sept 7; only new item is a non-pricing Threat Intelligence report |
| OpenAI | 1 | [openai.md](./openai.md) | Full model cards — 🆕 GPT-Live-1 API pricing ($0.05/min), 🆕 Agents API (public beta, no fee), 🆕 GPT-Image-2.5 Sunburst/Flare (new flagship image tier) + GPT-Image-2 repriced 50% cheaper, 🆕 gpt-rosalind-research, ⚠️ o4-mini & GPT-4.1 nano confirmed deprecated (shutdown Oct 23, 2026) |
| Google Gemini | 1 | [gemini.md](./gemini.md) | Full model cards incl. Gemini 3.5 Flash (new flagship), 3.1 Flash-Lite stable GA, 2.0 Flash deprecation |
| Mistral AI | 1 | [mistral.md](./mistral.md) | Full model cards — re-verified Sept 14, 2026, **zero pricing changes** since Sept 7; only new item is Mistral's €3B Series D funding round |
| OpenRouter Picks | 2 | [openrouter-picks.md](./openrouter-picks.md) | One best-performing model per Tier 2 provider, all via OpenRouter |

---

## ⚠️ Legacy / Deprecated / Retired Models

### 🟠 Anthropic — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| 🔄 Claude Fable 5 | **REPLACED** by Fable 5.1 (Sept 1, 2026) — still fully active | $10.00 | $50.00 | → Claude Fable 5.1 (same price, ~25–45% cheaper via cache-read discount) |
| 🔄 Claude Mythos 5 | **REPLACED** by Mythos 5.1 (Sept 1, 2026) — still active for approved orgs | $10.00 | $50.00 | → Claude Mythos 5.1 |
| ⚠️ Claude Mythos Preview | **LEGACY** · Superseded by Claude Mythos 5 (June 9, 2026), itself now replaced by Mythos 5.1 | $25.00 | $125.00 | → Claude Mythos 5.1 |
| 🔄 Claude Opus 4.8 | **REPLACED** as default by Claude Opus 5 — still fully active, same $5/$25 price, not deprecated | $5.00 | $25.00 | → Claude Opus 5 (same price) |
| 🔄 Claude Sonnet 4.6 | **REPLACED** as default by Claude Sonnet 5 — still fully active, now the *more expensive* option ($3/$15 vs Sonnet 5's $2/$10) | $3.00 | $15.00 | → Claude Sonnet 5 ($2/$10, permanent) |
| ⚠️ Claude Opus 4.7 | **LEGACY** · Fast Mode ❌ REMOVED July 24, 2026 | $5.00 | $25.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude Opus 4.6 | **LEGACY** · Fast Mode ❌ REMOVED June 29, 2026 | $5.00 | $25.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude Sonnet 4.5 | **LEGACY** · 1M beta RETIRED Apr 30, 2026 | $3.00 | $15.00 | → Claude Sonnet 5 or Sonnet 4.6 |
| ⚠️ Claude Opus 4.5 | **LEGACY** | $5.00 | $25.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude Opus 4.1 | **LEGACY** (retired except Bedrock/Google Cloud) | $15.00 | $75.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude Sonnet 4 | **RETIRED ❌ June 15, 2026** on Claude API (still on Bedrock/Google Cloud) | $3.00 | $15.00 | → Claude Sonnet 5 or Sonnet 4.6 |
| ⚠️ Claude Opus 4 | **RETIRED ❌ June 15, 2026** on Claude API (still on Google Cloud) | $15.00 | $75.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude Haiku 3.5 | **RETIRED Feb 19, 2026 ❌ (Claude API)** | $0.80 | $4.00 | → Claude Haiku 4.5 |
| ⚠️ Claude Haiku 3 | **RETIRED Feb 19, 2026 ❌** | $0.25 | $1.25 | → Claude Haiku 4.5 |
| ⚠️ Claude Sonnet 3.7 | **RETIRED Oct 28, 2025 ❌** | $3.00 | $15.00 | → Claude Sonnet 5 or Sonnet 4.6 |
| ⚠️ Claude 3 Opus | **DEPRECATED** Jan 2026 | $15.00 | $75.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude 3.5 Sonnet | **RETIRED Jan 5, 2026** | $3.00 | $15.00 | → Claude Sonnet 5 or Sonnet 4.6 |
| ⚠️ Claude 2.x | **RETIRED** | ~$8.00 | ~$24.00 | → Claude Sonnet 5 or Sonnet 4.6 |

### 🟢 OpenAI — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ **o4-mini** | 🆕 **DEPRECATED — Shuts down October 23, 2026** (confirmed via official Deprecations page) | $1.10 | $4.40 | → **`gpt-5.6-terra`** (official recommendation) |
| ⚠️ **GPT-4.1 nano** | 🆕 **DEPRECATED — Shuts down October 23, 2026** (confirmed via official Deprecations page) | $0.10 | $0.40 | → **`gpt-5.6-luna`** (official recommendation) |
| ⚠️ **o1** | 🆕 **DEPRECATED — Shuts down October 23, 2026** *(migration target corrected — was previously listed as "o3/o3-pro")* | $15.00 | $60.00 | → **`gpt-5.6-sol`** (official recommendation) |
| ⚠️ **o3-mini** | 🆕 **DEPRECATED — Shuts down October 23, 2026** *(newly tracked)* | — | — | → **`gpt-5.6-sol`** |
| ⚠️ **o1-pro** | 🆕 **DEPRECATED — Shuts down October 23, 2026** | — | — | → **`gpt-5.6-sol`** (`reasoning.mode: pro`) |
| ⚠️ **gpt-image-1** | 🆕 **DEPRECATED — Shuts down October 23, 2026** | — | — | → **`gpt-image-2`** |
| ⚠️ **gpt-5.4-cyber** | 🆕 **DEPRECATED — Shuts down October 1, 2026** | — | — | → **`gpt-5.6-cyber`** |
| ⚠️ whisper-1 / gpt-4o-transcribe / gpt-4o-mini-transcribe / gpt-4o-transcribe-diarize | 🆕 **DEPRECATED Aug 26, 2026 — shut down Feb 26, 2027** | varies | varies | → `gpt-live-transcribe` or `gpt-transcribe` |
| ⚠️ gpt-realtime / gpt-audio / gpt-4o-realtime / gpt-realtime-mini / gpt-audio-mini family | 🆕 **DEPRECATED — shut down Jan 20, 2027** | varies | varies | → `gpt-realtime-2.1`, `gpt-realtime-2.1-mini`, or `gpt-audio-1.5` |
| 🔄 GPT-5.6 Sol | **REPLACED** as flagship by GPT-6 Astra (Sept 3, 2026) — still fully active at a **lower, promotional price** | $4.00 *(was $5.00)* | $20.00 *(was $30.00)* | → GPT-6 Astra ($10/$50) for max capability, or stay on Sol at the new lower price |
| 🔄 GPT-5.5 | **REPLACED** as flagship first by GPT-5.6 Sol, now superseded further by GPT-6 Astra — still fully active, unchanged price | $5.00 | $30.00 | → GPT-5.6 Terra ($2.00/$12.00, under half price) or GPT-6 Astra |
| 🔄 GPT-Image-2 | 📉 **Repriced 50% cheaper**; demoted from flagship to value tier by GPT-Image-2.5 Sunburst/Flare — not deprecated | $4.00 *(was $8.00)* | $15.00 *(was $30.00)* | Still active — no migration needed |
| ⚠️ GPT-Realtime-2 | **LEGACY** · Superseded by `gpt-realtime-2.1` — identical pricing | $4.00 (text) / $32.00 (audio) | $24.00 (text) / $64.00 (audio) | → gpt-realtime-2.1 |
| ⚠️ GPT-Realtime-1.5 | **LEGACY** · Superseded first by gpt-realtime-2, now by gpt-realtime-2.1 | $4.00 (text) / $32.00 (audio) | $16.00 (text) / $64.00 (audio) | → gpt-realtime-2.1 |
| ⚠️ GPT-Realtime-Mini | **LEGACY** · Superseded by `gpt-realtime-2.1-mini` — identical pricing | $0.60 (text) / $10.00 (audio) | $2.40 (text) / $20.00 (audio) | → gpt-realtime-2.1-mini |
| ⚠️ GPT-4o mini TTS | **DEPRECATED** · Explicitly labeled "Deprecated" on live OpenAI models page | — | — | → gpt-realtime-2.1 or current TTS models |
| ⚠️ GPT-Image-1.5 | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | $8.00 | $32.00 | → gpt-image-2 |
| ⚠️ GPT-Image-1-mini | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | $2.50 | $8.00 | → gpt-image-2 |
| ⚠️ chatgpt-image-latest | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | — | — | → gpt-image-2 |
| ⚠️ GPT-5.4 Pro | LEGACY · Superseded by GPT-5.5 Pro (same std price, better perf) | $30.00 | $180.00 | → GPT-5.5 Pro |
| ⚠️ GPT-5.3 / Codex | LEGACY · Phasing out (still available as gpt-5.3-codex) | $1.75 | $14.00 | → GPT-5.6 Terra or GPT-5.5 |
| ⚠️ GPT-5.2 | LEGACY · **All GPT-5.2 retired from ChatGPT June 12, 2026 ❌**; `gpt-5.2-chat-latest` shut down Aug 10, 2026 | $1.75 | $14.00 | → GPT-5.4 or GPT-5.6 Terra |
| ⚠️ GPT-5.1 | **RETIRED March 11, 2026** | — | — | → GPT-5.6 family or GPT-6 Astra |
| ⚠️ GPT-4o | LEGACY · dated snapshot `gpt-4o-2024-05-13` shuts down Oct 23, 2026 | $2.50 | $10.00 | → GPT-4.1 or GPT-5.6 Sol |
| ⚠️ GPT-4o mini | LEGACY | $0.15 | $0.60 | → GPT-5.6 Luna ($0.20/$1.20) or GPT-4.1 nano *(also now deprecated)* |
| ⚠️ o1 (legacy alias table entry, see above) | LEGACY | $15.00 | $60.00 | → gpt-5.6-sol |
| ⚠️ GPT-4 Turbo / GPT-4-0613 / gpt-4-1106-preview | **Shuts down October 23, 2026** | — | — | → gpt-5.6-sol |
| ⚠️ GPT-3.5 Turbo (`gpt-3.5-turbo-0125`) | **Shuts down October 23, 2026** | — | — | → gpt-5.6-terra |
| ⚠️ gpt-3.5-turbo-instruct / babbage-002 / davinci-002 / gpt-3.5-turbo-1106 | **Shuts down September 28, 2026** | — | — | → gpt-5.6-terra |

### 🔵 Google Gemini — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ Gemini 2.0 Flash | **DEPRECATED · Shutdown June 1, 2026** | → Gemini 2.5 Flash or Gemini 3.5 Flash |
| ⚠️ Gemini 2.0 Flash-Lite | **DEPRECATED · Shutdown June 1, 2026** | → Gemini 2.5 Flash-Lite |
| ⚠️ Gemini 3 Pro Preview | **RETIRED** March 9, 2026 | → Gemini 3.5 Flash or Gemini 3.1 Pro Preview |
| ⚠️ Gemini 1.5 Pro | LEGACY | → Gemini 2.5 Pro |
| ⚠️ Gemini 1.5 Flash | LEGACY | → Gemini 2.5 Flash |

### 🟡 Mistral AI — Legacy

| Model | Status | Migration Target |
|---|---|---|
| 🔄 OCR 4.0 | **REPLACED** by OCR 4.1 (~August 2026) — identical pricing, 4.1 adds confidence scores | → OCR 4.1 (`mistral-ocr-latest`) |
| ⚠️ OCR 3 v25.12 | **LEGACY** · Superseded by the OCR 4 line; available for existing integrations | → OCR 4.1 ($4/1K pages std, $2/1K batch) |
| 🔄 Leanstral v26.03 | **REPLACED** by Leanstral 1.5 | → Leanstral 1.5 (`leanstral-1-5`) — ⚠️ itself scheduled for retirement Sep 30, 2026 |
| ⚠️ Voxtral Mini 3B v25.07 | **LEGACY** · `voxtral-mini-2507` in legacy table; `voxtral-mini-latest` alias reassigned | → Voxtral Mini Transcribe 2 ($0.003/min) |
| ⚠️ Devstral 2 v25.12 | **LEGACY** · `devstral-2512` in legacy table; `devstral-medium-latest` still active | Use `devstral-medium-latest` |
| ⚠️ Devstral Small 2 v25.12 | **LEGACY** · `labs-devstral-small-2512` in legacy table; `devstral-small-latest` still active | Use `devstral-small-latest` |
| ⚠️ Magistral Medium 1.2 / 1.1 | **LEGACY** · specific versions; `magistral-medium-latest` still active | Use `magistral-medium-latest` |
| ⚠️ Magistral Small 1.2 (v2509) | **LEGACY** · specific version; `magistral-small-latest` still active | → Mistral Small 4 with `reasoning_effort=high` |
| ⚠️ Mistral Medium 3.1 / 3 | **LEGACY** | → Mistral Medium 3.5 or Mistral Large 3 |
| ⚠️ Voxtral Mini Transcribe v25.07 | **LEGACY** · Superseded by v26.02 | → Voxtral Mini Transcribe 2 or Realtime |
| ⚠️ Mistral Small Creative v25.12 | **LEGACY** | → Verify on console.mistral.ai |
| ⚠️ Pixtral Large | **LEGACY** · Deprecated May 2026 | → Mistral Medium 3.5 or Mistral Small 4 |
| ⚠️ Devstral Small 1.1 / 1.0 | LEGACY | → Devstral Small 2 |
| ⚠️ Devstral Medium 1.0 | LEGACY | → Devstral 2 or Medium 3.5 |
| ⚠️ Mistral Small 3.2 / 3.1 / 3.0 | LEGACY | → Mistral Small 4 |
| ⚠️ Mistral Large 2.x | LEGACY | → Mistral Large 3 |
| ⚠️ Codestral 2501 / 24.05 | LEGACY | → Codestral 2508 |
| ⚠️ Mistral Saba, Pixtral 12B, Ministral 3B/8B (24.10), Mistral Nemo 12B, Codestral Mamba, Mathstral, Mistral 7B, Mistral Large/Small/Medium 1.0, original Mixtral 8x7B/8x22B | LEGACY | → Current generation equivalents (see mistral.md) |

---

## 🏷️ Price Change Log

| Date | Provider | Model | Change |
|---|---|---|---|
| 2026-09-14 | OpenAI | **o4-mini, GPT-4.1 nano** | ⚠️ **CONFIRMED DEPRECATED** — Official Deprecations page confirms both shut down **October 23, 2026**. Moved from Active to Legacy. Migrate to `gpt-5.6-terra` (o4-mini) and `gpt-5.6-luna` (GPT-4.1 nano). `o1`, `o3-mini`, `o1-pro`, and `gpt-image-1` are also on the same Oct 23, 2026 shutdown list; `gpt-5.4-cyber` shuts down Oct 1, 2026. |
| 2026-09-14 | OpenAI | **GPT-Live-1** | 🆕 **NOW PRICED IN THE API** — $0.05/minute for the voice layer, launched Sept 10, 2026. Previously ChatGPT-only and unpriced. |
| 2026-09-14 | OpenAI | **Agents API** | 🆕 **NEW PRODUCT** — Public beta launched Sept 10, 2026; managed Codex-harness agent runtime with no additional fees beyond standard token/tool rates. |
| 2026-09-14 | OpenAI | **GPT-Image-2.5 Sunburst / Flare** | 🆕 **NEW FLAGSHIP IMAGE MODELS** — $8/$2 cached/$30 image, $5/$1.25 cached text per MTok — the price GPT-Image-2 used to carry. |
| 2026-09-14 | OpenAI | **GPT-Image-2** | 📉 **REPRICED 50% CHEAPER** — Image $8→$4, cached $2→$1, output $30→$15 per MTok (text similarly halved); demoted from flagship to value tier, not deprecated. |
| 2026-09-14 | OpenAI | **gpt-rosalind-research** | 🆕 **PRICING PUBLISHED** — $5.00/$0.50 cached/$25.00 per MTok; billing begins October 5, 2026. Life Sciences trusted-access model. |
| 2026-09-14 | Anthropic | **All active + legacy models** | ✅ RE-VERIFIED — Zero price changes detected against the live pricing pages since Sept 7. |
| 2026-09-14 | Mistral | **All active + legacy models** | ✅ RE-VERIFIED — Zero price changes detected against the live pricing page since Sept 7. Mistral raised a €3B Series D funding round (Sept 8, 2026) — no pricing impact. |
| 2026-09-07 | OpenAI | **GPT-6 Astra** | 🆕 **NEW FLAGSHIP MODEL** — Launched September 3, 2026 at $10.00/$50.00 per MTok (short context), OpenAI's first model to reach the "Critical" cybersecurity capability threshold under its Preparedness Framework. 1.05M context, 128K max output, Apr 30 2026 knowledge cutoff. Replaces GPT-5.6 Sol as OpenAI's recommended flagship. New capabilities: async tool calling, mid-turn steering, mid-conversation `configuration_update` reasoning changes. Development delayed following a July 2026 Hugging Face security incident involving unrelated OpenAI research agents. |
| 2026-09-07 | OpenAI | **GPT-5.6 Sol** | 📉 **PROMOTIONAL PRICE CUT** — $5.00/$30.00 → **$4.00/$20.00** per MTok (short context), as Sol steps down from flagship status in favor of GPT-6 Astra. Promotional pricing available at least through November 21, 2026. Long context: $10.00/$45.00 → $8.00/$30.00. |
| 2026-09-07 | OpenAI | **gpt-5.6-cyber** | 🆕 **PRICING PUBLISHED** — $12.50/$1.25 cached/$75.00 per MTok (short context only), previously unpriced. Newly documented alongside `gpt-daybreak-blue-latest`/`gpt-daybreak-red-latest` aliases (Daybreak cybersecurity program). |
| 2026-09-07 | Anthropic | **Claude Fable 5.1 / Mythos 5.1** | 🆕 **NEW MODELS** — Launched September 1, 2026, replacing Fable 5/Mythos 5 as Anthropic's most advanced models. Same $10.00/$50.00 base price, but cache-read pricing cut 75% (from $1.00/MTok to $0.25/MTok) — an estimated 25% cheaper for typical workloads, up to 45% cheaper for highly agentic workloads. Fable 5.1 is GA; Mythos 5.1 is trusted-access only. |
| 2026-09-07 | Anthropic | **Claude Sonnet 5** | ✅ **PRICING CONFIRMED PERMANENT** — The $2.00/$10.00 introductory rate is now permanent; the scheduled September 1, 2026 increase to $3.00/$15.00 will not occur. |
| 2026-09-07 | Anthropic | **Tools** | 🆕 **NEW: Browser use tool** (`browser_toolset_20260801`, ~6,600 tokens overhead) and updated Computer use toolset (`computer_toolset_20260801`, ~4,500 tokens) newly documented on the live pricing page. |
| 2026-09-07 | Mistral | **Z.ai GLM-5.2** | 🆕 **NEW MODEL** — Mistral's first third-party hosted open model (announced Aug 11, 2026), $1.40/$0.14 cached/$4.40 per MTok, 1M context, long-context agentic/coding specialist. First model on Mistral's platform with a cached-input discount. |
| 2026-09-07 | Mistral | **OCR 4.1** | 🆕 **NEW MODEL** — Supersedes OCR 4.0 as flagship OCR; identical pricing ($4/$2/$5 per 1K pages); adds block-level confidence scores. OCR 4.0 moved to legacy. |
| 2026-09-07 | Mistral | **Regional Endpoints / Priority Tier** | 🆕 Regional Endpoints reached **General Availability** (EU/US choice, +10% surcharge); Mistral Priority Tier entered **public preview** (SLA-backed committed service levels). |
| 2026-08-10 | OpenAI | **All active models, Tools, Realtime, Image, Video, Transcription, Deep Research, Computer Use, Codex** | ✅ RE-VERIFIED — Zero API price changes detected since the Aug 3, 2026 refresh. |
| 2026-08-10 | OpenAI | **ChatGPT consumer product update (non-pricing)** | 🆕 Aug 6, 2026: GPT-5.6 Luna became the default model for ChatGPT Free/Go users with unlimited text chats. No API pricing changed. |
| 2026-08-10 | Anthropic | **All active + legacy models** | ✅ RE-VERIFIED — Zero price changes detected against the live pricing page. |
| 2026-08-10 | Mistral | **Shieldstral 1.0** | 🆕 **NEW DISCOVERY (not priced)** — Open-weight (Apache 2.0) policy-adaptive multimodal safety classifier, no hosted API pricing. |
| 2026-08-03 | OpenAI | **GPT-5.6 Terra / Luna** | 📉 **PRICE CUTS** — Terra: $2.50/$15.00 → $2.00/$12.00. Luna: $1.00/$6.00 → $0.20/$1.20 (~80% cut). |
| 2026-08-03 | Anthropic | **Claude Opus 4.7 Fast Mode** | ✅ **REMOVAL CONFIRMED** — `speed: "fast"` requests against Opus 4.7 now return an error. |
| 2026-07-27 | Anthropic | **Claude Opus 5** | 🆕 **NEW MODEL** — Launched July 24, 2026 at $5.00/$25.00, replacing Opus 4.8 as Max default/strongest-on-Pro. |
| 2026-07-14 | OpenAI | **GPT-5.6 (Sol/Terra/Luna)** | 🆕 **REACHED GENERAL AVAILABILITY — July 9, 2026.** |
| 2026-06-30 | Anthropic | **Claude Sonnet 5** | 🆕 NEW MODEL — Launched June 30, 2026, introductory pricing $2/$10 (later made permanent Sept 1, 2026). |
| 2026-06-29 | Mistral | **OCR 4** | 🆕 NEW MODEL — Launched June 23, 2026 (superseded by OCR 4.1 in September). |
| 2026-04-29 | Mistral | **Mistral Medium 3.5** | 🆕 LAUNCHED — $1.50/$7.50. 256K context. 128B dense. |

> ℹ️ For the full historical change log (entries prior to August 10, 2026), see the git history of this file or the individual provider model-card files, which retain complete per-refresh detail.

---

## ℹ️ Notes
- All prices are in **USD** per million tokens (MTok) unless stated otherwise.
- **Batch API discounts (50%)** apply at Anthropic, OpenAI, Mistral, and Google Gemini.
- **Prompt/context caching** discounts apply where noted. Mistral's own models do **not** offer prompt caching (Z.ai GLM-5.2, hosted on Mistral's platform, is the first exception). OpenAI's GPT-5.6/GPT-6 Astra generation uses a cache-write-at-1.25× model. Anthropic's Fable 5.1/Mythos 5.1 cut cache-read pricing to 0.025× (from 0.1×) — the cheapest cache reads of any tracked provider.
- Enterprise/volume pricing available from all providers on request.
- **OpenAI GPT-6 Astra, GPT-5.6, GPT-5.5, and GPT-5.4** have short-context (<~270–272K) and long-context (>~270–272K) pricing tiers.
- **OpenAI service tiers:** Priority/Fast mode → Standard → Batch/Flex (50% off).
- **Google Gemini Pro** models double input cost for prompts >200K tokens.
- **Mistral** processes API data in the EU by default, with **Regional Endpoints now GA** for EU/US choice (+10% surcharge), and a new SLA-backed **Priority Tier** in public preview.
- **Anthropic** offers US-only inference at 1.1× pricing via `inference_geo: "us"` parameter.
- **Tool/agent pricing is additive:** Anthropic Web Search ($10/1K searches), Code Execution, Computer/Browser use tools, and Claude Managed Agents ($0.08/session-hour); OpenAI Web Search ($10–25/1K calls), Computer Use, Containers, File Search, GPT-Live-1 sessions ($0.05/min), and the Agents API (no extra fee); Mistral Agent API (Web Search/Code Execution at $30/1K calls, Libraries, Image Generation) all bill on top of standard per-model token rates.
- ⚠️ Models marked **RETIRED** return API errors. **DEPRECATED** = end-of-life published. **LEGACY** = still accessible but in provider's legacy section. **SUSPENDED** = access halted by external directive. **🔄 REPLACED** = superseded by a newer default/recommended model but still active and not deprecated. **🔓 RESTORED** = a previously suspended model has regained access. **📉 PRICE CUT** = confirmed price decrease on an active model.
- 🆕 **Unpriced/discovery-only items** (e.g., Mistral's Shieldstral 1.0 and Robostral Navigate) are noted for awareness but are **not** given a full tracked model card until the provider publishes official pricing/specs.
- ⚠️ **September 14, 2026:** Confirmed via OpenAI's official Deprecations page that **`o4-mini` and `GPT-4.1 nano` are deprecated and shut down October 23, 2026** — both moved from Active to Legacy in this refresh, alongside `o1`, `o3-mini`, `o1-pro`, and `gpt-image-1` (same shutdown date) and `gpt-5.4-cyber` (shuts down Oct 1, 2026).
- 🆕 **September 10, 2026:** OpenAI launched **GPT-Live-1 in the API** ($0.05/min) and the new **Agents API** (public beta, no added fees).
- 🆕 **September 3, 2026:** OpenAI launched **GPT-6 Astra**, its new flagship model and first to reach "Critical" cybersecurity capability status; GPT-5.6 Sol was demoted to a promotional $4.00/$20.00 price point.
- 🆕 **September 1, 2026:** Anthropic launched **Claude Fable 5.1 and Mythos 5.1**, cutting cache-read pricing 75% versus Fable 5/Mythos 5; **Claude Sonnet 5's $2/$10 pricing was confirmed permanent.**
- 🆕 **August 11, 2026:** Mistral began hosting **Z.ai's GLM-5.2**, its first third-party open model, and announced GA Regional Endpoints plus a new Priority Tier in public preview.
- 📝 **September 14, 2026:** This refresh independently re-verified Anthropic, OpenAI, and Mistral pricing against each provider's live pricing/docs pages, plus each provider's news feed and (for OpenAI) the official Deprecations page. **Key changes:** OpenAI's GPT-Live-1 launched in the API at $0.05/min; OpenAI's new Agents API launched in public beta with no added fees; GPT-Image-2.5 Sunburst/Flare became the new flagship image models while GPT-Image-2 was repriced 50% cheaper; `gpt-rosalind-research` (Life Sciences) gained published pricing; and `o4-mini`/`GPT-4.1 nano` were confirmed deprecated (shutdown Oct 23, 2026) and moved to Legacy. GPT-6 Astra and the full GPT-5.6 family were re-verified unchanged. Anthropic and Mistral pricing were both independently re-verified with **zero changes** — Anthropic's only news was a non-pricing Threat Intelligence report, and Mistral's was a €3B Series D funding announcement with no pricing impact. Google Gemini and OpenRouter Picks tables reflect the last confirmed figures from a prior refresh and were not re-verified this cycle.
