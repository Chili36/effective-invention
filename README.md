# 🤖 LLM Pricing Tracker

Up-to-date pricing and specifications for large language models from **Anthropic**, **OpenAI**, **Google Gemini**, **Mistral AI**, and top **OpenRouter picks**.

> **Last updated:** 2026-04-15 (refresh #6)  
> **Sources:** Official provider pricing pages + third-party verification — scraped/verified on date above.

---

## 📋 Quick-Reference Index — Active Models

### 🟠 Tier 1 — Anthropic Claude

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Claude Opus 4.6** | $5.00 | $25.00 | **1M tokens** | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Sonnet 4.6** | $3.00 | $15.00 | **1M tokens** | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Haiku 4.5** | $1.00 | $5.00 | 200K tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Opus 4.5 | $5.00 | $25.00 | 200K tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Sonnet 4.5 | $3.00 | $15.00 | 200K tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Haiku 3.5 *(prev-gen, still active)* | $0.80 | $4.00 | 128K tokens | API, AWS Bedrock, Vertex AI |

> 💡 Batch API: 50% off · Prompt caching: up to 90% off · Opus 4.6 Fast Mode: $30/$150 (6× base)  
> ⚠️ Claude Haiku 3 retiring **April 19, 2026** (4 days) — migrate to Haiku 4.5 immediately  
> 🔒 Claude Mythos Preview announced April 7 — restricted access only (Project Glasswing); no public API  
> 🆙 Claude Opus 4.7 reportedly launching this week — model card will be added upon release

---

### 🟢 Tier 1 — OpenAI (Proprietary)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|---|
| **GPT-5.4** *(short ctx <270K)* | $2.50 | $0.25 | $15.00 | 1.05M tokens | API |
| **GPT-5.4** *(long ctx >270K)* | $5.00 | $0.50 | $22.50 | 1.05M tokens | API |
| **GPT-5.4 Pro** | $30.00 | — | $180.00 | 1.05M tokens | API |
| **GPT-5.4 mini** | $0.75 | $0.075 | $4.50 | 400K tokens | API |
| **GPT-5.4 nano** | $0.20 | $0.020 | $1.25 | 400K tokens | API |
| GPT-4.1 | $2.00 | $0.50 | $8.00 | 1.04M tokens | API |
| **GPT-4.1 mini** | $0.40 | $0.10 | $1.60 | 1.00M tokens | API |
| GPT-4.1 nano | $0.10 | — | $0.40 | 1M+ tokens | API |
| o3 *(reasoning)* | $2.00 | $0.50 | $8.00 | 200K tokens | API |
| o4-mini *(reasoning)* | $1.10 | $0.275 | $4.40 | 200K tokens | API |

> 💡 Batch API: 50% off all models · Cached inputs: 50–90% off · Regional processing: +10% on GPT-5.4 family  
> 🔒 GPT-5.4-Cyber announced April 14 — limited vetted access only; no public API pricing

---

### 🔵 Tier 1 — Google Gemini

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Notes |
|---|---|---|---|---|
| **Gemini 3.1 Pro Preview** | $2.00 / $4.00* | $12.00 / $18.00* | **1M tokens** | *Tiered at >200K; Preview |
| **Gemini 3.1 Flash-Lite Preview** | $0.25 | $1.50 | **1M tokens** | Preview |
| **Gemini 2.5 Pro** | $1.25 / $2.50* | $10.00 / $15.00* | **1M tokens** | *Tiered at >200K; GA |
| **Gemini 2.5 Flash** | $0.30 | $2.50 | **1M tokens** | GA; optional thinking mode |
| **Gemini 2.5 Flash-Lite** | $0.10 | $0.40 | **1M tokens** | GA; cheapest Gemini |
| Gemini 2.0 Flash | $0.10 | $0.40 | 1M tokens | Active; prev-gen |

> 💡 Batch API: 50% off · Context caching: 90% off repeated prefixes · Free tier via AI Studio · Pro models: double input cost for prompts >200K

---

### 🟡 Tier 1 — Mistral AI

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Mistral Large 3 (2512)** | $0.50 | $1.50 | 262K tokens | API (Mistral AI Studio) |
| Mistral Medium 3.1 | $0.40 | $2.00 | 131K tokens | API (Mistral AI Studio) |
| **Mistral Small 4** *(Mar 2026)* | $0.15 | ~$0.60* | 128K tokens | API (Mistral AI Studio) |
| Codestral 2508 | $0.30 | $0.90 | 128K tokens | API (Mistral AI Studio) |
| Devstral 2 | $0.40 | $2.00 | 128K tokens | API (Mistral AI Studio) |
| Devstral Small 1.1 | $0.07 | $0.28 | 128K tokens | API (Mistral AI Studio) |
| Voxtral Small 24B | $0.10 | $0.30 | 128K tokens | API (Mistral AI Studio) |
| Mistral Nemo | $0.15 | $0.15 | 128K tokens | API (Mistral AI Studio) |
| Ministral 14B | $0.20 | $0.20 | 256K tokens | API (Mistral AI Studio) |
| Ministral 8B | $0.10 | $0.10 | 256K tokens | API (Mistral AI Studio) |
| Ministral 3B | $0.10 | $0.10 | 556K tokens | API (Mistral AI Studio) |

> 💡 EU data residency by default · Free experimentation tier · Open-weight models (Apache 2.0) for self-hosting  
> *Mistral Small 4 output pricing subject to verification on official Mistral console (source: flowlyn.com Apr 2026)

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
| Anthropic | 1 | [anthropic.md](./anthropic.md) | Full model cards incl. caching, batch, fast mode, deprecation dates |
| OpenAI | 1 | [openai.md](./openai.md) | Full model cards incl. context tiers, reasoning models, batch pricing |
| Google Gemini | 1 | [gemini.md](./gemini.md) | Full model cards incl. context tiers, thinking tokens, free tier |
| Mistral AI | 1 | [mistral.md](./mistral.md) | Full model cards incl. open-weight models, Le Chat plans, EU compliance |
| OpenRouter Picks | 2 | [openrouter-picks.md](./openrouter-picks.md) | One best-performing model per Tier 2 provider, all via OpenRouter |

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new deployments.

### 🟠 Anthropic — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ Claude Sonnet 4 | **DEPRECATED · 🚨 Retiring Jun 15, 2026** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude Opus 4.1 | LEGACY | $15.00 | $75.00 | → Claude Opus 4.6 (67% cheaper) |
| ⚠️ Claude Opus 4 | **DEPRECATED · 🚨 Retiring Jun 15, 2026** | $15.00 | $75.00 | → Claude Opus 4.6 |
| ⚠️ Claude Haiku 3 | **DEPRECATED · 🚨 Retiring Apr 19, 2026 (4 days!)** | $0.25 | $1.25 | → Claude Haiku 4.5 |
| ⚠️ Claude Sonnet 3.7 | **DEPRECATED** (API still accessible; no new projects) | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 3 Opus | **DEPRECATED** (API still accessible; phasing out) | $15.00 | $75.00 | → Claude Opus 4.6 |
| ⚠️ Claude 3.5 Sonnet | **RETIRED** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 2.x | **RETIRED** | ~$8.00 | ~$24.00 | → Claude Sonnet 4.6 |

### 🟢 OpenAI — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ GPT-5.3 / Codex | LEGACY · Phasing out Jun 2026 | $1.75 | $14.00 | → GPT-5.4 |
| ⚠️ GPT-5.2 | LEGACY · Retiring Jun 2026 | $1.75 | $14.00 | → GPT-5.4 |
| ⚠️ GPT-5.1 | **RETIRED March 11, 2026** | — | — | → GPT-5.4 / GPT-5.3 |
| ⚠️ GPT-4o | LEGACY | $2.50 | $10.00 | → GPT-4.1 (cheaper, 1M ctx) |
| ⚠️ GPT-4o mini | LEGACY | $0.15 | $0.60 | → GPT-5.4 nano or GPT-4.1 nano |
| ⚠️ o1 | LEGACY (very expensive) | $15.00 | $60.00 | → o3 (87% cheaper) |
| ⚠️ GPT-4 Turbo | **RETIRED** | — | — | → GPT-4.1 |
| ⚠️ GPT-3.5 Turbo | **RETIRED** | — | — | → GPT-4.1 nano |

### 🔵 Google Gemini — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ Gemini 3 Pro Preview | **RETIRED** March 9, 2026 | → Gemini 3.1 Pro Preview |
| ⚠️ Gemini 2.0 Flash-Lite | **DEPRECATED · Shutdown June 1, 2026** | → Gemini 2.5 Flash-Lite |
| ⚠️ Gemini 1.5 Pro | LEGACY | → Gemini 2.5 Pro |
| ⚠️ Gemini 1.5 Flash | LEGACY | → Gemini 2.5 Flash |

### 🟡 Mistral AI — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ Mistral Small 3.2 24B | LEGACY · Superseded Mar 2026 | → Mistral Small 4 |
| ⚠️ Mistral Small 3.1 | LEGACY · Superseded Jun 2025 | → Mistral Small 4 |
| ⚠️ Mistral Large 2 (2407) | LEGACY | → Mistral Large 3 |
| ⚠️ Mistral Medium 3 (original) | LEGACY · Superseded Aug 2025 | → Mistral Medium 3.1 |
| ⚠️ Codestral 2501 | LEGACY · Superseded Aug 2025 | → Codestral 2508 |
| ⚠️ Mixtral 8×7B (API) | LEGACY (still self-hostable) | → Mistral Medium 3.1 (API) |

---

## 🏷️ Price Change Log

| Date | Provider | Model | Change |
|---|---|---|---|
| 2026-04-15 | Anthropic | **Claude Sonnet 4** | ⚠️ DEPRECATED — Retirement scheduled June 15, 2026. Migrate to Sonnet 4.6. |
| 2026-04-15 | Anthropic | **Claude Opus 4** | ⚠️ DEPRECATED — Retirement scheduled June 15, 2026. Migrate to Opus 4.6. |
| 2026-04-15 | Anthropic | **Claude Haiku 3** | ⚠️ IMMINENT — Retirement April 19, 2026 is now 4 days away. Migrate to Haiku 4.5 immediately. |
| 2026-04-15 | Anthropic | **Claude Mythos Preview** | 🔒 Announced April 7 — restricted access only (Project Glasswing cybersecurity initiative). No public API. |
| 2026-04-15 | OpenAI | **GPT-5.4-Cyber** | 🔒 Announced April 14 — limited vetted access only. Not available via public API. |
| 2026-04-15 | OpenAI | **GPT-5.1** | ⚠️ RETIRED March 11, 2026. Added to legacy section. |
| 2026-04-15 | Mistral | **Mistral Small 4** | ✅ ADDED — Released March 3, 2026; $0.15/M input; now current `mistral-small-latest` |
| 2026-04-15 | Mistral | **Mistral Small 3.2 24B** | ⚠️ MOVED TO LEGACY — Superseded by Small 4 ($0.07/$0.20, released Jun 2025) |
| 2026-04-15 | Mistral | **Mistral Small 3.1** | ⚠️ MOVED TO LEGACY — Superseded by Small 3.2 and then Small 4 |
| 2026-04-15 | Mistral | **Codestral 2508** | ✅ UPDATED — Version 2508 (Aug 2025) at $0.30/$0.90; 70% cheaper than old Codestral 2501 ($1.00/$3.00) |
| 2026-04-15 | Mistral | **Mistral Medium 3.1** | ✅ ADDED — August 2025 update to the Medium tier; $0.40/$2.00 |
| 2026-04-15 | Mistral | **Voxtral Small 24B** | ✅ ADDED — Audio/speech model (Oct 2025); $0.10/$0.30 |
| 2026-04-15 | Mistral | **Devstral Small 1.1** | ✅ ADDED — Budget coding agent (Jul 2025); $0.07/$0.28 |
| 2026-04-13 | Anthropic | **Claude Haiku 3.5** | ✏️ CORRECTED — Restored to Active ($0.80/$4); was incorrectly marked RETIRED. Official pricing page confirms still accessible. |
| 2026-04-13 | Anthropic | **Claude Sonnet 3.7** | ✏️ CORRECTED — Status updated to DEPRECATED (not RETIRED; API still accessible per official pricing page). |
| 2026-04-13 | Anthropic | **Claude 3 Opus** | ✏️ CORRECTED — Status updated to DEPRECATED (not RETIRED; still listed on official pricing page). |
| 2026-04-13 | OpenAI | **GPT-4.1 mini** | ✅ ADDED — $0.40/$1.60 per MTok; 1M context; bridges gap between GPT-4.1 nano and GPT-4.1. |
| 2026-04-13 | Mistral | **Le Chat Team plan** | ✏️ CORRECTED — $24.99/user/month (was incorrectly listed as ~$20K/month enterprise). Verified on mistral.ai/pricing. |
| 2026-04-12 | Google | **Gemini 3.1 Pro Preview** | ✅ Added — $2/$12 (≤200K), $4/$18 (>200K), 1M context — replaced Gemini 3 Pro Preview |
| 2026-04-12 | Google | **Gemini 3.1 Flash-Lite Preview** | ✅ Added — $0.25/$1.50, 1M context |
| 2026-04-12 | Google | **Gemini 2.5 Pro / Flash / Flash-Lite** | ✅ Confirmed GA pricing — $1.25/$10, $0.30/$2.50, $0.10/$0.40 |
| 2026-04-12 | Google | **Gemini 2.0 Flash-Lite** | ⚠️ DEPRECATED — shutting down June 1, 2026 |
| 2026-04-12 | Google | **Gemini 3 Pro Preview** | ⚠️ RETIRED March 9, 2026 |
| 2026-04-12 | OpenRouter | **gpt-oss-120b** | ✅ Added — $0.039/$0.19, 131K context |
| 2026-04-12 | OpenRouter | **DeepSeek V3.2** | ✅ Added — $0.26/$0.38, 163K context |
| 2026-04-12 | OpenRouter | **Qwen3.6 Plus** | ✅ Added — free preview (April 2026); paid pricing TBD |
| 2026-04-12 | OpenRouter | **Nemotron 3 Super 120B** | ✅ Added — $0.10/$0.50, 262K context |
| 2026-04-12 | OpenRouter | **MiniMax M2.7** | ✅ Added — $0.30/$1.20, 205K context |
| 2026-04-12 | OpenRouter | **Grok 4.1 Fast** | ✅ Added — $0.20/$0.50, 2M context |
| 2026-04-11 | Anthropic | **Claude Opus 4.6** | ✅ Confirmed $5/$25 · 1M context at standard pricing · Fast Mode $30/$150 |
| 2026-04-11 | Anthropic | **Claude Sonnet 4.6** | ✅ Confirmed $3/$15 · 1M context standard |
| 2026-04-11 | Anthropic | **Claude Haiku 3** | ⚠️ DEPRECATION CONFIRMED — Retiring April 19, 2026 |
| 2026-04-11 | OpenAI | **GPT-5.4 family** | ✅ Confirmed launch Mar 5, 2026 · $2.50/$15 (short), $5/$22.50 (long ctx >270K) |
| 2026-04-11 | OpenAI | **GPT-5.4 mini** | ✅ Confirmed $0.75/$4.50 (launched Mar 17, 2026) |
| 2026-04-11 | OpenAI | **GPT-5.4 nano** | ✅ Confirmed $0.20/$1.25 |
| 2026-04-11 | Mistral | **Mistral Large 3** | ✅ Confirmed $0.50/$1.50 at 262K context |

---

## ℹ️ Notes
- All prices are in **USD** and listed **per million tokens (MTok)**.
- **Batch API discounts (50%)** are available from Anthropic, OpenAI, and Google Gemini. Mistral does **not** currently offer a batch discount tier.
- **Prompt/context caching** discounts apply where noted. Mistral does **not** offer prompt caching.
- Enterprise/volume pricing is available from all providers on a negotiated basis.
- **OpenAI GPT-5.4** uses short context (<270K) and long context (>270K) pricing tiers.
- **Google Gemini Pro** models (2.5 Pro, 3.1 Pro) double input cost for prompts >200K tokens.
- **Mistral** processes all API data in the EU by default — key compliance advantage for GDPR workloads.
- **Anthropic** offers US-only inference (data residency) at 1.1× pricing for models released after February 1, 2026.
- **Tier 2 OpenRouter Picks** use OpenRouter prices which are typically at or near direct provider API rates.
- ⚠️ Models marked **RETIRED** return API errors. Models marked **DEPRECATED** have a known retirement date or are actively phasing out but may still be API-accessible.
- ✏️ **Correction policy:** When verified data from official pricing pages contradicts a prior entry, the old entry is corrected and logged in the Price Change Log above.
- 🔒 **Restricted models** (Mythos Preview, GPT-5.4-Cyber) are real models with no public API or general pricing — noted for awareness only.
