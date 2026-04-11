# 🤖 LLM Pricing Tracker

Up-to-date pricing and specifications for large language models from **Anthropic**, **OpenAI**, and **Mistral AI**.

> **Last updated:** 2026-04-11 (refresh #3)  
> **Sources:** Official provider pricing pages + third-party verification — scraped/verified on date above.

---

## 📋 Quick-Reference Index — Active Models

### 🟠 Anthropic — Claude Models

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Claude Opus 4.6** | $5.00 | $25.00 | **1M tokens** (standard) | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Sonnet 4.6** | $3.00 | $15.00 | **1M tokens** (standard) | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Haiku 4.5** | $1.00 | $5.00 | 200K tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Opus 4.5 | $5.00 | $25.00 | 200K tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Sonnet 4.5 | $3.00 | $15.00 | 200K tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Sonnet 4 | $3.00 | $15.00 | 200K tokens | API, AWS Bedrock, Vertex AI |

> 💡 Batch API: 50% off · Prompt caching: up to 90% off · Opus 4.6 Fast Mode: $30/$150 (6× base)

---

### 🟢 OpenAI — Models

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|---|
| **GPT-5.4** *(short ctx <270K)* | $2.50 | $0.25 | $15.00 | 1.05M tokens | API |
| **GPT-5.4** *(long ctx >270K)* | $5.00 | $0.50 | $22.50 | 1.05M tokens | API |
| **GPT-5.4 Pro** | $30.00 | — | $180.00 | 1.05M tokens | API |
| **GPT-5.4 mini** | $0.75 | $0.075 | $4.50 | 400K tokens | API |
| **GPT-5.4 nano** | $0.20 | $0.020 | $1.25 | 400K tokens | API |
| GPT-4.1 | $2.00 | $0.50 | $8.00 | 1.04M tokens | API |
| GPT-4.1 nano | $0.10 | — | $0.40 | 1M+ tokens | API |
| o3 *(reasoning)* | $2.00 | $0.50 | $8.00 | 200K tokens | API |
| o4-mini *(reasoning)* | $1.10 | $0.275 | $4.40 | 200K tokens | API |

> 💡 Batch API: 50% off all models · Cached inputs: 50–90% off · Regional processing: +10% on GPT-5.4 family

---

### 🔵 Mistral AI — Models

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Mistral Large 3 (2512)** | $0.50 | $1.50 | 262K tokens | API (Mistral AI Studio) |
| Mistral Medium 3 | $0.40 | $2.00 | 131K tokens | API (Mistral AI Studio) |
| **Mistral Small 3.1** | $0.20 | $0.60 | 128K tokens | API (Mistral AI Studio) |
| Codestral | $1.00 | $3.00 | 128K tokens | API (Mistral AI Studio) |
| Mistral Nemo | $0.15 | $0.15 | 128K tokens | API (Mistral AI Studio) |
| Ministral 14B | $0.20 | $0.20 | 256K tokens | API (Mistral AI Studio) |
| Ministral 8B | $0.10 | $0.10 | 256K tokens | API (Mistral AI Studio) |
| Ministral 3B | $0.10 | $0.10 | 556K tokens | API (Mistral AI Studio) |

> 💡 EU data residency by default · Free experimentation tier (no CC required) · Open-weight models (Apache 2.0) available for self-hosting

---

## 📁 Model Card Files

| Provider | File | Description |
|---|---|---|
| Anthropic | [anthropic.md](./anthropic.md) | Full model cards incl. caching, batch, fast mode, deprecation dates |
| OpenAI | [openai.md](./openai.md) | Full model cards incl. context tiers, reasoning models, batch pricing |
| Mistral AI | [mistral.md](./mistral.md) | Full model cards incl. open-weight models, Le Chat plans, EU compliance |

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new deployments. Retire or migrate ASAP.

### 🟠 Anthropic — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ Claude Opus 4.1 | LEGACY | $15.00 | $75.00 | → Claude Opus 4.6 (67% cheaper) |
| ⚠️ Claude Opus 4 | LEGACY | $15.00 | $75.00 | → Claude Opus 4.6 |
| ⚠️ Claude Haiku 3 | **DEPRECATED · Retiring Apr 19, 2026** | $0.25 | $1.25 | → Claude Haiku 4.5 |
| ⚠️ Claude Haiku 3.5 | **RETIRED** (API returns errors) | $0.80 | $4.00 | → Claude Haiku 4.5 |
| ⚠️ Claude Sonnet 3.7 | **RETIRED** Feb 19, 2026 | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 3 Opus | **RETIRED** Jan 5, 2026 | $15.00 | $75.00 | → Claude Opus 4.6 |
| ⚠️ Claude 3.5 Sonnet | **RETIRED** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 2.x | **RETIRED** | ~$8.00 | ~$24.00 | → Claude Sonnet 4.6 |

### 🟢 OpenAI — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ GPT-5.3 / Codex | LEGACY · Phasing out Jun 2026 | $1.75 | $14.00 | → GPT-5.4 |
| ⚠️ GPT-5.2 | LEGACY · Retiring Jun 2026 | $1.75 | $14.00 | → GPT-5.4 |
| ⚠️ GPT-4o | LEGACY | $2.50 | $10.00 | → GPT-4.1 (cheaper, 1M ctx) |
| ⚠️ GPT-4o mini | LEGACY | $0.15 | $0.60 | → GPT-5.4 nano or GPT-4.1 nano |
| ⚠️ o1 | LEGACY (very expensive) | $15.00 | $60.00 | → o3 (87% cheaper) |
| ⚠️ GPT-4 Turbo | **RETIRED** | — | — | → GPT-4.1 |
| ⚠️ GPT-3.5 Turbo | **RETIRED** | — | — | → GPT-4.1 nano |

### 🔵 Mistral AI — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ Mistral Large 2 (2407) | LEGACY | → Mistral Large 3 |
| ⚠️ Mistral Small 3 (older) | LEGACY | → Mistral Small 3.1 |
| ⚠️ Mixtral 8×7B (API) | LEGACY (still self-hostable) | → Mistral Medium 3 (API) |

---

## 🏷️ Price Change Log

| Date | Provider | Model | Change |
|---|---|---|---|
| 2026-04-11 | Anthropic | **Claude Opus 4.6** | ✅ Confirmed $5/$25 · 1M context at standard pricing · Fast Mode $30/$150 |
| 2026-04-11 | Anthropic | **Claude Sonnet 4.6** | ✅ Confirmed $3/$15 · 1M context standard · 1M beta on Sonnet 4.5 retiring Apr 30 |
| 2026-04-11 | Anthropic | **Claude Haiku 3** | ⚠️ DEPRECATION CONFIRMED — Retiring April 19, 2026 |
| 2026-04-11 | Anthropic | **Claude Haiku 3.5** | ⚠️ RETIRED — API now returns errors |
| 2026-04-11 | Anthropic | **Claude Sonnet 3.7** | ⚠️ RETIRED Feb 19, 2026 |
| 2026-04-11 | OpenAI | **GPT-5.4 family** | ✅ Confirmed launch Mar 5, 2026 · $2.50/$15 (short), $5/$22.50 (long ctx >270K) |
| 2026-04-11 | OpenAI | **GPT-5.4 Pro** | ✅ Confirmed $30/$180 |
| 2026-04-11 | OpenAI | **GPT-5.4 mini** | ✅ Confirmed $0.75/$4.50 (launched Mar 17, 2026) |
| 2026-04-11 | OpenAI | **GPT-5.4 nano** | ✅ Confirmed $0.20/$1.25 (launched Mar 17, 2026) |
| 2026-04-11 | OpenAI | **o4-mini** | ✅ Confirmed $1.10/$4.40 · replaced o3-mini |
| 2026-04-11 | OpenAI | **GPT-4o** | ⚠️ Marked LEGACY — superseded by GPT-4.1 |
| 2026-04-11 | Mistral | **Mistral Large 3** | ✅ Confirmed $0.50/$1.50 at 262K context |
| 2026-04-11 | Mistral | **Mistral Small 3.1** | ✅ Confirmed $0.20/$0.60 |
| 2026-04-11 | Mistral | **Mistral Large 2** | ⚠️ Marked LEGACY |

---

## ℹ️ Notes
- All prices are in **USD** and listed **per million tokens (MTok)**.
- **Batch API discounts (50%)** are available from both Anthropic and OpenAI. Mistral does **not** currently offer a batch discount tier.
- **Prompt/context caching** discounts apply where noted. Mistral does **not** offer prompt caching.
- Enterprise/volume pricing is available from all providers on a negotiated basis.
- Model availability on third-party platforms (AWS Bedrock, Vertex AI, Azure AI Foundry) may differ slightly from direct API pricing.
- **OpenAI GPT-5.4 family** uses short context (<270K) and long context (>270K) pricing tiers.
- **Mistral** processes all API data in the EU by default — a key compliance advantage for GDPR-regulated workloads.
- **Anthropic** offers US-only inference (data residency) at 1.1× pricing for models released after February 1, 2026.
- ⚠️ Models marked **RETIRED** will return API errors. Models marked **DEPRECATED** have a retirement date and should be migrated away from immediately.
