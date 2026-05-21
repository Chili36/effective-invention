# 🤖 LLM Pricing Tracker

Up-to-date pricing and specifications for large language models from **Anthropic**, **OpenAI**, **Google Gemini**, **Mistral AI**, and top **OpenRouter picks**.

> **Last updated:** 2026-05-21 (refresh #14)  
> **Sources:** Official provider pricing pages + third-party verification — scraped/verified on date above.

---

## 📋 Quick-Reference Index — Active Models

### 🟠 Tier 1 — Anthropic Claude

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Claude Opus 4.7** *(Current Flagship)* | $5.00 | $25.00 | **1M tokens** | API, AWS Bedrock (all regions), Vertex AI, MS Foundry, GitHub Copilot Pro+ |
| Claude Opus 4.6 *(prev flagship)* | $5.00 | $25.00 | **1M tokens** | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Sonnet 4.6** | $3.00 | $15.00 | **1M tokens** | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Haiku 4.5** | $1.00 | $5.00 | 200K tokens | API, AWS Bedrock (all regions), Vertex AI, MS Foundry |
| Claude Opus 4.5 | $5.00 | $25.00 | 200K tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Sonnet 4.5 ⚠️ | $3.00 | $15.00 | 200K tokens *(1M beta **RETIRED Apr 30** — use Sonnet 4.6; retirement date TBD)* | API, AWS Bedrock, Vertex AI, MS Foundry |

> 💡 Batch API: 50% off · Prompt caching: up to 90% off · **Opus 4.6 Fast Mode only**: $30/$150 (6× base) *(not available on Opus 4.7)*  
> ❌ **Claude Sonnet 4.5 1M context beta CONFIRMED RETIRED April 30, 2026** — migrate to Sonnet 4.6  
> ⚠️ **Claude Sonnet 4.5 formal retirement date pending** — proactively migrate to Sonnet 4.6 now  
> 🔒 Claude Mythos Preview (Project Glasswing) — restricted access only; no public API  

---

### 🟢 Tier 1 — OpenAI (Proprietary)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|---|
| **GPT-5.5** *(Current Flagship)* | $5.00 / $10.00* | $0.50 | $30.00 / $45.00* | **1.05M tokens** | API |
| **GPT-5.5 Pro** | $30.00 | — | $180.00 | 1M tokens | API |
| GPT-5.4 *(prev flagship)* | $2.50 / $5.00† | $0.25 / $0.50† | $15.00 / $22.50† | 1.05M tokens | API |
| GPT-5.4 Pro *(prev ultra-premium)* | $30.00 | — | $180.00 | 1.05M tokens | API |
| **GPT-5.4 mini** | $0.75 | $0.075 | $4.50 | 400K tokens | API |
| **GPT-5.4 nano** | $0.20 | $0.020 | $1.25 | 400K tokens | API |
| GPT-4.1 | $2.00 | $0.50 | $8.00 | 1.04M tokens | API |
| **GPT-4.1 mini** | $0.40 | $0.10 | $1.60 | 1.00M tokens | API |
| GPT-4.1 nano | $0.10 | — | $0.40 | 1M+ tokens | API |
| o3 *(reasoning)* | $2.00 | $0.50 | $8.00 | 200K tokens | API |
| o3-pro *(reasoning)* | $20.00 | — | $80.00 | 200K tokens | API |
| o4-mini *(reasoning)* | $1.10 | $0.275 | $4.40 | 200K tokens | API |

> 💡 Batch API: 50% off all models · Cached inputs: 50–90% off · Regional processing: +10% on GPT-5.5 and GPT-5.4 family  
> *GPT-5.5 long-context pricing (>272K tokens): **2× input ($10.00) / 1.5× output ($45.00)** for the full session — plan context budgets accordingly  
> †GPT-5.4 tiered pricing: short ctx (<272K) / long ctx (>272K) — standard rates below 272K  
> ✏️ **Correction (May 21, 2026):** GPT-5.5 context window corrected **1M → 1.05M tokens**; long-context surcharge added (previously omitted — GPT-5.5 is NOT flat-rate)  
> ⏰ **GPT-5.2 and GPT-5.3 retiring June 2026** — migrate to GPT-5.4 or GPT-5.5  
> 🔒 GPT-5.4-Cyber — limited vetted access only; no public API pricing

---

### 🔵 Tier 1 — Google Gemini

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Notes |
|---|---|---|---|---|
| **Gemini 3.5 Flash** 🆕 *(New Flagship — May 19, 2026)* | $1.50 | $9.00 | **1M tokens** | GA Stable; thinking supported; fastest frontier model |
| **Gemini 3.1 Pro Preview** | $2.00 / $4.00* | $12.00 / $18.00* | **1M tokens** | *Tiered at >200K; Preview |
| **Gemini 3.1 Flash-Lite** 🆕 *(Stable GA)* | $0.25 | $1.50 | **1M tokens** | GA Stable (May 2026); thinking supported |
| **Gemini 3.1 Flash-Lite Preview** | $0.25 | $1.50 | **1M tokens** | Preview |
| **Gemini 2.5 Pro** | $1.25 / $2.50* | $10.00 / $15.00* | **1M tokens** | *Tiered at >200K; GA |
| **Gemini 2.5 Flash** | $0.30 | $2.50 | **1M tokens** | GA; optional thinking mode |
| **Gemini 2.5 Flash-Lite** | $0.10 | $0.40 | **1M tokens** | GA; cheapest Gemini |
| ~~Gemini 2.0 Flash~~ ⚠️ | $0.10 | $0.40 | 1M tokens | ⚠️ **DEPRECATED — Shutdown June 1, 2026** |

> 💡 Batch API: 50% off · Context caching: 90% off repeated prefixes · Free tier via AI Studio · Pro models: double input cost for prompts >200K  
> 🆕 **Gemini 3.5 Flash** (May 19, 2026): New stable GA flagship; outperforms Gemini 3.1 Pro on agentic/coding benchmarks at a lower price ($1.50 vs $2.00 input); 4× faster  
> ⚠️ **Gemini 2.0 Flash DEPRECATED** — official shutdown **June 1, 2026**. Migrate to 2.5 Flash or 3.5 Flash immediately  
> 📅 **Gemini 3.5 Pro** coming June 2026 — already in internal use at Google  

---

### 🟡 Tier 1 — Mistral AI

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Mistral Medium 3.5** 🆕 *(Apr 29, 2026)* | $1.50 | $7.50 | 256K tokens | API (Mistral AI Studio) |
| **Pixtral Large** 🆕 | $2.00 | $6.00 | 128K tokens | API (Mistral AI Studio) |
| **Mistral Large 3 (2512)** | $0.50 | $1.50 | 256K tokens | API (Mistral AI Studio) |
| **Magistral Medium 1.2** | $2.00 | $5.00 | 128K tokens *(best <40K)* | API (Mistral AI Studio) |
| **Magistral Small 1.2** | $0.50 | $1.50 | 128K tokens *(best <40K)* | API (Mistral AI Studio) |
| Mistral Medium 3.1 *(check alias routing)* | $0.40 | $2.00 | 131K tokens | API (Mistral AI Studio) |
| **Mistral Small 4** *(Mar 2026)* | $0.15 | $0.60 | **256K tokens** | API (Mistral AI Studio) |
| Codestral 2508 | $0.30 | $0.90 | 256K tokens | API (Mistral AI Studio) |
| **Devstral 2 (2512)** | $0.40 | $0.90 | 256K tokens | API (Mistral AI Studio) |
| **Devstral Small 2** 🆕 | $0.10 | $0.30 | **256K tokens** | API (Mistral AI Studio) |
| Mistral Small Creative | $0.10 | $0.30 | 33K tokens | API (Mistral AI Studio) |
| Voxtral Small 24B | $0.10 | $0.30 | 128K tokens | API (Mistral AI Studio) |
| Voxtral TTS | $0.016/1K chars | — | — | API (Mistral AI Studio) |
| Mistral Nemo | $0.15 | $0.15 | 128K tokens | API (Mistral AI Studio) |
| Ministral 14B | $0.20 | $0.20 | 256K tokens | API (Mistral AI Studio) |
| Ministral 8B | $0.10 | $0.10 | 256K tokens | API (Mistral AI Studio) |
| Ministral 3B | $0.04 | $0.04 | 556K tokens | API (Mistral AI Studio) |

> 💡 EU data residency by default · Free experimentation tier · Open-weight models (Apache 2.0/modified MIT) for self-hosting  
> 🆕 **Mistral Medium 3.5** (Apr 29, 2026) — 128B dense flagship; $1.50/$7.50; 256K ctx; replaces Devstral 2 in Vibe; vision + configurable reasoning + coding in one model  
> 🆕 **Pixtral Large** — multimodal flagship; $2.00/$6.00; 128K context; vision + text; dedicated model card added May 21, 2026  
> 🆕 **Devstral Small 2** (Dec 2025) — replaces Devstral Small 1.1; $0.10/$0.30; 256K context; ~58% SWE-bench; added to active table May 21, 2026  
> ⚠️ **`mistral-medium-latest` alias may now route to Medium 3.5** — verify your version via API response `model` field  
> ✏️ **Ministral 3B price corrected (May 18, 2026):** $0.04/$0.04 per MTok (was $0.10/$0.10) — verified from mistral.ai/pricing via aipricing.guru May 16, 2026

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

---

## 📁 Model Card Files

| Provider | Tier | File | Description |
|---|---|---|---|
| Anthropic | 1 | [anthropic.md](./anthropic.md) | Full model cards incl. caching, batch, fast mode (Opus 4.6 only), deprecation dates |
| OpenAI | 1 | [openai.md](./openai.md) | Full model cards incl. context tiers (GPT-5.5 + GPT-5.4), reasoning models, batch pricing |
| Google Gemini | 1 | [gemini.md](./gemini.md) | Full model cards incl. Gemini 3.5 Flash (new flagship), 3.1 Flash-Lite stable GA, 2.0 Flash deprecation |
| Mistral AI | 1 | [mistral.md](./mistral.md) | Full model cards incl. Medium 3.5, Pixtral Large, Devstral Small 2, Magistral reasoning, open-weight |
| OpenRouter Picks | 2 | [openrouter-picks.md](./openrouter-picks.md) | One best-performing model per Tier 2 provider, all via OpenRouter |

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new deployments.

### 🟠 Anthropic — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ Claude Sonnet 4.5 | DEPRECATED · Retirement date TBD — migrate proactively | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude Sonnet 4 | **RETIRED April 20, 2026 ❌ API ERRORS** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude Opus 4.1 | LEGACY | $15.00 | $75.00 | → Claude Opus 4.7 (67% cheaper) |
| ⚠️ Claude Opus 4 | **RETIRED April 20, 2026 ❌ API ERRORS** | $15.00 | $75.00 | → Claude Opus 4.7 |
| ⚠️ Claude Haiku 3.5 | **RETIRED February 19, 2026 ❌ API ERRORS** | $0.80 | $4.00 | → Claude Haiku 4.5 |
| ⚠️ Claude Haiku 3 | **RETIRED February 19, 2026 ❌ API ERRORS** | $0.25 | $1.25 | → Claude Haiku 4.5 |
| ⚠️ Claude Sonnet 3.7 | **RETIRED October 28, 2025 ❌ API ERRORS** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 3 Opus | **DEPRECATED** Jan 2026 — available by request for paying customers | $15.00 | $75.00 | → Claude Opus 4.7 |
| ⚠️ Claude 3.5 Sonnet | **RETIRED January 5, 2026** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 2.x | **RETIRED** | ~$8.00 | ~$24.00 | → Claude Sonnet 4.6 |

### 🟢 OpenAI — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ GPT-5.4 Pro | LEGACY · Superseded by GPT-5.5 Pro | $30.00 | $180.00 | → GPT-5.5 Pro (same price, better performance) |
| ⚠️ GPT-5.3 / Codex | LEGACY · Phasing out Jun 2026 | $1.75 | $14.00 | → GPT-5.5 or GPT-5.4 |
| ⚠️ GPT-5.2 | LEGACY · Retiring Jun 2026 (Thinking: Jun 5) | $1.75 | $14.00 | → GPT-5.4 or GPT-5.5 |
| ⚠️ GPT-5.1 | **RETIRED March 11, 2026** | — | — | → GPT-5.5 |
| ⚠️ GPT-4o | LEGACY | $2.50 | $10.00 | → GPT-4.1 (cheaper, 1M ctx) |
| ⚠️ GPT-4o mini | LEGACY | $0.15 | $0.60 | → GPT-5.4 nano or GPT-4.1 nano |
| ⚠️ o1 | LEGACY (very expensive) | $15.00 | $60.00 | → o3 (87% cheaper) |
| ⚠️ GPT-4 Turbo | **RETIRED** | — | — | → GPT-4.1 |
| ⚠️ GPT-3.5 Turbo | **RETIRED** | — | — | → GPT-4.1 nano |

### 🔵 Google Gemini — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ Gemini 2.0 Flash | **DEPRECATED · Shutdown June 1, 2026** | → Gemini 2.5 Flash ($0.30/$2.50) or Gemini 3.5 Flash ($1.50/$9.00) |
| ⚠️ Gemini 2.0 Flash-Lite | **DEPRECATED · Shutdown June 1, 2026** | → Gemini 2.5 Flash-Lite ($0.10/$0.40) |
| ⚠️ Gemini 3 Pro Preview | **RETIRED** March 9, 2026 | → Gemini 3.5 Flash or Gemini 3.1 Pro Preview |
| ⚠️ Gemini 1.5 Pro | LEGACY | → Gemini 2.5 Pro |
| ⚠️ Gemini 1.5 Flash | LEGACY | → Gemini 2.5 Flash |

### 🟡 Mistral AI — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ Devstral Small 1.1 | LEGACY · Superseded by Devstral Small 2 (Dec 2025) | → Devstral Small 2 ($0.10/$0.30, 256K ctx) |
| ⚠️ Devstral Medium | LEGACY · Superseded by Devstral 2 (Dec 2025) | → Devstral 2 ($0.40/$0.90) or Medium 3.5 |
| ⚠️ Mistral Small 3.2 24B | LEGACY · Superseded Mar 2026 | → Mistral Small 4 |
| ⚠️ Mistral Small 3.1 | LEGACY · Superseded Jun 2025 | → Mistral Small 4 |
| ⚠️ Mistral Large 2 (2407) | LEGACY | → Mistral Large 3 |
| ⚠️ Mistral Medium 3 (original) | LEGACY · Superseded Aug 2025 | → Mistral Medium 3.1 or Medium 3.5 |
| ⚠️ Codestral 2501 | LEGACY · Superseded Aug 2025 | → Codestral 2508 |
| ⚠️ Mixtral 8×7B (API) | LEGACY (still self-hostable) | → Mistral Medium 3.1 (API) |

---

## 🏷️ Price Change Log

| Date | Provider | Model | Change |
|---|---|---|---|
| 2026-05-21 | Google | **Gemini 3.5 Flash** | 🆕 ADDED — Released May 19, 2026 (Google I/O). New stable GA flagship. Standard: $1.50 input / $9.00 output per MTok; 1,048,576 token context; 65,536 max output; Thinking supported; Batch: $0.75/$4.50; Priority: $2.70/$16.20. Outperforms Gemini 3.1 Pro Preview on agentic and coding benchmarks (Terminal-Bench 2.1 76.2%, GDPval-AA 1656 Elo) at 25% lower input price. 4× faster than other frontier models. Default model in Gemini app, AI Mode in Search, and Google Antigravity. Source: ai.google.dev/gemini-api/docs/models/gemini-3.5-flash + blog.google, verified May 21, 2026. |
| 2026-05-21 | Google | **Gemini 3.1 Flash-Lite** (stable) | 🆕 ADDED — Stable GA version now available (`gemini-3.1-flash-lite`). Same pricing as preview: $0.25/$1.50 per MTok (standard); 1,048,576 context; 65,536 max output; Thinking supported; Knowledge cutoff January 2025. Source: ai.google.dev/gemini-api/docs/models/gemini-3.1-flash-lite, verified May 21, 2026. |
| 2026-05-21 | Google | **Gemini 2.0 Flash** | ⚠️ STATUS CHANGE — DEPRECATED. Official Gemini API pricing page confirms **shutdown June 1, 2026**. Previously listed as Active. Migrate to Gemini 2.5 Flash ($0.30/$2.50) or Gemini 3.5 Flash ($1.50/$9.00). Source: ai.google.dev/gemini-api/docs/pricing, verified May 21, 2026. |
| 2026-05-21 | OpenAI | **GPT-5.5** | ✏️ CORRECTION — Context window corrected **1,000,000 → 1,050,000 tokens**. Long-context pricing **added** (previously omitted): >272K input tokens triggers 2× input / 1.5× output for the full session ($10.00/$45.00 per MTok). GPT-5.5 is **not** flat-rate. Source: developers.openai.com/api/docs/models/gpt-5.5, verified May 21, 2026. |
| 2026-05-21 | Mistral | **Devstral Small 2** | 🆕 ADDED — Current active small coding agent model ($0.10/$0.30, 256K context, 24B params, ~58% SWE-bench, Apache 2.0). Replaces Devstral Small 1.1 ($0.07/$0.28, 128K context). Source: aipricing.guru/mistral-pricing/ (May 20, 2026), cloudprice.net. |
| 2026-05-21 | Mistral | **Devstral Small 1.1** | ⚠️ MOVED TO LEGACY — Superseded by Devstral Small 2. `devstral-small-latest` now routes to v2. |
| 2026-05-21 | Mistral | **Pixtral Large** | 🆕 DEDICATED CARD ADDED — $2.00/$6.00 per MTok, 128K context; multimodal flagship (vision + text); confirmed active model on aipricing.guru (May 20, 2026). Previously mentioned only as a line item — now has dedicated active model card. |
| 2026-05-21 | Anthropic | **All active models** | ✅ RE-VERIFIED — All Anthropic prices confirmed unchanged since 2026-05-18. No retirements or price changes detected. |
| 2026-05-18 | Anthropic | **Claude Sonnet 4 & Opus 4** | ✏️ CORRECTION — Previous cards listed retirement as June 15, 2026. Official Anthropic model deprecations page (docs.anthropic.com) confirms **both retired April 20, 2026**. All API calls return errors. |
| 2026-05-18 | Anthropic | **Claude Haiku 3.5** | ✏️ CORRECTION — Previously listed as Active. Official Anthropic deprecation docs confirm **retired February 19, 2026** on the Claude API. Moved to Legacy section. Migrate to Haiku 4.5. |
| 2026-05-18 | Anthropic | **Claude Haiku 3** | ✏️ DATE CORRECTION — Retirement date corrected from April 19-20, 2026 to **February 19, 2026** per official Anthropic deprecation docs. |
| 2026-05-18 | Anthropic | **Claude Sonnet 3.7** | ✏️ CORRECTION — Previously listed as DEPRECATED/API-accessible. Official Anthropic deprecation docs confirm **retired October 28, 2025**. All API calls return errors. |
| 2026-05-18 | Mistral | **Ministral 3B** | ✏️ PRICE CORRECTION — Input and output price corrected from $0.10/$0.10 to **$0.04/$0.04** per MTok, per aipricing.guru sourced directly from mistral.ai/pricing on 2026-05-16. README active table and model card updated. |
| 2026-05-11 | Anthropic | **Claude Opus 4.7** | ✏️ CORRECTION — Fast Mode ($30/$150) removed from Opus 4.7 model card. Per the official Anthropic pricing page (verified May 11, 2026), Fast Mode (beta) is available **only on Claude Opus 4.6**, not Opus 4.7. Previous card version incorrectly listed it for 4.7. |
| 2026-05-11 | All (Anthropic, OpenAI, Mistral) | **May 2026 pricing verification** | 🔍 Full re-verification against official sources. All active model prices confirmed accurate. |
| 2026-05-04 | Mistral | **Mistral Medium 3.5** | 🆕 ADDED — Released April 29, 2026. $1.50/$7.50 per MTok (confirmed official Mistral blog). 128B dense model; 256K context; vision + configurable reasoning + coding in one model; replaces Devstral 2 in Vibe CLI; open weights under modified MIT. SWE-Bench Verified 77.6%; τ³-Telecom 91.4%. |
| 2026-05-04 | Anthropic | **Claude Sonnet 4.5 1M context beta** | ❌ CONFIRMED RETIRED — The `context-1m-2025-08-07` beta header retired April 30, 2026 as scheduled. Requests exceeding 200K on Sonnet 4.5 now return errors. Migrate to Claude Sonnet 4.6 or Opus 4.6 (1M context at standard pricing, no header needed). |
| 2026-05-04 | Anthropic | **Claude Security** | 🆕 PLATFORM — Claude Security public beta announced for Enterprise customers (May 2026). Security operations and vulnerability analysis workflows. Billed at standard token rates. |
| 2026-05-04 | Mistral | **Mistral Medium 3.1** | ⚠️ NOTE — `mistral-medium-latest` alias may now route to Medium 3.5. Use explicit model ID `mistral-medium-3-1` if you need the $0.40/$2.00 tier. Medium 3.1 remains available for budget text workloads. |
| 2026-04-27 | Mistral | **Devstral 2 (2512)** | ✏️ CORRECTION — Output price updated $2.00 → **$0.90/MTok** (source: pricepertoken.com Apr 23, 2026). Context window corrected 128K → **256K** (source: Artificial Analysis). |
| 2026-04-27 | Mistral | **Magistral Medium 1.2 & Small 1.2** | ✏️ Context window confirmed as **128K tokens** (optimal performance below 40K per OpenRouter). Model ID corrected to `magistral-medium-2509` (Sep 2025 release). |
| 2026-04-27 | Mistral | **Mistral Small Creative** | 🆕 ADDED — Experimental creative writing model; $0.10/$0.30 per MTok; 33K context; released Dec 16, 2025. Not a general-purpose model. |
| 2026-04-25 | OpenAI | **GPT-5.5** | 🆕 LAUNCHED April 23-24, 2026 — $5.00/$30.00 per MTok (2× GPT-5.4 price); 1.05M context; first fully retrained base since GPT-4.5; natively omnimodal; AI Index score 60 (#1). |
| 2026-04-25 | OpenAI | **GPT-5.5 Pro** | 🆕 LAUNCHED April 24, 2026 — $30.00/$180.00 per MTok; 1M context. |
| 2026-04-25 | OpenAI | **o3-pro** | ✅ ADDED — $20.00/$80.00 per MTok; maximum reasoning depth; 200K context. |
| 2026-04-16 | Anthropic | **Claude Opus 4.7** | 🆕 LAUNCHED — $5/$25 per MTok. New: xhigh effort level, task budgets (beta), /ultrareview, 3.75MP vision, new tokenizer. SWE-bench Verified 87.6%. |
| 2026-04-12 | Google | **Gemini 3.1 Pro Preview** | ✅ Added — $2/$12 (≤200K), $4/$18 (>200K), 1M context |
| 2026-04-12 | OpenRouter | **gpt-oss-120b / DeepSeek V3.2 / Qwen3.6 Plus / Nemotron 3 / MiniMax M2.7 / Grok 4.1 Fast** | ✅ All Tier 2 picks added or updated |
| 2026-04-11 | Anthropic | **Claude Opus 4.6 / Sonnet 4.6** | ✅ Confirmed pricing and 1M context at standard pricing |
| 2026-04-11 | OpenAI | **GPT-5.4 family** | ✅ Confirmed launch Mar 5, 2026 · $2.50/$15 (short), $5/$22.50 (long ctx >272K) |
| 2026-04-11 | Mistral | **Mistral Large 3** | ✅ Confirmed $0.50/$1.50 at 256K context |

---

## ℹ️ Notes
- All prices are in **USD** and listed **per million tokens (MTok)**.
- **Batch API discounts (50%)** are available from Anthropic, OpenAI, and Google Gemini. Mistral does **not** currently offer a batch discount tier.
- **Prompt/context caching** discounts apply where noted. Mistral does **not** offer prompt caching.
- Enterprise/volume pricing is available from all providers on a negotiated basis.
- **OpenAI GPT-5.4 and GPT-5.5** use short context (<272K) and long context (>272K) pricing tiers. For GPT-5.5: long-context = 2× input / 1.5× output. ✏️ **Correction May 21, 2026:** GPT-5.5 is NOT flat-rate — previous versions of this file incorrectly stated otherwise.
- **OpenAI GPT-5.5 context window** is **1,050,000 tokens** (not 1,000,000). ✏️ Corrected May 21, 2026.
- **Google Gemini Pro** models (2.5 Pro, 3.1 Pro) double input cost for prompts >200K tokens.
- **Mistral** processes all API data in the EU by default — key compliance advantage for GDPR workloads.
- **Anthropic** offers US-only inference (data residency) at 1.1× pricing for models released after February 1, 2026.
- **Tier 2 OpenRouter Picks** use OpenRouter prices which are typically at or near direct provider API rates.
- ⚠️ Models marked **RETIRED** return API errors. Models marked **DEPRECATED** have a known retirement date or are actively phasing out but may still be API-accessible.
- 🔒 **Restricted models** (Mythos Preview, GPT-5.4-Cyber) are real models with no public API or general pricing — noted for awareness only.
- ⚠️ **Claude Opus 4.7 tokenizer change:** New tokenizer may produce up to 35% more tokens for the same text vs Opus 4.6. Per-token price is unchanged at $5/$25, but monitor per-request costs during migration.
- ⚠️ **Claude Opus 4.7 Fast Mode:** Fast Mode ($30/$150, 6×) is available on **Opus 4.6 only**, NOT Opus 4.7. Verified against official Anthropic pricing page May 11, 2026.
- ⚠️ **GPT-5.5 price increase:** $5/$30 is 2× GPT-5.4 ($2.50/$15) per token. Measure on your own workloads before migrating.
- 🆕 **Gemini 3.5 Flash (May 19, 2026):** New stable GA flagship; $1.50/$9.00 MTok standard; 1M context; outperforms 3.1 Pro Preview at lower cost; 4× faster than other frontier models. Gemini 3.5 Pro coming June 2026.
- ⚠️ **Gemini 2.0 Flash DEPRECATED:** Official shutdown **June 1, 2026**. Migrate to Gemini 2.5 Flash or 3.5 Flash immediately.
- 🆕 **Gemini 3.1 Flash-Lite (stable, May 2026):** Stable GA version now available; same $0.25/$1.50 pricing as preview; thinking supported.
- 🆕 **Mistral Medium 3.5 (Apr 29):** $1.50/$7.50 MTok; 128B dense merged model; vision + configurable reasoning + coding; replaces Devstral 2 in Vibe CLI; open weights (modified MIT).
- 🆕 **Pixtral Large:** $2.00/$6.00 MTok; Mistral's multimodal flagship; 128K context; vision + text. Dedicated card added May 21, 2026.
- 🆕 **Devstral Small 2 (Dec 2025):** $0.10/$0.30 MTok; 256K context; ~58% SWE-bench; replaces Devstral Small 1.1. Added to active table May 21, 2026.
- ❌ **Claude Sonnet 4.5 1M context beta retired April 30, 2026** — migrate to Sonnet 4.6 (1M context GA at standard pricing, no beta header).
- ✏️ **Anthropic retirement date corrections (May 18, 2026):** Sonnet 4 & Opus 4 retired April 20 (not June 15); Haiku 3 & Haiku 3.5 retired February 19 (not April); Sonnet 3.7 retired October 28, 2025. Source: docs.anthropic.com/en/docs/about-claude/model-deprecations.
- ✏️ **Ministral 3B price correction (May 18, 2026):** $0.04/$0.04 per MTok (was $0.10/$0.10). Source: mistral.ai/pricing via aipricing.guru, May 16, 2026.
