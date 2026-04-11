# 🤖 LLM Pricing Tracker

Up-to-date pricing and specifications for large language models from **Anthropic**, **OpenAI**, and **Mistral AI**.

> **Last updated:** 2026-04-11 (refresh #2)  
> **Sources:** Official provider pricing pages — scraped/verified on date above.

---

## 📋 Quick-Reference Index

### Anthropic — Claude Models

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| Claude Opus 4.6 | $5.00 | $25.00 | 1M tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Opus 4.5 | $5.00 | $25.00 | 200K tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Opus 4.1 | $15.00 | $75.00 | 200K tokens | API, AWS Bedrock, Vertex AI |
| Claude Sonnet 4.6 | $3.00 | $15.00 | 1M tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Sonnet 4.5 | $3.00 | $15.00 | 200K tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Sonnet 4 | $3.00 | $15.00 | 200K tokens | API, AWS Bedrock, Vertex AI |
| Claude Haiku 4.5 | $1.00 | $5.00 | 200K tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Haiku 3.5 | $0.80 | $4.00 | 200K tokens | API, AWS Bedrock, Vertex AI |
| Claude Haiku 3 | $0.25 | $1.25 | 200K tokens | API, AWS Bedrock, Vertex AI |

### OpenAI — GPT Models

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|---|
| GPT-5.4 | $2.50 | $0.25 | $15.00 | 1.05M tokens (short ctx <270K) | API |
| GPT-5.4 *(long ctx >270K)* | $5.00 | $0.50 | $22.50 | 1.05M tokens | API |
| 🆕 GPT-5.4 Pro | $30.00 | — | $180.00 | 1.05M tokens | API |
| GPT-5.4 mini | $0.75 | $0.075 | $4.50 | 400K tokens | API |
| GPT-5.4 nano | $0.20 | $0.020 | $1.25 | 400K tokens | API |
| GPT-5.3 Chat / Codex | $1.75 | $0.175 | $14.00 | 400K tokens | API |
| GPT-4.1 | $2.00 | $0.50 | $8.00 | 1.04M tokens | API |
| o4-mini | $1.10 | $0.28 | $4.40 | 200K tokens | API |

### Mistral AI — Models

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| Mistral Large 3 (2512) | $0.50 | $1.50 | 262K tokens | API (Mistral AI Studio) |
| Mistral Medium 3 | $0.40 | $2.00 | 131K tokens | API (Mistral AI Studio) |
| 🆕 Mistral Small 3.1 | $0.20 | $0.60 | 128K tokens | API (Mistral AI Studio) |
| Codestral | $1.00 | $3.00 | 128K tokens | API (Mistral AI Studio) |
| Mistral Nemo | $0.15 | $0.15 | 128K tokens | API (Mistral AI Studio) |
| Ministral 14B | $0.20 | $0.20 | 256K tokens | API (Mistral AI Studio) |
| Ministral 8B | $0.10 | $0.10 | 256K tokens | API (Mistral AI Studio) |
| Ministral 3B | $0.10 | $0.10 | 556K tokens | API (Mistral AI Studio) |

---

## 📁 Model Card Files

| Provider | File |
|---|---|
| Anthropic | [anthropic.md](./anthropic.md) |
| OpenAI | [openai.md](./openai.md) |
| Mistral AI | [mistral.md](./mistral.md) |

---

## 🏷️ Price Change Log

| Date | Provider | Model | Change |
|---|---|---|
| 2026-04-11 | *Initial tracking* | All models | Baseline established |
| 2026-04-11 | OpenAI | **GPT-5.4 Pro** | 🆕 NEW — $30.00 input / $180.00 output per MTok |
| 2026-04-11 | OpenAI | **GPT-5.4** (long ctx) | 🆕 NEW — Long-context tier (>270K tokens): $5.00/$22.50 per MTok |
| 2026-04-11 | OpenAI | **GPT-5.4 mini** | 🔄 UPDATE — Cached input confirmed at $0.075/MTok (was unlisted) |
| 2026-04-11 | OpenAI | **GPT-5.4 nano** | 🔄 UPDATE — Cached input confirmed at $0.020/MTok (was unlisted) |
| 2026-04-11 | Mistral | **Mistral Small 3.1** | 🆕 NEW — $0.20 input / $0.60 output per MTok |
| 2026-04-11 | Anthropic | *(all)* | ✅ No changes — prices confirmed stable |

---

## ℹ️ Notes
- All prices are in **USD** and listed **per million tokens (MTok)**.
- Batch API discounts (50%) are available from both Anthropic and OpenAI.
- Prompt/context caching discounts apply where noted in the full model cards.
- Enterprise/volume pricing is available from all providers on a negotiated basis.
- Model availability on third-party platforms (AWS Bedrock, Vertex AI) may differ slightly from direct API pricing.
- OpenAI now uses **short context** (<270K) and **long context** (>270K) pricing tiers for flagship models.
