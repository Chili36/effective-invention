# 🤖 LLM Pricing Tracker

Up-to-date pricing and specifications for large language models from **Anthropic**, **OpenAI**, **Google Gemini**, **Mistral AI**, and top **OpenRouter picks**.

> **Last updated:** 2026-05-28 (refresh #16)
> **Sources:** Official provider pricing pages + third-party verification — scraped/verified on date above.

---

## 📋 Quick-Reference Index — Active Models

### 🟠 Tier 1 — Anthropic Claude

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Max Output | Availability |
|---|---|---|---|---|---|
| **Claude Opus 4.8** *(Current Flagship)* | $5.00 | $25.00 | **1M tokens** | 128k sync / 300k Batch | API, AWS Bedrock (Messages API), Vertex AI, MS Foundry (200k ctx) |
| **Claude Sonnet 4.6** | $3.00 | $15.00 | **1M tokens** | 64k sync / 300k Batch | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Haiku 4.5** | $1.00 | $5.00 | 200K tokens | 64k | API, AWS Bedrock (all regions), Vertex AI, MS Foundry |

> 💡 Batch API: 50% off · Prompt caching: up to 90% off
> ⚡ **Opus 4.8 Fast Mode:** 2× standard pricing ($10/$50) for up to 2.5× faster speeds
> 🧠 **Thinking:** Opus 4.8 = Adaptive only · Sonnet 4.6 = Adaptive + Extended · Haiku 4.5 = Extended only
> 🔒 Claude Mythos Preview (Project Glasswing) — restricted access only; no public API
> 🚨 **Opus 4.7 moved to Legacy (May 28, 2026)** — migrate to Opus 4.8 (same price, improved capabilities)

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

---

### 🟡 Tier 1 — Mistral AI

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Mistral Medium 3.5** 🆕 *(Apr 29, 2026)* | $1.50 | $7.50 | 256K tokens | API (Mistral AI Studio) |
| **Mistral Large 3 (2512)** | $0.50 | $1.50 | 256K tokens | API (Mistral AI Studio) |
| **Magistral Medium 1.2** | $2.00 | $5.00 | 128K tokens *(best <40K)* | API (Mistral AI Studio) |
| Mistral Medium 3.1 *(check alias routing)* | $0.40 | $2.00 | 131K tokens | API (Mistral AI Studio) |
| **Mistral Small 4** *(Mar 2026)* | $0.10 | $0.30 | **256K tokens** | API (Mistral AI Studio) |
| Codestral 2508 | $0.30 | $0.90 | 256K tokens | API (Mistral AI Studio) |
| **Devstral 2 (2512)** | $0.40 | $2.00 | 256K tokens | API (Mistral AI Studio) |
| **Devstral Small 2** | $0.10 | $0.30 | **256K tokens** | API (Mistral AI Studio) |
| Voxtral Small 24B | $0.004/min (audio) | $0.40 | 128K tokens | API (Mistral AI Studio) |
| Voxtral TTS | $0.016/1K chars | — | — | API (Mistral AI Studio) |
| Mistral Nemo | $0.15 | $0.15 | 128K tokens | API (Mistral AI Studio) |
| Ministral 3 14B | $0.20 | $0.20 | 256K tokens | API (Mistral AI Studio) |
| Ministral 3 8B | $0.15 | $0.15 | 256K tokens | API (Mistral AI Studio) |
| Ministral 3 3B | $0.10 | $0.10 | 556K tokens | API (Mistral AI Studio) |

> 💡 Batch API: 50% off (confirmed May 28, 2026) · EU data residency by default · Open-weight models (Apache 2.0/modified MIT) for self-hosting
> 🆕 **Mistral Medium 3.5** (Apr 29, 2026) — 128B dense flagship; $1.50/$7.50; 256K ctx; vision + configurable reasoning + coding in one model
> ✏️ **May 28, 2026 price updates:** Devstral 2 output corrected to $2.00/MTok · Pixtral Large → Legacy · Mistral Small 4 reduced to $0.10/$0.30 · Ministral 8B raised to $0.15/$0.15 · Ministral 3B updated to $0.10/$0.10
> ⚠️ **`mistral-medium-latest` alias may now route to Medium 3.5** — verify your version via API response `model` field

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
| Anthropic | 1 | [anthropic.md](./anthropic.md) | Full model cards incl. Opus 4.8 (new flagship), max output corrections, thinking capabilities, knowledge cutoffs, deprecation dates |
| OpenAI | 1 | [openai.md](./openai.md) | Full model cards incl. context tiers (GPT-5.5 + GPT-5.4), reasoning models, batch pricing |
| Google Gemini | 1 | [gemini.md](./gemini.md) | Full model cards incl. Gemini 3.5 Flash (new flagship), 3.1 Flash-Lite stable GA, 2.0 Flash deprecation |
| Mistral AI | 1 | [mistral.md](./mistral.md) | Full model cards incl. Medium 3.5, price corrections (Devstral 2, Small 4, Ministral), Pixtral Large legacy |
| OpenRouter Picks | 2 | [openrouter-picks.md](./openrouter-picks.md) | One best-performing model per Tier 2 provider, all via OpenRouter |

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new deployments.

### 🟠 Anthropic — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ Claude Opus 4.7 | **LEGACY** · Moved to Legacy section (May 28, 2026); still API-accessible; No Fast Mode | $5.00 | $25.00 | → Claude Opus 4.8 (same price, improved performance, Fast Mode available) |
| ⚠️ Claude Opus 4.6 | **LEGACY** · Moved to Legacy section (May 25, 2026); still API-accessible; Fast Mode $30/$150 (6×) | $5.00 | $25.00 | → Claude Opus 4.8 (same price, cheaper Fast Mode at 2×) |
| ⚠️ Claude Sonnet 4.5 | **LEGACY** · Moved to Legacy section (May 25, 2026); 1M beta RETIRED Apr 30, 2026 | $3.00 | $15.00 | → Claude Sonnet 4.6 (same price, 1M context) |
| ⚠️ Claude Opus 4.5 | **LEGACY** · Moved to Legacy section (May 25, 2026); still API-accessible | $5.00 | $25.00 | → Claude Opus 4.8 (same price, 1M context, 128k output) |
| ⚠️ Claude Opus 4.1 | LEGACY | $15.00 | $75.00 | → Claude Opus 4.8 (67% cheaper) |
| ⚠️ Claude Sonnet 4 | **RETIRED April 20, 2026 ❌ API ERRORS** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude Opus 4 | **RETIRED April 20, 2026 ❌ API ERRORS** | $15.00 | $75.00 | → Claude Opus 4.8 |
| ⚠️ Claude Haiku 3.5 | **RETIRED February 19, 2026 ❌ API ERRORS** | $0.80 | $4.00 | → Claude Haiku 4.5 |
| ⚠️ Claude Haiku 3 | **RETIRED February 19, 2026 ❌ API ERRORS** | $0.25 | $1.25 | → Claude Haiku 4.5 |
| ⚠️ Claude Sonnet 3.7 | **RETIRED October 28, 2025 ❌ API ERRORS** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 3 Opus | **DEPRECATED** Jan 2026 — available by request for paying customers | $15.00 | $75.00 | → Claude Opus 4.8 |
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
| ⚠️ Pixtral Large | **LEGACY** · Deprecated per docs.mistral.ai (May 2026); removed from pricing page | → Mistral Medium 3.5 ($1.50/$7.50, vision + reasoning) or Mistral Small 4 ($0.10/$0.30, vision) |
| ⚠️ Magistral Small 1.2 | **LEGACY** · Deprecated per docs.mistral.ai (May 25, 2026) | → Mistral Small 4 with `reasoning_effort=high` ($0.10/$0.30) |
| ⚠️ Mistral Small Creative | **LEGACY** · Labs model deprecated per docs.mistral.ai (May 25, 2026) | → Mistral Small 4 ($0.10/$0.30) |
| ⚠️ Devstral Small 1.1 | LEGACY · Superseded by Devstral Small 2 (Dec 2025) | → Devstral Small 2 ($0.10/$0.30, 256K ctx) |
| ⚠️ Devstral Medium | LEGACY · Superseded by Devstral 2 (Dec 2025) | → Devstral 2 ($0.40/$2.00) or Medium 3.5 |
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
| 2026-05-28 | Anthropic | **Claude Opus 4.8** | 🚨 LAUNCHED — New active flagship. Model ID `claude-opus-4-8`. $5/$25 per MTok (same as Opus 4.7). Fast Mode: 2× standard ($10/$50) for up to 2.5× speed. Context: 1M tokens (200k on MS Foundry). Max output: 128k sync / 300k Batch. Adaptive thinking ✅, Extended thinking ❌. Source: `platform.claude.com/docs/en/about-claude/models/overview`, verified May 28, 2026. |
| 2026-05-28 | Anthropic | **Claude Opus 4.7** | ⚠️ STATUS CHANGE → LEGACY — Official Anthropic pricing page now lists Opus 4.7 in "Legacy models" section. Model still API-accessible at $5/$25. Migrate to Claude Opus 4.8. |
| 2026-05-28 | Mistral | **Devstral 2 (2512)** | ✏️ PRICE CORRECTION — Output corrected from $0.90 → **$2.00 per MTok**. Official Mistral launch announcement (`mistral.ai/news/devstral-2-vibe-cli`) stated $0.40/$2.00 from the start; the $0.90 figure was incorrectly inferred during the free launch period. OpenRouter confirms $0.40/$2.00. API alias updated: `devstral-medium-latest`. |
| 2026-05-28 | Mistral | **Pixtral Large** | ⚠️ MOVED TO LEGACY — No longer listed on `mistral.ai/pricing`. Confirmed in `docs.mistral.ai` legacy table as `pixtral-large-2411`. Migrate to Mistral Medium 3.5 ($1.50/$7.50) for vision + coding tasks. |
| 2026-05-28 | Mistral | **Mistral Small 4** | ✏️ PRICE UPDATE — Input: $0.15 → **$0.10** / Output: $0.60 → **$0.30** per MTok. Per official `mistral.ai/pricing` page (verified May 28, 2026). |
| 2026-05-28 | Mistral | **Ministral 3B** | ✏️ PRICE UPDATE — $0.04/$0.04 → **$0.10/$0.10** per MTok. Per official `mistral.ai/pricing` page (verified May 28, 2026). Note: This reverts the May 18 correction to $0.04 — official page now shows $0.10/$0.10. |
| 2026-05-28 | Mistral | **Ministral 8B** | ✏️ PRICE UPDATE — $0.10/$0.10 → **$0.15/$0.15** per MTok. Per official `mistral.ai/pricing` page (verified May 28, 2026). |
| 2026-05-28 | Mistral | **Voxtral Small** | ✏️ UPDATE — Audio input pricing clarified: $0.004/min (audio) or $0.10/MTok (text). Output updated $0.30 → **$0.40/MTok**. Per official `mistral.ai/pricing` page. |
| 2026-05-28 | Mistral | **Batch API discount** | 🆕 CONFIRMED — Mistral offers 50% batch processing discount (per pricing page FAQ: "Batch processing gets a 50% discount"). Previous card stated no batch discount available — this was incorrect. |
| 2026-05-28 | OpenAI | **All active models** | ✅ RE-VERIFIED — All OpenAI prices confirmed unchanged since May 25, 2026. Source: openai.com/api/pricing/, developers.openai.com/api/docs/pricing. |
| 2026-05-25 | Anthropic | **Claude Opus 4.7** | ✏️ CORRECTION — Max output corrected **32k → 128k tokens** (sync). Per official API docs (`platform.claude.com/docs/en/about-claude/models/overview`, verified May 25, 2026). Price unchanged at $5/$25. |
| 2026-05-25 | Anthropic | **Claude Sonnet 4.6** | ✏️ CORRECTION — Max output corrected **16k → 64k tokens** (sync). Source: official API docs, verified May 25, 2026. Price unchanged at $3/$15. |
| 2026-05-25 | Anthropic | **Claude Haiku 4.5** | ✏️ CORRECTION — Max output corrected **8k → 64k tokens**. Source: official API docs, verified May 25, 2026. Price unchanged at $1/$5. |
| 2026-05-25 | Anthropic | **Claude Opus 4.6** | ⚠️ STATUS CHANGE → LEGACY — Official Anthropic pricing page lists Opus 4.6 in the "Legacy models" section. Model still API-accessible at $5/$25. Fast Mode ($30/$150) remains available on this model. |
| 2026-05-25 | Anthropic | **Claude Sonnet 4.5** | ⚠️ STATUS CHANGE → LEGACY — Official Anthropic pricing page lists Sonnet 4.5 in "Legacy models" section. 1M context beta was retired April 30, 2026. |
| 2026-05-25 | Anthropic | **Claude Opus 4.5** | ⚠️ STATUS CHANGE → LEGACY — Official Anthropic pricing page lists Opus 4.5 in "Legacy models" section. Still API-accessible at $5/$25. |
| 2026-05-25 | Mistral | **Magistral Small 1.2** | ⚠️ MOVED TO LEGACY — `docs.mistral.ai/models/overview` lists `magistral-small-2509` in the deprecated/legacy model table. |
| 2026-05-25 | Mistral | **Mistral Small Creative** | ⚠️ MOVED TO LEGACY — `docs.mistral.ai/models/overview` lists `labs-mistral-small-creative` in deprecated table. |
| 2026-05-21 | Google | **Gemini 3.5 Flash** | 🆕 ADDED — Released May 19, 2026 (Google I/O). New stable GA flagship. Standard: $1.50 input / $9.00 output per MTok; 1M context. |
| 2026-05-21 | Google | **Gemini 2.0 Flash** | ⚠️ STATUS CHANGE — DEPRECATED. Official shutdown June 1, 2026. |
| 2026-05-18 | Anthropic | **Claude Sonnet 4 & Opus 4** | ✏️ CORRECTION — Retirement date corrected to **April 20, 2026** (was June 15). |
| 2026-05-18 | Mistral | **Ministral 3B** | ✏️ PRICE CORRECTION — Was $0.10/$0.10, corrected to $0.04/$0.04 per aipricing.guru scrape (May 16). Now reverted back to $0.10/$0.10 per official page (May 28). |
| 2026-05-04 | Mistral | **Mistral Medium 3.5** | 🆕 ADDED — Released April 29, 2026. $1.50/$7.50 per MTok. 128B dense model; 256K context; vision + configurable reasoning + coding. |
| 2026-04-25 | OpenAI | **GPT-5.5 / GPT-5.5 Pro** | 🆕 LAUNCHED April 23-24, 2026. $5.00/$30.00 / $30.00/$180.00 per MTok. |
| 2026-04-16 | Anthropic | **Claude Opus 4.7** | 🆕 LAUNCHED — $5/$25 per MTok. SWE-bench Verified 87.6%. |

---

## ℹ️ Notes
- All prices are in **USD** and listed **per million tokens (MTok)**.
- **Batch API discounts (50%)** are available from Anthropic, OpenAI, Google Gemini, and **Mistral** (confirmed May 28, 2026). Previous tracking incorrectly noted Mistral had no batch discount.
- **Prompt/context caching** discounts apply where noted. Mistral does **not** offer prompt caching.
- Enterprise/volume pricing is available from all providers on a negotiated basis.
- **OpenAI GPT-5.4 and GPT-5.5** use short context (<272K) and long context (>272K) pricing tiers. For GPT-5.5: long-context = 2× input / 1.5× output.
- **Google Gemini Pro** models (2.5 Pro, 3.1 Pro) double input cost for prompts >200K tokens.
- **Mistral** processes all API data in the EU by default — key compliance advantage for GDPR workloads.
- **Anthropic** offers US-only inference (data residency) at 1.1× pricing for models released after February 1, 2026.
- **Tier 2 OpenRouter Picks** use OpenRouter prices which are typically at or near direct provider API rates.
- ⚠️ Models marked **RETIRED** return API errors. Models marked **LEGACY** are still API-accessible but listed in the provider's legacy/deprecated section.
- 🔒 **Restricted models** (Mythos Preview, GPT-5.4-Cyber) have no public API or general pricing — noted for awareness only.
- 🚨 **Anthropic flagship change (May 28, 2026):** Claude Opus 4.8 is now the active flagship. Opus 4.7 moved to Legacy. Same price ($5/$25). Fast Mode returns on Opus 4.8 at 2× standard ($10/$50, up to 2.5× faster).
- ✏️ **Mistral price corrections (May 28, 2026):** Devstral 2 output $0.90 → $2.00 (was incorrect from free-period confusion); Pixtral Large deprecated; Mistral Small 4 $0.15/$0.60 → $0.10/$0.30; Ministral 8B $0.10 → $0.15; Ministral 3B $0.04 → $0.10.
- 🆕 **Mistral batch discount confirmed (May 28, 2026):** 50% off for batch processing — previous tracking was incorrect in stating Mistral had no batch discount.
- ⚠️ **Gemini 2.0 Flash DEPRECATED:** Official shutdown **June 1, 2026**.
