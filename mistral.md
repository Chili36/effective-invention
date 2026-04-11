# 🔵 Mistral AI — Model Cards

> **Sources:** [Mistral AI Pricing Page](https://mistral.ai/pricing) | [Mistral Docs Pricing](https://docs.mistral.ai/deployment/ai-studio/pricing) | [PricePerToken.com — Mistral](https://pricepertoken.com/pricing-page/provider/mistral-ai)  
> **Date Scraped:** 2026-04-11  
> **Prices in USD per million tokens (MTok)**

---

## Model Pricing Overview

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Best For | Status |
|---|---|---|---|---|---|
| Mistral Large 3 (2512) | $0.50 | $1.50 | 262,000 | Complex reasoning, multilingual, flagship OSS | ✅ Active |
| Mistral Medium 3 | $0.40 | $2.00 | 131,000 | Balanced cost/performance, coding, enterprise | ✅ Active |
| Codestral | $1.00 | $3.00 | 128,000 | Code generation, developer automation | ✅ Active |
| Mistral Nemo | $0.15 | $0.15 | 128,000 | Lightweight, fast inference | ✅ Active |
| Ministral 14B | $0.20 | $0.20 | 256,000 | Edge/local workloads, efficient reasoning | ✅ Active |
| Ministral 8B | $0.15 | $0.15 | 256,000 | Edge/local workloads, speed-critical tasks | ✅ Active |
| Ministral 3B | $0.10 | $0.10 | 556,000 | Ultra-lightweight, high-volume | ✅ Active |
| Mistral Large 2 (legacy) | $2.00 | $6.00 | 128,000 | Legacy enterprise workloads | ⚠️ Legacy |

---

## Individual Model Cards

### Mistral Large 3 (2512)

| Field | Detail |
|---|---|
| **Provider** | Mistral AI |
| **Model Name** | Mistral Large 3 (2512) |
| **Model ID** | `mistral-large-2512` |
| **Released** | December 1, 2025 |
| **Input Price** | $0.50 / MTok |
| **Output Price** | $1.50 / MTok |
| **Context Window** | 262,144 tokens |
| **Availability** | Mistral AI Studio (API) |
| **Status** | ✅ Active — Current flagship |
| **Notes** | One of the best OSS models in the world. Superior reasoning, multilingual support, native multimodal capabilities. Tier-1 performance at an industry-leading price point. |

---

### Mistral Medium 3

| Field | Detail |
|---|---|
| **Provider** | Mistral AI |
| **Model Name** | Mistral Medium 3 |
| **Model ID** | `mistral-medium-3` |
| **Released** | May 7, 2025 |
| **Input Price** | $0.40 / MTok |
| **Output Price** | $2.00 / MTok |
| **Context Window** | 131,072 tokens |
| **Availability** | Mistral AI Studio (API) |
| **Status** | ✅ Active |
| **Notes** | State-of-the-art performance at claimed 8× lower cost than rival GPT-4-class models. Strong for coding, logical reasoning, and enterprise use cases. Price-performance hero. |

---

### Codestral

| Field | Detail |
|---|---|
| **Provider** | Mistral AI |
| **Model Name** | Codestral |
| **Model ID** | `codestral-latest` |
| **Input Price** | $1.00 / MTok |
| **Output Price** | $3.00 / MTok |
| **Context Window** | 128,000 tokens |
| **Availability** | Mistral AI Studio (API); Le Chat (subscription-included) |
| **Status** | ✅ Active |
| **Notes** | Specifically designed for advanced coding agents. Strong code generation and agentic capabilities. API usage billed per token (separate from Le Chat subscription). |

---

### Mistral Nemo

| Field | Detail |
|---|---|
| **Provider** | Mistral AI |
| **Model Name** | Mistral Nemo |
| **Model ID** | `open-mistral-nemo` |
| **Input Price** | $0.15 / MTok |
| **Output Price** | $0.15 / MTok |
| **Context Window** | 128,000 tokens |
| **Availability** | Mistral AI Studio (API) |
| **Status** | ✅ Active |
| **Notes** | Lightweight, cost-efficient model with flat input/output pricing. Great for summarization and simple NLP tasks. |

---

### Ministral 14B

| Field | Detail |
|---|---|
| **Provider** | Mistral AI |
| **Model Name** | Ministral 14B |
| **Model ID** | `ministral-14b` |
| **Input Price** | $0.20 / MTok |
| **Output Price** | $0.20 / MTok |
| **Context Window** | 256,000 tokens |
| **Availability** | Mistral AI Studio (API) |
| **Status** | ✅ Active |
| **Notes** | Part of the Ministral 3 family — the world's best edge models. Flat input/output pricing. |

---

### Ministral 8B

| Field | Detail |
|---|---|
| **Provider** | Mistral AI |
| **Model Name** | Ministral 8B |
| **Model ID** | `ministral-8b` |
| **Input Price** | $0.15 / MTok |
| **Output Price** | $0.15 / MTok |
| **Context Window** | 256,000 tokens |
| **Availability** | Mistral AI Studio (API) |
| **Status** | ✅ Active |
| **Notes** | Speed-critical tasks and high-volume workloads. Flat input/output pricing. |

---

### Ministral 3B

| Field | Detail |
|---|---|
| **Provider** | Mistral AI |
| **Model Name** | Ministral 3B |
| **Model ID** | `ministral-3b` |
| **Input Price** | $0.10 / MTok |
| **Output Price** | $0.10 / MTok |
| **Context Window** | 556,000 tokens |
| **Availability** | Mistral AI Studio (API) |
| **Status** | ✅ Active |
| **Notes** | Ultra-lightweight, massive context window, ultra-low price. Ideal for classification, summarization, and edge inference. |

---

### Mistral Large 2 (Legacy)

| Field | Detail |
|---|---|
| **Provider** | Mistral AI |
| **Model Name** | Mistral Large 2 |
| **Model ID** | `mistral-large-2407` |
| **Input Price** | $2.00 / MTok |
| **Output Price** | $6.00 / MTok |
| **Context Window** | 128,000 tokens |
| **Availability** | Mistral AI Studio (API) |
| **Status** | ⚠️ Legacy — superseded by Large 3 |
| **Notes** | Older flagship model; retained for compatibility. Significantly more expensive than current Large 3. |

---

## Feature-Specific Pricing

### Batch Inference
- Available for supported models via Mistral AI Studio.
- Asynchronous processing at discounted rates — check Mistral docs for current batch multipliers.

### Embeddings
- Mistral Embed: ~**$0.01 / MTok** (flat rate for text embeddings).

### Fine-Tuning
- Available via Mistral AI Studio for supported models.
- Custom pricing — contact Mistral for enterprise fine-tuning agreements.

---

## Subscription Plans (Le Chat)

| Plan | Price | Notes |
|---|---|---|
| Free | $0/mo | Access to core models; usage limits apply |
| Pro | $14.99/mo | Unlimited chats (fair use), 150 Flash Answers/day, No Telemetry Mode, Codestral included |
| Student | ~$7/mo (~53% off Pro) | Requires .edu email; annual renewal |
| Team | Custom/seat | 30GB storage/user, domain verification, admin console, training opt-out |
| Enterprise | $20K+/month (custom) | Private/on-prem deployment, no-code agents, audit logs, EU data residency |

> **Note:** Le Chat subscription plans are separate from API usage. API access is always billed per token.

---

## Rate Limits
- Rate limits are based on usage tier in Mistral AI Studio.
- Default data retention: 30 days; Enterprise can enforce zero retention.
- See [Mistral Rate Limits & Usage Tiers](https://docs.mistral.ai/deployment/ai-studio/tier) for tier details.

## Availability
- **Direct API:** [console.mistral.ai](https://console.mistral.ai) (Mistral AI Studio)
- **Azure AI Foundry:** Select Mistral models available via Microsoft Azure.
- **Self-Hosted / On-Prem:** Available for enterprise — contact Mistral AI.
- **Open Source:** Mistral Large 3 and other models released open-weight on Hugging Face.

---

*Sources: [mistral.ai/pricing](https://mistral.ai/pricing) | [pricepertoken.com/pricing-page/provider/mistral-ai](https://pricepertoken.com/pricing-page/provider/mistral-ai) | [pricepertoken.com — Mistral Medium 3](https://pricepertoken.com/pricing-page/model/mistral-ai-mistral-medium-3) | [pricepertoken.com — Mistral Large 3 2512](https://pricepertoken.com/pricing-page/model/mistral-ai-mistral-large-2512) — Verified 2026-04-11*
