# 🔵 Mistral AI — Model Cards

> **Sources:** [Mistral AI Pricing Page](https://mistral.ai/pricing) · [PricePerToken.com — Mistral](https://pricepertoken.com/pricing-page/provider/mistral-ai) · [DevTk.AI Mistral Pricing Guide (Feb 2026)](https://devtk.ai/en/blog/mistral-api-pricing-guide-2026/)  
> **Date Scraped:** 2026-04-11 (refresh #2)  
> **Prices in USD per million tokens (MTok)**  
> **⚠️ Price Change Alert:** 🆕 `Mistral Small 3.1` added ($0.20/$0.60 per MTok).

---

## Model Pricing Overview

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Best For | Status |
|---|---|---|---|---|---|
| Mistral Large 3 (2512) | $0.50 | $1.50 | 262,000 | Complex reasoning, multilingual, flagship OSS | ✅ Active |
| Mistral Medium 3 | $0.40 | $2.00 | 131,000 | Balanced cost/performance, coding, enterprise | ✅ Active |
| 🆕 Mistral Small 3.1 | $0.20 | $0.60 | 128,000 | High-volume agentic tasks, multimodal | ✅ Active |
| Codestral | $1.00 | $3.00 | 128,000 | Code generation, developer automation | ✅ Active |
| Mistral Nemo | $0.15 | $0.15 | 128,000 | Lightweight, fast inference | ✅ Active |
| Ministral 14B | $0.20 | $0.20 | 256,000 | Edge/local workloads, efficient reasoning | ✅ Active |
| Ministral 8B | $0.10 | $0.10 | 256,000 | Edge/local workloads, speed-critical tasks | ✅ Active |
| Ministral 3B | $0.10 | $0.10 | 556,000 | Ultra-lightweight, high-volume | ✅ Active |
| Mistral Large 2411 (legacy) | $2.00 | $6.00 | 131,000 | Legacy — superseded by Large 3 (2512) | ⚠️ Legacy |

> **Note on `mistral-large-latest`:** The API alias `mistral-large-latest` may still point to `mistral-large-2411` ($2.00/$6.00) depending on your region and account. Always pin to a specific model version for cost predictability.

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
| **Status** | ✅ Active — Current flagship OSS model |
| **Notes** | One of the best open-weight models. Superior reasoning, multilingual support, native multimodal. Cheapest output pricing in its capability tier. |

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
| **Notes** | GPT-4-class performance at a fraction of the cost. Strong coding, logical reasoning, and enterprise use cases. |

---

### 🆕 Mistral Small 3.1

| Field | Detail |
|---|---|
| **Provider** | Mistral AI |
| **Model Name** | Mistral Small 3.1 |
| **Model ID** | `mistral-small-3.1` |
| **First Tracked** | 2026-04-11 |
| **Input Price** | $0.20 / MTok |
| **Output Price** | $0.60 / MTok |
| **Context Window** | 128,000 tokens |
| **Availability** | Mistral AI Studio (API) |
| **Status** | ✅ Active |
| **Notes** | Optimized for agentic tasks, coding, and multimodal understanding. Competes directly with Gemini Flash on price. One of the most affordable capable models on the market. |

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
| **Notes** | Lightweight, cost-efficient with flat input/output pricing. Great for summarization and simple NLP. |

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
| **Notes** | Best-in-class edge model. Flat input/output pricing. |

---

### Ministral 8B

| Field | Detail |
|---|---|
| **Provider** | Mistral AI |
| **Model Name** | Ministral 8B |
| **Model ID** | `ministral-8b` |
| **Input Price** | $0.10 / MTok |
| **Output Price** | $0.10 / MTok |
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
| **Notes** | Ultra-lightweight, massive context window. Ideal for classification, summarization, edge inference. |

---

### Mistral Large 2411 (Legacy)

| Field | Detail |
|---|---|
| **Provider** | Mistral AI |
| **Model Name** | Mistral Large 2411 |
| **Model ID** | `mistral-large-2411` |
| **Released** | November 19, 2024 |
| **Input Price** | $2.00 / MTok |
| **Output Price** | $6.00 / MTok |
| **Context Window** | 131,072 tokens |
| **Availability** | Mistral AI Studio (API) |
| **Status** | ⚠️ Legacy — superseded by Large 3 (2512) |
| **Notes** | `mistral-large-latest` API alias may still route here. Pin to `mistral-large-2512` to get the newer, cheaper model. |

---

## Feature-Specific Pricing

### Batch Inference
- Available via Mistral AI Studio for supported models; asynchronous processing at discounted rates.

### Embeddings
- **Mistral Embed:** ~**$0.02 / MTok** (flat rate for text embeddings).

### Fine-Tuning
- Available for Small and Medium models via Mistral AI Studio.
- Custom pricing — contact Mistral for enterprise fine-tuning agreements.
- Strategy: fine-tuned Small 3.1 can replace Large 3 at ~10× lower cost for narrow tasks.

### Open-Weight Models
- Mistral 7B, Mixtral 8x7B, Mixtral 8x22B available under **Apache 2.0** for self-hosting.
- No per-token fees for self-hosted deployments.

---

## Subscription Plans (Le Chat)

| Plan | Price | Notes |
|---|---|---|
| Free | $0/mo | Core models; usage limits apply |
| Pro | $14.99/mo | Unlimited chats (fair use), 150 Flash Answers/day, No Telemetry Mode, Codestral included, 15 GB doc storage |
| Student | ~$7/mo (~53% off Pro) | Requires .edu email; annual renewal |
| Team | Custom/seat | 30 GB storage/user, domain verification, admin console, training opt-out |
| Enterprise | $20K+/month (custom) | Private/on-prem, no-code agents, audit logs, EU data residency |

> **Note:** Subscription plans are separate from API usage. API is always billed per token.

---

## Availability
- **Direct API:** [console.mistral.ai](https://console.mistral.ai) (Mistral AI Studio)
- **Azure AI Foundry:** Select Mistral models available via Microsoft Azure.
- **Self-Hosted / On-Prem:** Enterprise option — contact Mistral AI.
- **Open Source:** Large 3 and other models released open-weight on Hugging Face (Apache 2.0).

---

*Sources: [mistral.ai/pricing](https://mistral.ai/pricing) · [pricepertoken.com/pricing-page/provider/mistral-ai](https://pricepertoken.com/pricing-page/provider/mistral-ai) · [devtk.ai/en/blog/mistral-api-pricing-guide-2026](https://devtk.ai/en/blog/mistral-api-pricing-guide-2026/) — Verified 2026-04-11*
