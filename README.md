# 🤖 LLM Pricing Tracker

Up-to-date pricing and specifications for large language models from **Anthropic**, **OpenAI**, **Google Gemini**, **Mistral AI**, and top **OpenRouter picks**.

> **Last updated:** 2026-10-05 (refresh #37)
> **Sources:** Official provider pricing pages — scraped/verified on date above.

---

## 📋 Quick-Reference Index — Active Models

### 🟠 Tier 1 — Anthropic Claude

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Max Output | Availability |
|---|---|---|---|---|---|
| 🆕 **Claude Opus 5.5** *(Leading Model — Released Sept 22, 2026)* | $4.00 | $20.00 | **1M tokens** | 128k | Claude API, Claude.ai, Claude Code, AWS, Google Cloud, Azure |
| 🆕 **Claude Sonnet 5.5** *(Released Sept 28, 2026 — Best Speed/Intelligence Combo)* | $2.00 | $10.00 | **1M tokens** | 128k | Claude API, Claude.ai, Claude Code, Claude Cowork, AWS, Google Cloud, MS Foundry |
| 🆕 **Claude Fable 5.1** *(Released Sept 1, 2026 — Most Advanced Model)* | $10.00 | $50.00 | **1M tokens** | 128k | Claude API, Claude.ai, Claude Code, Claude Cowork, AWS, Google Cloud, Azure |
| 🔒 **Claude Mythos 5.1** *(Trusted Access — Sept 1, 2026)* | $10.00 | $50.00 | **1M tokens** | 128k | CVP / LSVP trusted-access programs |
| **Claude Opus 5** *(🔄 replaced by Opus 5.5 — still active)* | $5.00 | $25.00 | **1M tokens** | 128k sync / 300k Batch | API, AWS Bedrock, Claude Platform on AWS, Google Cloud, MS Foundry |
| **Claude Opus 4.8** *(🔄 replaced by Opus 5 — still active)* | $5.00 | $25.00 | **1M tokens** | 128k sync / 300k Batch | API, AWS Bedrock (Messages API), Vertex AI, MS Foundry (200k ctx) |
| **Claude Sonnet 5** *(🔄 replaced by Sonnet 5.5 — still active)* | $2.00 | $10.00 | **1M tokens** | 128k sync / 300k Batch | API, Claude.ai, Claude Code, AWS Bedrock, Google Cloud, MS Foundry |
| **Claude Sonnet 4.6** *(🔄 replaced by Sonnet 5 as default)* | $3.00 | $15.00 | **1M tokens** | 64k sync / 300k Batch | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Haiku 4.5** | $1.00 | $5.00 | 200K tokens | 64k | API, AWS Bedrock (all regions), Vertex AI, MS Foundry |

> 💡 Batch API: 50% off · Prompt caching: up to 90% off (up to **97.5% off** cache reads on Fable 5.1/Mythos 5.1, **95% off** on Opus 5.5; Sonnet 5.5 stays on the standard 0.1× rate)
> 🆕 **September 28, 2026 — Claude Sonnet 5.5 launched**, the second model in the "Claude 5.5" family. Same $2/$10 price as Sonnet 5, but runs 30%+ faster and scores 70.6% on Terminal-Bench 4.0 (vs. Sonnet 5's 10.3%, Opus 5.5's 66.4%). First Sonnet-tier model with real-time cybersecurity safeguards. Sonnet 5 is now 🔄 REPLACED (still active).
> 🆕 **September 30, 2026 — Claude Sonnet 4.5 deprecated**, with a tentative retirement date of **November 30, 2026** on the Claude API; migrate to Sonnet 5.5.
> 🔜 **Claude Haiku 5.5 remains unreleased** as of October 5 — still "in the coming weeks," with Haiku 4.5's own retirement floor (not sooner than Oct 15, 2026) approaching.
> 🆕 **September 22, 2026 — Claude Opus 5.5 launched**, the first model in Anthropic's new "Claude 5.5" family. Replaces Claude Opus 5 as Anthropic's leading model at **$4.00/$20.00** per MTok (20% cheaper) with **$0.20/MTok** cache reads (60% cheaper than Opus 5's $0.50). Anthropic estimates ~40% lower cost than Opus 5 on typical workloads.
> 🆕 Claude Fable 5.1 and Mythos 5.1 launched Sept 1, 2026 — same $10/$50 base price as Fable 5/Mythos 5, but cache-read pricing cut 75% (to $0.25/MTok), cutting typical workload costs by ~25% and highly agentic workload costs by up to ~45%.

---

### 🟢 Tier 1 — OpenAI (Proprietary)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|---|
| 🆕 **GPT-6 Astra** *(Flagship — Released Sept 3, 2026)* | $10.00 / $20.00* | $1.00 / $2.00* | $50.00 / $75.00* | **1.05M tokens** | ChatGPT, API, Azure/Foundry, AWS Bedrock |
| 🆕 **GPT-6.1 Sol** *(Released Sept 29, 2026 at DevDay — replaces GPT-6 Sol after 7 days)* | $2.00 / $4.00* | $0.10 / $0.20* | $10.00 / $15.00* | **1.05M tokens** | ChatGPT Work, Codex, API, GitHub Copilot |
| 🆕 **GPT-6 Luna** *(Released Sept 22, 2026 — 50% cheaper than GPT-5.6 Luna)* | $0.10 / $0.20* | $0.01 / $0.02* | $0.50 / $0.75* | **1.05M tokens** | ChatGPT Work/Codex/Free-Go desktop, API |
| **GPT-5.6 Terra** *(✅ confirmed unchanged — no GPT-6 equivalent yet)* | $2.00 / $4.00* | $0.20 / $0.40* | $12.00 / $18.00* | **~1.05M tokens** | ChatGPT, Codex, API — self-serve |
| 📉 **GPT-5.6 Sol** *(🔄 replaced by GPT-6.1 Sol — promo pricing confirmed through Nov 21, 2026)* | $4.00 / $8.00* | $0.40 / $0.80* | $20.00 / $30.00* | **~1.05M tokens** | ChatGPT, Codex, API — self-serve |
| **GPT-5.6 Luna** *(🔄 replaced by GPT-6 Luna — still active)* | $0.20 / $0.40* | $0.02 / $0.04* | $1.20 / $1.80* | **~1.05M tokens** | ChatGPT, Codex, API — self-serve |
| **GPT-5.6 Cyber** *(Daybreak program)* | $12.50 | $1.25 | $75.00 | ~1.05M tokens | Vetted access (Daybreak) |
| 🆕 **GPT-Rosalind (Research)** *(Life Sciences, trusted access — billing now live since Oct 5, 2026)* | $5.00 | $0.50 | $25.00 | — | Trusted-access program only |
| ⚠️ **GPT-5.5** *(API active — retires from ChatGPT/Codex Oct 14, 2026)* | $5.00 / $10.00* | $0.50 / $1.00* | $30.00 / $45.00* | **1M tokens** | API (unaffected) · ChatGPT/Codex until Oct 14, 2026 |
| **GPT-5.5 Pro** | $30.00 / $60.00* | — | $180.00 / $270.00* | 1M tokens | API |
| GPT-5.4 *(prev flagship)* | $2.50 / $5.00† | $0.25 / $0.50† | $15.00 / $22.50† | 1M tokens | API |
| GPT-5.4 Pro | $30.00 / $60.00* | — | $180.00 / $270.00* | 1.05M tokens | API |
| **GPT-5.4 mini** | $0.75 | $0.075 | $4.50 | 400K tokens | API |
| ⚠️ **GPT-5.4 nano** *(deprecated Oct 1, 2026 — shuts down Apr 1, 2027)* | $0.20 | $0.020 | $1.25 | 400K tokens | API |
| GPT-4.1 | $2.00 | $0.50 | $8.00 | 1.04M tokens | API |
| **GPT-4.1 mini** | $0.40 | $0.10 | $1.60 | 1.00M tokens | API |
| ⚠️ o3 *(reasoning — dated snapshot shuts down Dec 11, 2026)* | $2.00 | $0.50 | $8.00 | 200K tokens | API |
| ⚠️ o3-pro *(reasoning — dated snapshot shuts down Dec 11, 2026)* | $20.00 | — | $80.00 | 200K tokens | API |

> ⚠️ **`o4-mini` and `GPT-4.1 nano` are DEPRECATED** — both **shut down October 23, 2026**. See Legacy section for migration targets.
> ❌ **The Videos API, `sora-2`, and `sora-2-pro` (+ dated snapshots) SHUT DOWN September 24, 2026** — no replacement model listed. See Legacy section.
> ✅ **`GPT-6 Cyber` did NOT appear at DevDay (Sept 29)** despite pre-event reporting — OpenAI's official DevDay recap makes no mention of it. Remains unconfirmed/discovery-only; `gpt-5.6-cyber` is still OpenAI's most advanced priced cyber model.
> 🆕 **September 29, 2026 — OpenAI DevDay 2026.** Launched **GPT-6.1 Sol** (replacing GPT-6 Sol on the pricing/model catalog after just 7 days — same $2/$10 price, cached input cut from $0.20 to $0.10/MTok), a priced **Ultrafast** speed tier for GPT-6 Astra (6× standard: $60/$300 short ctx), **Dots** (always-on agents, Pro/Business Premium), a new **Pro 500** ChatGPT plan (25× Plus allowance + Ultrafast), and **OpenAI Private Intelligence** (Zero Data Retention with Private Safety Processing).
> 🆕 **October 1, 2026 — new deprecation wave:** `gpt-5.3-codex`, `gpt-5.1`, `gpt-5.4-nano` shut down **April 1, 2027** → migrate to GPT-6.1 Sol / GPT-6 Luna. Legacy TTS (`tts-1`, `tts-1-hd`, old `gpt-4o-mini-tts` snapshots) shut down **January 6, 2027** → `gpt-realtime-2.1-mini`.
> 🆕 **September 22, 2026 — GPT-6 Sol and GPT-6 Luna launched**, expanding the GPT-6 family alongside Astra, both **50% cheaper** than the GPT-5.6 promotional rates they replaced. **There is no GPT-6 Terra** — GPT-5.6 Terra ($2.00/$12.00) remains OpenAI's un-replaced mid-tier "Default" model.
> 💡 Batch/Flex API: 50% off all models · Cached inputs: 50–95% off · Regional processing: +10% on GPT-6/5.6/5.5/5.4 family
> 🆕 **GPT-6 Astra launched September 3, 2026** — OpenAI's new flagship, "our most intelligent model yet," and OpenAI's first model to reach the **"Critical"** cybersecurity capability threshold under its Preparedness Framework. 1.05M context, 128K max output, Apr 30 2026 knowledge cutoff.
> *GPT-6 / GPT-5.6 / GPT-5.5 / GPT-5.5 Pro / GPT-5.4 Pro long-context pricing (>~270–272K tokens): standard × 2 input / × 1.5 output (× 2 for Pro models)
> †GPT-5.4 tiered pricing: short ctx (<~270K) / long ctx (>~270K)
> 🔧 **Tools pricing confirmed unchanged:** Web Search $10/1K calls (all models + reasoning-preview) or $25/1K calls (non-reasoning preview, free content tokens) · Computer Use (`computer-use-preview`) $1.50/$6.00 · Containers $0.03–$1.92 per 20-min session · File Search $0.10/GB-day storage + $2.50/1K tool calls · GPT-Live-1 sessions $0.05/min · Agents API no extra fee (now supports computer use).
> ✅ Re-verified October 5, 2026 against the live `developers.openai.com/api/docs/pricing`, `developers.openai.com/api/docs/models`, `developers.openai.com/api/docs/models/gpt-5.6-terra`, `developers.openai.com/api/docs/deprecations`, and `openai.com/index/devday-2026-recap/`.

**Multimodal / Specialized:**

| Model | Pricing |
|---|---|
| GPT-Live-1 | $0.05/minute (API) — backend model/tools billed separately |
| GPT-Live-1 mini | Referenced in ChatGPT; no confirmed standalone API price yet |
| gpt-realtime-2.1 | Audio $32/$64 · Text $4/$24 · Image $5 input/$0.50 cached (per MTok) |
| gpt-realtime-2.1-mini | Audio $10/$20 · Text $0.60/$2.40 · Image $0.80 input/$0.08 cached (per MTok) |
| gpt-realtime-translate | $0.034 / minute |
| gpt-realtime-whisper | $0.017 / minute — new streaming STT model, distinct from legacy `whisper-1` |
| gpt-live-transcribe | $0.017 / minute |
| gpt-transcribe | $0.0045 / minute |
| ⚠️ gpt-4o-transcribe / gpt-4o-mini-transcribe / whisper-1 | DEPRECATED Aug 26, 2026 — shut down Feb 26, 2027 → gpt-live-transcribe or gpt-transcribe |
| gpt-image-2.5-sunburst / gpt-image-2.5-flare | **Flagship image models** — Image $8 input/$2 cached/$30 output · Text $5 input/$1.25 cached (per MTok) |
| gpt-image-2 | Value tier — Image $4 input/$1 cached/$15 output · Text $2.50 input/$0.625 cached (per MTok) |
| ⚠️ gpt-image-1.5 | DEPRECATED — shutdown Dec 1, 2026 → migrate to gpt-image-2 |
| ⚠️ gpt-image-1-mini | DEPRECATED — shutdown Dec 1, 2026 → migrate to gpt-image-2 |
| ⚠️ gpt-image-1 | DEPRECATED — shutdown **Oct 23, 2026** → migrate to gpt-image-2 |
| ⚠️ tts-1 / tts-1-hd / old gpt-4o-mini-tts snapshots | 🆕 DEPRECATED Oct 1, 2026 — shuts down **Jan 6, 2027** → gpt-realtime-2.1-mini |
| ⚠️ **sora-2 / sora-2-pro / Videos API** | **SHUT DOWN September 24, 2026 — no replacement listed** |
| o3-deep-research | $5.00 input / $20.00 output per MTok |
| o4-mini-deep-research | $1.00 input / $4.00 output per MTok |
| **computer-use-preview** | $1.50 input / $6.00 output per MTok |
| **gpt-rosalind-research** | $5.00 input / $0.50 cached / $25.00 output per MTok — billing now live (Oct 5, 2026) |

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

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|---|
| 🆕 **Z.ai GLM 5.3** *(now GA — sole active third-party model)* | $1.40 | $0.14 | $4.40 | **1M tokens** | Mistral AI Studio |
| **Mistral Medium 3.5** *(Apr 29, 2026 — Flagship)* | $1.50 | $0.15 | $7.50 | 256K tokens | API |
| **Mistral Large 3 (2512)** | $0.50 | $0.05 | $1.50 | 256K tokens | API |
| **Mistral Small 4** | $0.15 | $0.015 | $0.60 | **256K tokens** | API |
| Codestral 2508 | $0.30 | $0.03 | $0.90 | 256K tokens | API |
| Voxtral Small 24B | $0.004/min (audio) | — | $0.40 | 128K tokens | API |
| **Voxtral Mini Transcribe 2** (Premier) | $0.003/min | $0.0003/min | — | — | API |
| **Voxtral Mini Transcribe Realtime** (Open) | $0.006/min | — | — | — | API |
| Voxtral TTS | $0.016/1K chars | — | — | — | API |
| **OCR 4.1** *(flagship OCR)* | $4.00/1K pages | $0.40/1K pages | $2.00/1K pages (Batch) · $5.00/1K pages (DocAI) | — | API |
| **Classifier API 3B** | $0.10 + $1/MTok training | — | $0.10 | — | API |
| **Classifier API 8B** | $0.04 + $1/MTok training | — | $0.04 | — | API |
| **Codestral Embed** *(Premier)* | $0.15 (input only) | $0.015 | — | — | API |
| **Mistral Embed** | $0.10 (input only) | — | — | — | API |
| **Mistral Moderation 2** | Free | Free | Free | — | API |
| Ministral 3 14B | $0.20 | $0.02 | $0.20 | 256K tokens | API |
| Ministral 3 8B | $0.15 | $0.015 | $0.15 | 256K tokens | API |
| Ministral 3 3B | $0.10 | $0.01 | $0.10 | 256K tokens | API |

> ⚠️ **Z.ai GLM 5.2 is now DEPRECATED (Oct 1, 2026), retiring October 31, 2026** — removed from the live pricing page; GLM 5.3 is now the platform's sole active third-party model at the same price.
> ⚠️ **Mixtral 8×7B and Mixtral 8×22B are now confirmed RETIRED** — both appear in Mistral's official "Deprecated & retired models" table this refresh, correcting prior tracking that listed them as still Active on the API. See Legacy section.
> ⚠️ **OCR 4.0 is now DEPRECATED** — fully superseded by OCR 4.1 at the same price; OCR 3 remains separately available for existing integrations.
> ✅ **Leanstral 1.5's September 30, 2026 retirement has now been confirmed to have occurred** — no successor announced yet.
> ⚠️ **Devstral 2, Devstral Small 2, and the entire Magistral family (Medium/Small) are RETIRED from the hosted API (July 31, 2026)**. Migrate to Mistral Medium 3.5 (Devstral/Magistral Medium use cases) or Mistral Small 4 with `reasoning_effort=high` (Devstral Small/Magistral Small use cases). See Legacy section below.
> ⚠️ **Mistral Medium 3 and Medium 3.1 are RETIRED (August 31, 2026)**; **Mistral Small 3.2** and **Mistral NeMo 12B** are RETIRED (July 31, 2026).
> 💡 Batch API: 50% off · EU/US Regional Endpoints (GA, +10% surcharge) · Mistral Priority Tier (public preview, SLA-backed)
> 💡 Cached input published for Mistral's own native models (90% off) — Large 3, Medium 3.5, Small 4, Ministral tiers, Codestral, Codestral Embed, OCR 4.1, Voxtral Mini Transcribe 2.
> ✅ **October 5, 2026 refresh:** Re-fetched the live `docs.mistral.ai/inference/pricing` and `docs.mistral.ai/models` pages directly. All active prices confirmed unchanged. Three status changes found: GLM 5.2 deprecated, Mixtral 8×7B/8×22B confirmed retired, OCR 4.0 confirmed deprecated.

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
| Anthropic | 1 | [anthropic.md](./anthropic.md) | Full model cards — 🆕 Claude Opus 5.5 launched (Sept 22), replacing Opus 5 as leading model at $4/$20 (20% cheaper); re-verified Sept 28 with zero further changes; Sonnet 5.5/Haiku 5.5 still unreleased |
| OpenAI | 1 | [openai.md](./openai.md) | Full model cards — 🆕 GPT-6 Sol & GPT-6 Luna launched (Sept 22), each 50% cheaper than the GPT-5.6 tier replaced; ❌ Sora-2/Sora-2-Pro/Videos API shutdown (Sept 24, 2026) now in effect; ✅ GPT-5.6 Terra confirmed unchanged; discovery-only unpriced GPT-6 Cyber report |
| Google Gemini | 1 | [gemini.md](./gemini.md) | Full model cards incl. Gemini 3.5 Flash (new flagship), 3.1 Flash-Lite stable GA, 2.0 Flash deprecation |
| Mistral AI | 1 | [mistral.md](./mistral.md) | Full model cards — re-verified Sept 28, 2026, **zero pricing changes** since Sept 23; Leanstral 1.5 retirement 2 days out |
| OpenRouter Picks | 2 | [openrouter-picks.md](./openrouter-picks.md) | One best-performing model per Tier 2 provider, all via OpenRouter |

---

## ⚠️ Legacy / Deprecated / Retired Models

### 🟠 Anthropic — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| 🔄 Claude Opus 5 | **REPLACED** as leading model by Claude Opus 5.5 (Sept 22, 2026) — still fully active, same-tier fallback target | $5.00 | $25.00 | → Claude Opus 5.5 ($4/$20, 20% cheaper) |
| 🔄 Claude Fable 5 | **REPLACED** by Fable 5.1 (Sept 1, 2026) — still fully active | $10.00 | $50.00 | → Claude Fable 5.1 (same price, ~25–45% cheaper via cache-read discount) |
| 🔄 Claude Mythos 5 | **REPLACED** by Mythos 5.1 (Sept 1, 2026) — still active for approved orgs | $10.00 | $50.00 | → Claude Mythos 5.1 |
| ⚠️ Claude Mythos Preview | **LEGACY** · Superseded by Claude Mythos 5 (June 9, 2026), itself now replaced by Mythos 5.1 | $25.00 | $125.00 | → Claude Mythos 5.1 |
| 🔄 Claude Opus 4.8 | **REPLACED** as default by Claude Opus 5 — still fully active, same $5/$25 price, not deprecated | $5.00 | $25.00 | → Claude Opus 5 or Opus 5.5 |
| 🔄 Claude Sonnet 5 | **REPLACED** by Claude Sonnet 5.5 (Sept 28, 2026) — still fully active, identical $2/$10 price | $2.00 | $10.00 | → Claude Sonnet 5.5 (same price, 30%+ faster) |
| 🔄 Claude Sonnet 4.6 | **REPLACED** as default by Claude Sonnet 5 — still fully active, now the *more expensive* option ($3/$15 vs Sonnet 5's $2/$10) | $3.00 | $15.00 | → Claude Sonnet 5.5 ($2/$10) |
| ⚠️ Claude Opus 4.7 | **LEGACY** · Fast Mode ❌ REMOVED July 24, 2026 | $5.00 | $25.00 | → Claude Opus 5.5, 5, or 4.8 |
| ⚠️ Claude Opus 4.6 | **LEGACY** · Fast Mode ❌ REMOVED June 29, 2026 | $5.00 | $25.00 | → Claude Opus 5.5, 5, or 4.8 |
| 🆕 ⚠️ Claude Sonnet 4.5 | **DEPRECATED Sept 30, 2026 — retires November 30, 2026** on the Claude API | $3.00 | $15.00 | → Claude Sonnet 5.5 |
| ⚠️ Claude Opus 4.5 | **LEGACY** | $5.00 | $25.00 | → Claude Opus 5.5, 5, or 4.8 |
| ⚠️ Claude Opus 4.1 | **RETIRED** August 5, 2026 (Claude API — retired except Bedrock/Google Cloud) | $15.00 | $75.00 | → Claude Opus 5.5, 5, or 4.8 |
| ⚠️ Claude Sonnet 4 | **RETIRED ❌ June 15, 2026** on Claude API (still on Bedrock/Google Cloud) | $3.00 | $15.00 | → Claude Sonnet 5 or Sonnet 4.6 |
| ⚠️ Claude Opus 4 | **RETIRED ❌ June 15, 2026** on Claude API (still on Google Cloud) | $15.00 | $75.00 | → Claude Opus 5.5, 5, or 4.8 |
| ⚠️ Claude Haiku 3.5 | **RETIRED Feb 19, 2026 ❌ (Claude API)** | $0.80 | $4.00 | → Claude Haiku 4.5 |
| ⚠️ Claude Haiku 3 | **RETIRED Feb 19, 2026 ❌** | $0.25 | $1.25 | → Claude Haiku 4.5 |
| ⚠️ Claude Sonnet 3.7 | **RETIRED Oct 28, 2025 ❌** | $3.00 | $15.00 | → Claude Sonnet 5 or Sonnet 4.6 |
| ⚠️ Claude 3 Opus | **RETIRED** January 2026 | $15.00 | $75.00 | → Claude Opus 5.5, 5, or 4.8 |
| ⚠️ Claude 3.5 Sonnet | **RETIRED** February 2026 | $3.00 | $15.00 | → Claude Sonnet 5 or Sonnet 4.6 |
| ⚠️ Claude 3 Haiku | **RETIRED** April 2026 | — | — | → Claude Haiku 4.5 |
| ⚠️ Claude 2.x | **RETIRED** | ~$8.00 | ~$24.00 | → Claude Sonnet 5 or Sonnet 4.6 |

### 🟢 OpenAI — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ❌ **Videos API, sora-2, sora-2-pro** | ❌ **SHUT DOWN September 24, 2026 (date passed) — no replacement listed** | $0.10–$0.70/sec | — | None announced |
| 🆕 🔄 GPT-6 Sol | **REPLACED** by GPT-6.1 Sol (Sept 29, 2026, DevDay) — removed from pricing/model catalog after just 7 days | $2.00 | $10.00 | → GPT-6.1 Sol (same price, cheaper cached input) |
| 🔄 GPT-5.6 Sol | **REPLACED** by GPT-6.1 Sol — still fully active; promo pricing confirmed through Nov 21, 2026; also backs `gpt-daybreak-blue-latest` and `gpt-5.6-cyber` pricing | $4.00 | $20.00 | → GPT-6.1 Sol ($2/$10, 50% cheaper) |
| 🔄 GPT-5.6 Luna | **REPLACED** by GPT-6 Luna (Sept 22, 2026) — still fully active | $0.20 | $1.20 | → GPT-6 Luna ($0.10/$0.50, ~50–58% cheaper) |
| 🆕 ⚠️ **gpt-5.3-codex, gpt-5.1, gpt-5.4-nano** | 🆕 **DEPRECATED Oct 1, 2026 — shuts down April 1, 2027** | $1.75 / — / $0.20 | $14.00 / — / $1.25 | → `gpt-6-sol` (codex, 5.1) / `gpt-6-luna` (nano) |
| 🆕 ⚠️ **tts-1, tts-1-hd, old gpt-4o-mini-tts snapshots** | 🆕 **DEPRECATED Oct 1, 2026 — shuts down January 6, 2027** | — | — | → `gpt-realtime-2.1-mini` |
| ⚠️ **gpt-5-2025-08-07, gpt-5-mini, gpt-5-nano, gpt-5-pro (dated snapshots)** | **DEPRECATED — Shuts down December 11, 2026** (notice issued June 11, 2026; a separate, later wave than the Oct 23 cull) | — | — | → `gpt-5.6-sol` / `terra` / `luna` (see openai.md for exact mapping) |
| ⚠️ **o3-2025-04-16, o3-pro-2025-06-10 (dated snapshots)** | **DEPRECATED — Shuts down December 11, 2026** — already retired from ChatGPT Aug 26, 2026; this is the **API** shutdown date | $2.00 / $20.00 | $8.00 / $80.00 | → `gpt-5.6-sol` (o3) / `gpt-5.6-sol` `reasoning.mode: pro` (o3-pro) |
| ⚠️ **GPT-5.5** *(product-surface retirement)* | **Retires from ChatGPT, ChatGPT Work, and Codex Oct 14, 2026** — API is NOT affected, does not appear on Deprecations page | $5.00 | $30.00 | → `gpt-6.1-sol` (Codex/ChatGPT users only) |
| ⚠️ **o4-mini** | **DEPRECATED — Shuts down October 23, 2026** (confirmed via official Deprecations page) | $1.10 | $4.40 | → **`gpt-5.6-terra`** (official recommendation) |
| ⚠️ **GPT-4.1 nano** | **DEPRECATED — Shuts down October 23, 2026** (confirmed via official Deprecations page) | $0.10 | $0.40 | → **`gpt-5.6-luna`/`gpt-6-luna`** (official recommendation) |
| ⚠️ **o1** | **DEPRECATED — Shuts down October 23, 2026** | $15.00 | $60.00 | → **`gpt-5.6-sol`/`gpt-6-sol`** (official recommendation) |
| ⚠️ **o3-mini** | **DEPRECATED — Shuts down October 23, 2026** | — | — | → **`gpt-5.6-sol`/`gpt-6-sol`** |
| ⚠️ **o1-pro** | **DEPRECATED — Shuts down October 23, 2026** | — | — | → **`gpt-5.6-sol`** (`reasoning.mode: pro`) |
| ⚠️ **gpt-image-1** | **DEPRECATED — Shuts down October 23, 2026** | — | — | → **`gpt-image-2`** |
| ⚠️ **gpt-5.4-cyber** | **DEPRECATED — Shuts down October 1, 2026** | — | — | → **`gpt-5.6-cyber`** |
| ⚠️ whisper-1 / gpt-4o-transcribe / gpt-4o-mini-transcribe / gpt-4o-transcribe-diarize | **DEPRECATED Aug 26, 2026 — shut down Feb 26, 2027** | varies | varies | → `gpt-live-transcribe` or `gpt-transcribe` |
| ⚠️ gpt-realtime / gpt-audio / gpt-4o-realtime / gpt-realtime-mini / gpt-audio-mini family | **DEPRECATED — shut down Jan 20, 2027** | varies | varies | → `gpt-realtime-2.1`, `gpt-realtime-2.1-mini`, or `gpt-audio-1.5` |
| 🔄 GPT-Image-2 | 📉 **Repriced 50% cheaper**; demoted from flagship to value tier by GPT-Image-2.5 Sunburst/Flare — not deprecated | $4.00 *(was $8.00)* | $15.00 *(was $30.00)* | Still active — no migration needed |
| ⚠️ GPT-Realtime-2 | **LEGACY** · Superseded by `gpt-realtime-2.1` — identical pricing | $4.00 (text) / $32.00 (audio) | $24.00 (text) / $64.00 (audio) | → gpt-realtime-2.1 |
| ⚠️ GPT-Realtime-1.5 | **LEGACY** · Superseded first by gpt-realtime-2, now by gpt-realtime-2.1 | $4.00 (text) / $32.00 (audio) | $16.00 (text) / $64.00 (audio) | → gpt-realtime-2.1 |
| ⚠️ GPT-Realtime-Mini | **LEGACY** · Superseded by `gpt-realtime-2.1-mini` — identical pricing | $0.60 (text) / $10.00 (audio) | $2.40 (text) / $20.00 (audio) | → gpt-realtime-2.1-mini |
| ⚠️ GPT-4o mini TTS | **DEPRECATED** · Explicitly labeled "Deprecated" on live OpenAI models page | — | — | → gpt-realtime-2.1 or current TTS models |
| ⚠️ GPT-Image-1.5 | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | $8.00 | $32.00 | → gpt-image-2 |
| ⚠️ GPT-Image-1-mini | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | $2.50 | $8.00 | → gpt-image-2 |
| ⚠️ chatgpt-image-latest | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | — | — | → gpt-image-2 |
| ⚠️ GPT-5.4 Pro | LEGACY · Superseded by GPT-5.5 Pro (same std price, better perf) | $30.00 | $180.00 | → GPT-5.5 Pro |
| ⚠️ GPT-5.3 / Codex | LEGACY · Phasing out (still available as gpt-5.3-codex, now deprecated Oct 1, 2026) | $1.75 | $14.00 | → GPT-5.6 Terra or GPT-6.1 Sol |
| ⚠️ GPT-5.2 | LEGACY · **All GPT-5.2 retired from ChatGPT June 12, 2026 ❌**; `gpt-5.2-chat-latest` shut down Aug 10, 2026 | $1.75 | $14.00 | → GPT-5.4 or GPT-5.6 Terra |
| ⚠️ GPT-5.1 | **DEPRECATED Oct 1, 2026 — shuts down April 1, 2027** | — | — | → GPT-6.1 Sol / GPT-6 Sol |
| ⚠️ GPT-4o | LEGACY · dated snapshot `gpt-4o-2024-05-13` shuts down Oct 23, 2026; removed from ChatGPT Feb 13, 2026 | $2.50 | $10.00 | → GPT-4.1 or GPT-6.1 Sol |
| ⚠️ GPT-4o mini | LEGACY | $0.15 | $0.60 | → GPT-6 Luna ($0.10/$0.50) or GPT-4.1 nano *(also now deprecated)* |
| ⚠️ GPT-4 Turbo / GPT-4-0613 / gpt-4-1106-preview | **Shuts down October 23, 2026** | — | — | → gpt-5.6-sol / gpt-6.1-sol |
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
| 🆕 ⚠️ **Z.ai GLM 5.2** | **DEPRECATED Oct 1, 2026 — retires October 31, 2026** | → **Z.ai GLM 5.3** (same price) |
| 🆕 ⚠️ **Mixtral 8×22B** | **RETIRED** *(corrected this refresh — now confirmed in Mistral's official deprecated/retired table; was mistracked as Active)* | → **Mistral Large 3** |
| 🆕 ⚠️ **Mixtral 8×7B** | **RETIRED** *(corrected this refresh — now confirmed in Mistral's official deprecated/retired table; was mistracked as Active)* | → **Mistral Small 4** |
| 🆕 ⚠️ **OCR 4.0** | **DEPRECATED** *(corrected this refresh — now confirmed in Mistral's deprecated table; was "still active for existing integrations")* | → **OCR 4.1** (`mistral-ocr-latest`) — same price |
| 🆕 ✅ **Leanstral 1.5** | **RETIRED September 30, 2026** — confirmed occurred as scheduled | No successor announced yet |
| ⚠️ **Devstral 2** | **RETIRED July 31, 2026** | → **Mistral Medium 3.5** |
| ⚠️ **Devstral Small 2** | **RETIRED July 31, 2026** | → **Mistral Small 4** |
| ⚠️ **Magistral Medium (1.0/1.1/1.2)** | **RETIRED July 31, 2026** | → **Mistral Medium 3.5** with `reasoning_effort=high` |
| ⚠️ **Magistral Small (1.0/1.1/1.2)** | **RETIRED July 31, 2026** | → **Mistral Small 4** with `reasoning_effort=high` |
| ⚠️ **Mistral Medium 3.1** | **RETIRED August 31, 2026** | → **Mistral Medium 3.5** |
| ⚠️ **Mistral Medium 3** | **RETIRED August 31, 2026** | → **Mistral Medium 3.5** |
| ⚠️ **Mistral Small 3.2** | **RETIRED July 31, 2026** | → **Mistral Small 4** |
| ⚠️ **Mistral NeMo 12B** | **RETIRED July 31, 2026** | → **Ministral 3 8B/14B** or **Mistral Small 4** |
| ⚠️ OCR 3 v25.12 | **LEGACY** · Separately available for existing integrations (unaffected by OCR 4.0's deprecation) | → OCR 4.1 ($4/1K pages std, $2/1K batch) |
| 🔄 Leanstral v26.03 | **LEGACY** · Replaced by Leanstral 1.5, which has itself now retired | No successor announced for the line |
| ⚠️ Voxtral Mini 3B v25.07 | **LEGACY** · `voxtral-mini-2507` in legacy table; `voxtral-mini-latest` alias reassigned | → Voxtral Mini Transcribe 2 ($0.003/min) |
| ⚠️ Mistral Small Creative v25.12 | **LEGACY/RETIRED** · Previously-untracked Labs model, confirmed retired | → Verify on console.mistral.ai |
| ⚠️ Pixtral Large | **LEGACY** · Deprecated May 2026 | → Mistral Medium 3.5 or Mistral Small 4 |
| ⚠️ Devstral Small 1.1 / 1.0 | RETIRED | → Mistral Small 4 |
| ⚠️ Devstral Medium 1.0 | RETIRED | → Mistral Medium 3.5 |
| ⚠️ Mistral Small 3.1 / 3.0 | LEGACY | → Mistral Small 4 |
| ⚠️ Mistral Large 2.x | LEGACY | → Mistral Large 3 |
| ⚠️ Codestral 2501 / 24.05 | LEGACY | → Codestral 2508 |
| ⚠️ Mistral Saba, Pixtral 12B, Ministral 3B/8B (24.10), Codestral Mamba, Mathstral, Mistral 7B, Mistral Large/Small/Medium 1.0 | LEGACY | → Current generation equivalents (see mistral.md) |

---

## 🏷️ Price Change Log

| Date | Provider | Model | Change |
|---|---|---|---|
| 2026-10-05 | OpenAI | **GPT-6.1 Sol** | 🆕 **LAUNCHED at DevDay 2026** — replaces GPT-6 Sol on the pricing/model catalog after just 7 days; same $2/$10 price, cached input cut to $0.10/MTok (95% off). |
| 2026-10-05 | OpenAI | **GPT-6 Astra Ultrafast** | 🆕 **PRICED** — new 6× speed tier: $60/$6/$75/$300 per MTok (short ctx). |
| 2026-10-05 | OpenAI | **GPT-6 Cyber** | ✅ **Did NOT launch at DevDay** despite pre-event reporting — remains unconfirmed, discovery-only. |
| 2026-10-05 | OpenAI | **gpt-5.3-codex, gpt-5.1, gpt-5.4-nano** | 🆕 **DEPRECATED** — shut down April 1, 2027. |
| 2026-10-05 | Anthropic | **Claude Sonnet 5.5** | 🆕 **LAUNCHED** (Sept 28, 2026) — same $2/$10 price as Sonnet 5, 30%+ faster, Terminal-Bench 4.0 70.6%. Sonnet 5 now 🔄 REPLACED. |
| 2026-10-05 | Anthropic | **Claude Sonnet 4.5** | ⚠️ **DEPRECATED** (Sept 30, 2026) — tentative retirement November 30, 2026 on the Claude API. |
| 2026-10-05 | Mistral | **Z.ai GLM 5.2** | ⚠️ **DEPRECATED** (Oct 1, 2026) — retires October 31, 2026; GLM 5.3 now sole active third-party model. |
| 2026-10-05 | Mistral | **Mixtral 8×7B, Mixtral 8×22B** | ⚠️ **CONFIRMED RETIRED** — now in Mistral's official deprecated/retired table; corrects prior "Active" tracking. |
| 2026-10-05 | Mistral | **OCR 4.0** | ⚠️ **CONFIRMED DEPRECATED** — fully superseded by OCR 4.1. |
| 2026-10-05 | Mistral | **Leanstral 1.5** | ✅ **RETIREMENT CONFIRMED** — occurred as scheduled on Sept 30, 2026. |
| 2026-09-28 | OpenAI | **Sora-2, Sora-2-Pro, Videos API** | ❌ **SHUTDOWN NOW IN EFFECT** — the September 24, 2026 date confirmed last cycle has passed; still no replacement model listed. |
| 2026-09-28 | OpenAI | **GPT-6 Cyber** *(discovery-only)* | 🆕 Reported in alpha via Daybreak Red (Fortune, Sept 24); possible DevDay preview Sept 29, 2026. No pricing/model ID published — not tracked as a card. |
| 2026-09-28 | Anthropic | **All active + legacy models** | ✅ RE-VERIFIED — Zero price changes since the September 22 refresh. Sonnet 5.5/Haiku 5.5 still unreleased, unpriced. |
| 2026-09-28 | Mistral | **All active + legacy models** | ✅ RE-VERIFIED — Zero price changes since the September 23 refresh. Leanstral 1.5 retirement now 2 days out. |
| 2026-09-23 | OpenAI | **Sora-2, Sora-2-Pro, Videos API** | 🆕 **CONFIRMED DEPRECATED — shuts down September 24, 2026** (notice issued March 24, 2026). No replacement model listed. |
| 2026-09-23 | OpenAI | **GPT-5.6 Terra** | ✅ **CONFIRMED UNCHANGED** — directly verified via its own model page: $2.00/$12.00, still labeled "Default," no GPT-6 equivalent yet. |
| 2026-09-23 | Anthropic | **All active + legacy models** | ✅ RE-VERIFIED — Zero price changes since the September 22 refresh (Opus 5.5 launch). |
| 2026-09-23 | Mistral | **All active + legacy models** | ✅ RE-VERIFIED — Zero price changes detected since the September 22 refresh. |
| 2026-09-22 | Anthropic | **Claude Opus 5.5** | 🆕 **NEW LEADING MODEL** — Launched Sept 22, 2026 at $4.00/$20.00 per MTok (20% cheaper than Opus 5), $0.20/MTok cache reads (60% cheaper). Anthropic estimates ~40% lower cost than Opus 5 on typical workloads. First model in the new "Claude 5.5" family; Sonnet 5.5 and Haiku 5.5 to follow. Opus 5 is now 🔄 REPLACED but remains fully active. |
| 2026-09-22 | OpenAI | **GPT-6 Sol, GPT-6 Luna** | 🆕 **NEW MODELS** — Launched Sept 22, 2026, expanding the GPT-6 family. Both 50% cheaper than the GPT-5.6 promotional rates they replace: Sol $4.00/$20.00 → **$2.00/$10.00**; Luna $0.20/$1.20 → **$0.10/$0.50**. No GPT-6 Terra — GPT-5.6 Terra ($2.00/$12.00) is unchanged. GPT-5.6 Sol/Luna are now 🔄 REPLACED but remain fully active. |
| 2026-09-22 | OpenAI | **GPT-6 prompt caching** | 🆕 **IMPROVED CACHING MECHANICS** — Higher default cache-hit rates, 30-minute prefix-reuse window, and mid-conversation `configuration_update` reasoning-effort/tool changes that preserve cache. No price change. |
| 2026-09-21 | OpenAI | **o3, o3-pro, GPT-5 snapshot family** | ⚠️ **CONFIRMED DEPRECATED — Shuts down December 11, 2026.** Distinct, later wave (notice issued June 11, 2026) from the October 23 cull. `gpt-5-2025-08-07`→sol, `gpt-5-mini`→terra, `gpt-5-nano`→luna, `gpt-5-pro`/`o3-pro`→sol (reasoning.mode: pro), `o3`→sol. |
| 2026-09-21 | OpenAI | **GPT-5.5** | 🆕 **RETIRING FROM CHATGPT/CODEX Oct 14, 2026** (announced Sept 15) — the OpenAI API is explicitly unaffected; product-surface retirement only. |
| 2026-09-21 | OpenAI | **Astra for Law** | 🆕 **NEW VERTICAL SOLUTION** — GPT-6-Astra-based legal foundation for law firms (Harvey, Legora); no separate SKU, billed at standard Astra rates. |
| 2026-09-21 | Mistral | **Devstral 2, Devstral Small 2, Magistral Medium, Magistral Small** | ⚠️ **CORRECTED TO RETIRED (July 31, 2026)** — previously mistracked as Active in this repo across multiple refreshes. Migrate to Mistral Medium 3.5 / Small 4. |
| 2026-09-21 | Mistral | **Mistral Medium 3, Medium 3.1** | ⚠️ **CORRECTED TO RETIRED (August 31, 2026)** — previously only listed as "Legacy." |
| 2026-09-21 | Mistral | **Mistral Small 3.2, Mistral NeMo 12B** | ⚠️ **CORRECTED TO RETIRED (July 31, 2026)** — NeMo was previously mistracked as still active on the API. |
| 2026-09-21 | Mistral | **Z.ai GLM-5.3** | 🆕 **NEW MODEL** — Mistral's second third-party hosted open model (~Sept 15, 2026), same pricing as GLM-5.2 ($1.40/$4.40, 1M context). |
| 2026-09-21 | Mistral | **Native model cached-input pricing** | 🆕 **NEW PRICING PUBLISHED** — Large 3, Medium 3.5, Small 4, Ministral tiers, Codestral, Codestral Embed, OCR 4.1/4.0, and Voxtral Mini Transcribe 2 all gained a published 90%-off cached-input rate for the first time. |
| 2026-09-21 | Mistral | **Mistral Moderation 2** | 📉 **CORRECTED TO FREE** — previously tracked at $0.10/MTok; live pricing page lists it as Free. |
| 2026-09-21 | Anthropic | **All active + legacy models** | ✅ RE-VERIFIED — Zero price changes detected since Sept 14. New non-pricing items: LSVP beta (Sept 17), Accenture partnership (Sept 18), R&D Automation Index (Sept 17), Cowork/chat merge (Sept 16). |
| 2026-09-14 | OpenAI | **o4-mini, GPT-4.1 nano** | ⚠️ **CONFIRMED DEPRECATED** — Official Deprecations page confirms both shut down **October 23, 2026**. Moved from Active to Legacy. Migrate to `gpt-5.6-terra` (o4-mini) and `gpt-5.6-luna` (GPT-4.1 nano). `o1`, `o3-mini`, `o1-pro`, and `gpt-image-1` are also on the same Oct 23, 2026 shutdown list; `gpt-5.4-cyber` shuts down Oct 1, 2026. |
| 2026-09-14 | OpenAI | **GPT-Live-1** | 🆕 **NOW PRICED IN THE API** — $0.05/minute for the voice layer, launched Sept 10, 2026. Previously ChatGPT-only and unpriced. |
| 2026-09-14 | OpenAI | **Agents API** | 🆕 **NEW PRODUCT** — Public beta launched Sept 10, 2026; managed Codex-harness agent runtime with no additional fees beyond standard token/tool rates. |
| 2026-09-14 | OpenAI | **GPT-Image-2.5 Sunburst / Flare** | 🆕 **NEW FLAGSHIP IMAGE MODELS** — $8/$2 cached/$30 image, $5/$1.25 cached text per MTok — the price GPT-Image-2 used to carry. |
| 2026-09-14 | OpenAI | **GPT-Image-2** | 📉 **REPRICED 50% CHEAPER** — Image $8→$4, cached $2→$1, output $30→$15 per MTok (text similarly halved); demoted from flagship to value tier, not deprecated. |
| 2026-09-14 | OpenAI | **gpt-rosalind-research** | 🆕 **PRICING PUBLISHED** — $5.00/$0.50 cached/$25.00 per MTok; billing begins October 5, 2026. Life Sciences trusted-access model. |
| 2026-09-14 | Anthropic | **All active + legacy models** | ✅ RE-VERIFIED — Zero price changes detected against the live pricing pages since Sept 7. |
| 2026-09-14 | Mistral | **All active + legacy models** | ✅ RE-VERIFIED — Zero price changes detected against the live pricing page since Sept 7. Mistral raised a €3B Series D funding round (Sept 8, 2026) — no pricing impact. |
| 2026-09-07 | OpenAI | **GPT-6 Astra** | 🆕 **NEW FLAGSHIP MODEL** — Launched September 3, 2026 at $10.00/$50.00 per MTok (short context), OpenAI's first model to reach the "Critical" cybersecurity capability threshold under its Preparedness Framework. 1.05M context, 128K max output, Apr 30 2026 knowledge cutoff. Replaces GPT-5.6 Sol as OpenAI's recommended flagship. |
| 2026-09-07 | OpenAI | **GPT-5.6 Sol** | 📉 **PROMOTIONAL PRICE CUT** — $5.00/$30.00 → **$4.00/$20.00** per MTok (short context), as Sol steps down from flagship status in favor of GPT-6 Astra. Promotional pricing available at least through November 21, 2026. Long context: $10.00/$45.00 → $8.00/$30.00. |
| 2026-09-07 | OpenAI | **gpt-5.6-cyber** | 🆕 **PRICING PUBLISHED** — $12.50/$1.25 cached/$75.00 per MTok (short context only), previously unpriced. |
| 2026-09-07 | Anthropic | **Claude Fable 5.1 / Mythos 5.1** | 🆕 **NEW MODELS** — Launched September 1, 2026, replacing Fable 5/Mythos 5 as Anthropic's most advanced models. Same $10.00/$50.00 base price, but cache-read pricing cut 75% (from $1.00/MTok to $0.25/MTok). |
| 2026-09-07 | Anthropic | **Claude Sonnet 5** | ✅ **PRICING CONFIRMED PERMANENT** — The $2.00/$10.00 introductory rate is now permanent; the scheduled September 1, 2026 increase to $3.00/$15.00 will not occur. |
| 2026-09-07 | Mistral | **Z.ai GLM-5.2** | 🆕 **NEW MODEL** — Mistral's first third-party hosted open model (announced Aug 11, 2026), $1.40/$0.14 cached/$4.40 per MTok, 1M context. |
| 2026-09-07 | Mistral | **OCR 4.1** | 🆕 **NEW MODEL** — Supersedes OCR 4.0 as flagship OCR; identical pricing ($4/$2/$5 per 1K pages); adds block-level confidence scores. |
| 2026-08-03 | OpenAI | **GPT-5.6 Terra / Luna** | 📉 **PRICE CUTS** — Terra: $2.50/$15.00 → $2.00/$12.00. Luna: $1.00/$6.00 → $0.20/$1.20 (~80% cut). |
| 2026-07-27 | Anthropic | **Claude Opus 5** | 🆕 **NEW MODEL** — Launched July 24, 2026 at $5.00/$25.00, replacing Opus 4.8 as Max default/strongest-on-Pro. |
| 2026-07-14 | OpenAI | **GPT-5.6 (Sol/Terra/Luna)** | 🆕 **REACHED GENERAL AVAILABILITY — July 9, 2026.** |
| 2026-06-30 | Anthropic | **Claude Sonnet 5** | 🆕 NEW MODEL — Launched June 30, 2026, introductory pricing $2/$10 (later made permanent Sept 1, 2026). |
| 2026-04-29 | Mistral | **Mistral Medium 3.5** | 🆕 LAUNCHED — $1.50/$7.50. 256K context. 128B dense. |

> ℹ️ For the full historical change log (entries prior to July 2026), see the git history of this file or the individual provider model-card files, which retain complete per-refresh detail.

---

## ℹ️ Notes
- All prices are in **USD** per million tokens (MTok) unless stated otherwise.
- **Batch API discounts (50%)** apply at Anthropic, OpenAI, Mistral, and Google Gemini.
- **Prompt/context caching** discounts now apply broadly. As of Sept 21, 2026, **Mistral's own native models publish cached-input pricing for the first time** (90% off) — this was previously exclusive to third-party-hosted GLM models on Mistral's platform. OpenAI's GPT-6/GPT-5.6 generation uses a cache-write-at-1.25× model, with improved default cache-hit rates and a 30-minute reuse window added Sept 22, 2026. Anthropic's Fable 5.1/Mythos 5.1 cut cache-read pricing to 0.025× (from 0.1×), and Opus 5.5 cut cache-read pricing to 0.05× — the cheapest cache reads of any tracked provider remain Fable 5.1/Mythos 5.1.
- Enterprise/volume pricing available from all providers on request.
- **OpenAI GPT-6, GPT-5.6, GPT-5.5, and GPT-5.4** have short-context (<~270–272K) and long-context (>~270–272K) pricing tiers.
- **OpenAI service tiers:** Priority/Fast mode → Standard → Batch/Flex (50% off).
- **OpenAI now has multiple deprecation waves in flight:** September 24, 2026 (Sora-2, Sora-2-Pro, Videos API — no replacement), October 23, 2026 (o1, o3-mini, o1-pro, o4-mini, gpt-4.1-nano, gpt-image-1, legacy GPT-4/3.5 family), and a **separate, later** December 11, 2026 wave (o3, o3-pro, and the original dated GPT-5/mini/nano/pro snapshots).
- **Google Gemini Pro** models double input cost for prompts >200K tokens.
- **Mistral** processes API data in the EU by default, with **Regional Endpoints now GA** for EU/US choice (+10% surcharge), and a new SLA-backed **Priority Tier** in public preview.
- **Anthropic** offers US-only inference at 1.1× pricing via `inference_geo: "us"` parameter.
- **Tool/agent pricing is additive:** Anthropic Web Search ($10/1K searches), Code Execution, Computer/Browser use tools, and Claude Managed Agents ($0.08/session-hour); OpenAI Web Search ($10–25/1K calls), Computer Use, Containers, File Search, GPT-Live-1 sessions ($0.05/min), and the Agents API (no extra fee); Mistral Agent API (Web Search/Code Execution at $30/1K calls, Libraries, Image Generation) all bill on top of standard per-model token rates.
- ⚠️ Models marked **RETIRED** return API errors. **DEPRECATED** = end-of-life published. **LEGACY** = still accessible but in provider's legacy section. **SUSPENDED** = access halted by external directive. **🔄 REPLACED** = superseded by a newer default/recommended model but still active and not deprecated. **🔓 RESTORED** = a previously suspended model has regained access. **📉 PRICE CUT** = confirmed price decrease on an active model.
- 🆕 **Unpriced/discovery-only items** (e.g., Mistral's Shieldstral 1.0 and Robostral Navigate) are noted for awareness but are **not** given a full tracked model card until the provider publishes official pricing/specs.
- 🆕 **September 23, 2026 — OpenAI:** Confirmed a new deprecation — the Videos API, `sora-2`, and `sora-2-pro` shut down September 24, 2026 with no replacement model listed. Also directly verified GPT-5.6 Terra's own model page: unchanged, still labeled "Default," no GPT-6 equivalent.
- 🆕 **September 22, 2026 — Anthropic:** Claude Opus 5.5 launched, replacing Claude Opus 5 as the leading model at $4.00/$20.00 (20% cheaper) with $0.20/MTok cache reads (60% cheaper); Opus 5 is now 🔄 REPLACED but fully active.
- 🆕 **September 22, 2026 — OpenAI:** GPT-6 Sol and GPT-6 Luna launched, each 50% cheaper than the GPT-5.6 promotional rates they replace; GPT-5.6 Terra is unchanged (no GPT-6 Terra yet); improved prompt caching shipped for the whole GPT-6 family (higher hit rates, 30-minute reuse window).
- ⚠️ **September 21, 2026 — major Mistral corrections:** Devstral 2, Devstral Small 2, and the entire Magistral family (all versions) were confirmed **RETIRED July 31, 2026** — this repo had previously (incorrectly) carried them as Active across several refreshes. Mistral Medium 3/3.1 were confirmed **RETIRED August 31, 2026** (previously only "Legacy"). Mistral Small 3.2 and Mistral NeMo 12B were also confirmed RETIRED July 31, 2026.
- 🆕 **September 21, 2026 — OpenAI:** confirmed a second, later deprecation wave shuts down `o3`, `o3-pro`, and the original dated GPT-5 snapshot family on **December 11, 2026** (notice issued June 11, 2026); GPT-5.5 will retire from ChatGPT/ChatGPT Work/Codex on **October 14, 2026** but the API is unaffected; "Astra for Law" launched as a GPT-6-Astra-based vertical solution.
- 🆕 **September 17, 2026:** Anthropic opened its **Life Sciences Verification Program (LSVP)** in beta for Mythos/Opus/Sonnet access with relaxed biology-work safeguards.
- ⚠️ **September 14, 2026:** Confirmed via OpenAI's official Deprecations page that **`o4-mini` and `GPT-4.1 nano` are deprecated and shut down October 23, 2026** — both moved from Active to Legacy, alongside `o1`, `o3-mini`, `o1-pro`, and `gpt-image-1` (same shutdown date) and `gpt-5.4-cyber` (shuts down Oct 1, 2026).
- 🆕 **September 10, 2026:** OpenAI launched **GPT-Live-1 in the API** ($0.05/min) and the new **Agents API** (public beta, no added fees).
- 🆕 **September 3, 2026:** OpenAI launched **GPT-6 Astra**, its new flagship model and first to reach "Critical" cybersecurity capability status; GPT-5.6 Sol was demoted to a promotional $4.00/$20.00 price point.
- 🆕 **September 1, 2026:** Anthropic launched **Claude Fable 5.1 and Mythos 5.1**, cutting cache-read pricing 75% versus Fable 5/Mythos 5; **Claude Sonnet 5's $2/$10 pricing was confirmed permanent.**
- 📝 **October 5, 2026:** This refresh independently re-verified Anthropic, OpenAI, and Mistral pricing directly against each provider's live pricing/docs pages. **Key findings:** Anthropic launched **Claude Sonnet 5.5** (Sept 28) at the same $2/$10 price as Sonnet 5, running 30%+ faster with a 70.6% Terminal-Bench 4.0 score; Sonnet 5 is now 🔄 REPLACED, and Claude Sonnet 4.5 was deprecated (Sept 30) with a November 30, 2026 retirement date. OpenAI held **DevDay 2026** (Sept 29), launching **GPT-6.1 Sol** (replacing GPT-6 Sol after just 7 days — same price, cheaper cached input), a priced **Ultrafast** tier for GPT-6 Astra, **Dots** always-on agents, a **Pro 500** plan, and **Private Intelligence**; `GPT-6 Cyber`, despite pre-event reporting, did **not** appear at DevDay and remains unconfirmed. A new OpenAI deprecation wave (Oct 1) was also confirmed for `gpt-5.3-codex`/`gpt-5.1`/`gpt-5.4-nano` (Apr 1, 2027 shutdown) and legacy TTS models (Jan 6, 2027 shutdown). Mistral deprecated **Z.ai GLM 5.2** (retiring Oct 31, 2026, superseded by GLM 5.3 at the same price), and this refresh additionally discovered that **Mixtral 8×7B/8×22B and OCR 4.0 are now confirmed retired/deprecated** in Mistral's own model-lifecycle table — correcting prior tracking that listed them as active. Mistral's Leanstral 1.5 retirement (Sept 30) is now confirmed to have occurred. Google Gemini and OpenRouter Picks tables reflect the last confirmed figures from a prior refresh and were not re-verified this cycle.
- 📝 **September 28, 2026:** This refresh independently re-verified Anthropic, OpenAI, and Mistral pricing against each provider's live pricing/docs pages and news feeds. **Key finding:** the Sora-2/Sora-2-Pro/Videos API deprecation confirmed last cycle has now actually taken effect (Sept 24 shutdown date passed, no replacement listed); discovered an unpriced report that OpenAI is alpha-testing a fourth cybersecurity model, `GPT-6 Cyber`, with a possible DevDay preview on Sept 29 — not tracked as a card pending official pricing. Anthropic and Mistral pricing were re-verified with **zero changes**; Claude Sonnet 5.5/Haiku 5.5 remain confirmed-but-unpriced, and Mistral's Leanstral 1.5 retirement (Sept 30) is now 2 days out. Google Gemini and OpenRouter Picks tables reflect the last confirmed figures from a prior refresh and were not re-verified this cycle.
- 📝 **September 23, 2026:** This refresh independently re-verified Anthropic, OpenAI, and Mistral pricing against each provider's live pricing/docs pages and news feeds. **Key finding:** OpenAI's Videos API, Sora-2, and Sora-2-Pro are confirmed deprecated, shutting down September 24, 2026 with no replacement model listed; GPT-5.6 Terra was directly re-confirmed unchanged via its own model page. Anthropic and Mistral pricing were re-verified with **zero changes** since the September 22 refresh. Google Gemini and OpenRouter Picks tables reflect the last confirmed figures from a prior refresh and were not re-verified this cycle.
- 📝 **September 22, 2026:** This refresh independently re-verified Anthropic, OpenAI, and Mistral pricing against each provider's live pricing/docs pages and news feeds. **Key changes:** Anthropic launched **Claude Opus 5.5**, replacing Claude Opus 5 as the leading model at $4.00/$20.00 per MTok (20% cheaper) with $0.20/MTok cache reads (60% cheaper) — Opus 5 is now 🔄 REPLACED but remains fully active; Sonnet 5.5 and Haiku 5.5 are announced to follow. OpenAI launched **GPT-6 Sol** ($2.00/$10.00) and **GPT-6 Luna** ($0.10/$0.50), each 50% cheaper than the GPT-5.6 promotional rates they replace, and shipped improved GPT-6 prompt caching (higher hit rates, 30-minute reuse window) — **there is no GPT-6 Terra**, so GPT-5.6 Terra remains OpenAI's un-replaced mid-tier "Default" model. Mistral pricing was re-verified with **zero changes** since the September 21 correction cycle. Google Gemini and OpenRouter Picks tables reflect the last confirmed figures from a prior refresh and were not re-verified this cycle.
- 📝 **September 21, 2026:** This refresh independently re-verified Anthropic, OpenAI, and Mistral pricing against each provider's live pricing/docs pages, plus each provider's news feed and (for OpenAI) the official Deprecations page. **Key changes:** OpenAI confirmed a second Dec 11, 2026 deprecation wave (o3/o3-pro/GPT-5 snapshots) and GPT-5.5's Oct 14 ChatGPT/Codex retirement (API unaffected), plus the new "Astra for Law" vertical; Mistral's tracker received **major corrections** — Devstral/Magistral (all versions), Mistral Medium 3/3.1, Small 3.2, and NeMo 12B are all now correctly marked RETIRED, Z.ai GLM-5.3 was added, native cached-input pricing was discovered, and Mistral Moderation 2 was corrected to Free. Anthropic pricing was re-verified with **zero changes** — its only news was non-pricing (LSVP beta, Accenture partnership, R&D index, Cowork/chat merge). Google Gemini and OpenRouter Picks tables reflect the last confirmed figures from a prior refresh and were not re-verified this cycle.
