# 🟢 OpenAI — GPT Model Cards

> **Source:** [OpenAI API Pricing](https://openai.com/api/pricing/) | [OpenAI API Model Comparison](https://developers.openai.com/api/docs/models/compare)  
> **Date Scraped:** 2026-04-11  
> **Prices in USD per million tokens (MTok)**

---

## Model Pricing Overview

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Max Output | Knowledge Cutoff |
|---|---|---|---|---|---|---|
| GPT-5.4 | $2.50 | $0.25 | $15.00 | 1,050,000 | 128K | Aug 31, 2025 |
| GPT-5.4 mini | $0.75 | — | $4.50 | 400,000 | 128K | Aug 31, 2025 |
| GPT-5.4 nano | $0.20 | — | $1.25 | 400,000 | 128K | Aug 31, 2025 |
| GPT-5.2 | $1.75 | $0.18 | $14.00 | 400,000 | 128K | Aug 31, 2025 |
| GPT-4.1 | $2.00 | $0.50 | $8.00 | 1,047,576 | 32,768 | Jun 1, 2024 |
| o4-mini | $1.10 | $0.28 | $4.40 | 200,000 | 100K | Jun 1, 2024 |

---

## Individual Model Cards

### GPT-5.4

| Field | Detail |
|---|---|
| **Provider** | OpenAI |
| **Model Name** | GPT-5.4 |
| **Model ID** | `gpt-5.4` |
| **Input Price** | $2.50 / MTok |
| **Cached Input** | $0.25 / MTok (90% off standard) |
| **Output Price** | $15.00 / MTok |
| **Batch Input** | $1.25 / MTok (50% off) |
| **Batch Output** | $7.50 / MTok (50% off) |
| **Context Window** | 1,050,000 tokens |
| **Max Output Tokens** | 128,000 |
| **Knowledge Cutoff** | Aug 31, 2025 |
| **Availability** | OpenAI API (v1/chat/completions, v1/responses, v1/batch) |
| **Supported Features** | Streaming, Function calling, Structured outputs, Distillation, Image input |
| **Rate Limits (TPM)** | Tier 1: 500K · Tier 2: 1M · Tier 3: 2M · Tier 4: 4M · Tier 5: 40M |
| **Data Residency** | +10% for regional processing endpoints |
| **Status** | ✅ Active — Flagship model |
| **Notes** | Best intelligence at scale for agentic, coding, and professional workflows. |

---

### GPT-5.4 mini

| Field | Detail |
|---|---|
| **Provider** | OpenAI |
| **Model Name** | GPT-5.4 mini |
| **Model ID** | `gpt-5.4-mini` |
| **Input Price** | $0.75 / MTok |
| **Output Price** | $4.50 / MTok |
| **Context Window** | 400,000 tokens |
| **Max Output Tokens** | 128,000 |
| **Knowledge Cutoff** | Aug 31, 2025 |
| **Availability** | OpenAI API |
| **Status** | ✅ Active |
| **Notes** | Strongest mini model for coding, computer use, and subagents. ~25% cheaper input than Claude Haiku 4.5. |

---

### GPT-5.4 nano

| Field | Detail |
|---|---|
| **Provider** | OpenAI |
| **Model Name** | GPT-5.4 nano |
| **Model ID** | `gpt-5.4-nano` |
| **Input Price** | $0.20 / MTok |
| **Output Price** | $1.25 / MTok |
| **Context Window** | 400,000 tokens |
| **Max Output Tokens** | 128,000 |
| **Knowledge Cutoff** | Aug 31, 2025 |
| **Availability** | OpenAI API |
| **Status** | ✅ Active |
| **Notes** | Cheapest GPT-5.4-class model for simple high-volume tasks. 12× cheaper input than GPT-5.4 Standard. |

---

### GPT-5.2

| Field | Detail |
|---|---|
| **Provider** | OpenAI |
| **Model Name** | GPT-5.2 |
| **Model ID** | `gpt-5.2` |
| **Input Price** | $1.75 / MTok |
| **Cached Input** | $0.18 / MTok |
| **Output Price** | $14.00 / MTok |
| **Context Window** | 400,000 tokens |
| **Max Output Tokens** | 128,000 |
| **Knowledge Cutoff** | Aug 31, 2025 |
| **Availability** | OpenAI API (v1/chat/completions, v1/responses, v1/assistants, v1/batch, v1/fine-tuning) |
| **Supported Features** | Streaming, Function calling, Structured outputs, Fine-tuning, Distillation, Predicted outputs, Image input |
| **Rate Limits (TPM)** | Tier 1: 500K · Tier 2: 1M · Tier 3: 2M · Tier 4: 4M · Tier 5: 40M |
| **Status** | ✅ Active |
| **Notes** | Best model for coding and agentic tasks across industries. |

---

### GPT-4.1

| Field | Detail |
|---|---|
| **Provider** | OpenAI |
| **Model Name** | GPT-4.1 |
| **Model ID** | `gpt-4.1` |
| **Input Price** | $2.00 / MTok |
| **Cached Input** | $0.50 / MTok |
| **Output Price** | $8.00 / MTok |
| **Context Window** | 1,047,576 tokens |
| **Max Output Tokens** | 32,768 |
| **Knowledge Cutoff** | Jun 1, 2024 |
| **Availability** | OpenAI API (v1/chat/completions, v1/responses, v1/assistants, v1/batch, v1/fine-tuning) |
| **Supported Features** | Streaming, Function calling, Structured outputs, Fine-tuning, Distillation, Predicted outputs, Image input |
| **Fine-Tuning Pricing** | Training: ~$3.00 / MTok; Inference input: ~$3.00 / MTok; Inference output: ~$12.00 / MTok |
| **Rate Limits (TPM)** | Tier 1: 30K · Tier 2: 450K · Tier 3: 800K · Tier 4: 2M · Tier 5: 30M |
| **Status** | ✅ Active |
| **Notes** | Smartest non-reasoning model; 1M context window; advanced agentic planning. |

---

### o4-mini

| Field | Detail |
|---|---|
| **Provider** | OpenAI |
| **Model Name** | o4-mini |
| **Model ID** | `o4-mini` |
| **Input Price** | $1.10 / MTok |
| **Cached Input** | $0.28 / MTok |
| **Output Price** | $4.40 / MTok |
| **Context Window** | 200,000 tokens |
| **Max Output Tokens** | 100,000 |
| **Knowledge Cutoff** | Jun 1, 2024 |
| **Availability** | OpenAI API (v1/chat/completions, v1/responses, v1/assistants, v1/batch, v1/fine-tuning) |
| **Supported Features** | Streaming, Function calling, Structured outputs, Fine-tuning, Distillation, Predicted outputs, Image input |
| **Rate Limits (TPM)** | Tier 1: 100K · Tier 2: 2M · Tier 3: 4M · Tier 4: 10M · Tier 5: 150M |
| **Status** | ✅ Active (succeeded by GPT-5 mini) |
| **Notes** | Fast, cost-efficient reasoning model excelling in math, coding, and visual tasks. |

---

## Feature-Specific Pricing

### Batch API
- **Discount:** 50% off standard input and output prices.
- Processes requests asynchronously within 24 hours.
- Example: GPT-5.4 Standard → Batch: $1.25 input / $7.50 output per MTok.

### Prompt Caching
- OpenAI automatically caches repeated input content.
- Example: GPT-5.4 Standard cached input = **$0.25 / MTok** (90% discount vs. standard $2.50).
- Applications with consistent system prompts benefit most.

### Data Residency / Regional Processing
- Regional processing endpoints for `gpt-5.4`, `gpt-5.4-mini`, `gpt-5.4-nano`, and `gpt-5.4-pro` incur **+10% uplift**.
- Applies to models released after March 5, 2026.

### Fine-Tuning
- GPT-4.1: ~$3.00 / MTok training; ~$3.00 input / $12.00 output for fine-tuned inference.
- GPT-4.1 Mini: ~$0.80 / MTok training; ~$0.80 input / $3.20 output.

---

## Rate Limit Tiers

Rate limits vary by model and usage tier (Tier 1–5). Example TPM limits for GPT-5.4:

| Tier | TPM Limit |
|---|---|
| Free | N/A |
| Tier 1 | 500,000 |
| Tier 2 | 1,000,000 |
| Tier 3 | 2,000,000 |
| Tier 4 | 4,000,000 |
| Tier 5 | 40,000,000 |

## Availability
- **Direct API:** [platform.openai.com](https://platform.openai.com)
- **Azure OpenAI Service:** Pay-as-you-go (comparable rates); Provisioned Throughput Units (PTUs) available for reserved capacity.

---

*Source: [openai.com/api/pricing](https://openai.com/api/pricing/) | [developers.openai.com/api/docs/models/compare](https://developers.openai.com/api/docs/models/compare) — Verified 2026-04-11*
