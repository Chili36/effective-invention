# 🟢 OpenAI — GPT Model Cards

> **Source:** [OpenAI API Pricing](https://developers.openai.com/api/docs/pricing)  
> **Date Scraped:** 2026-04-11 (refresh #2)  
> **Prices in USD per million tokens (MTok)**  
> **⚠️ Price Change Alert:** 🆕 `gpt-5.4-pro` added; long-context tier for `gpt-5.4` added; cached input confirmed for `gpt-5.4-mini` and `gpt-5.4-nano`.

---

## Flagship Model Pricing (Standard — Short Context < 270K tokens)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) |
|---|---|---|---|
| gpt-5.4 | $2.50 | $0.25 | $15.00 |
| gpt-5.4-mini | $0.75 | $0.075 | $4.50 |
| gpt-5.4-nano | $0.20 | $0.020 | $1.25 |
| 🆕 gpt-5.4-pro | $30.00 | — | $180.00 |

## Flagship Model Pricing (Standard — Long Context > 270K tokens)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) |
|---|---|---|---|
| 🆕 gpt-5.4 | $5.00 | $0.50 | $22.50 |
| 🆕 gpt-5.4-pro | $60.00 | — | $270.00 |

> **Note:** `gpt-5.4-mini` and `gpt-5.4-nano` do not have a separate long-context tier.

## Flagship Model Pricing — Batch (50% off Standard)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) |
|---|---|---|---|
| gpt-5.4 | $1.25 | $0.13 | $7.50 |
| gpt-5.4-mini | $0.375 | $0.0375 | $2.25 |
| gpt-5.4-nano | $0.10 | $0.01 | $0.625 |
| gpt-5.4-pro | $15.00 | — | $90.00 |

> Batch API processes requests asynchronously within 24 hours.

## Flagship Model Pricing — Priority (Higher Cost, Low Latency)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) |
|---|---|---|---|
| gpt-5.4 | $5.00 | $0.50 | $30.00 |

---

## Specialized & Legacy Models

| Model | Category | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context |
|---|---|---|---|---|---|
| gpt-5.3-chat-latest | ChatGPT | $1.75 | $0.175 | $14.00 | 400K |
| gpt-5.3-codex | Codex | $1.75 | $0.175 | $14.00 | 400K |
| gpt-4.1 | General | $2.00 | $0.50 | $8.00 | 1.04M |
| o4-mini | Reasoning | $1.10 | $0.28 | $4.40 | 200K |
| computer-use-preview | Computer Use | $1.50 | — | $6.00 | — |

> `gpt-5.3-codex` in Priority mode: $3.50 / $0.35 / $28.00 per MTok.

## Deep Research Models (Batch only)

| Model | Input ($/MTok) | Output ($/MTok) |
|---|---|---|
| o3-deep-research | $5.00 | $20.00 |
| o4-mini-deep-research | $1.00 | $4.00 |

---

## Realtime & Audio Models

| Model | Modality | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) |
|---|---|---|---|---|
| gpt-realtime-1.5 | Audio | $32.00 | $0.40 | $64.00 |
| gpt-realtime-1.5 | Text | $4.00 | $0.40 | $16.00 |
| gpt-realtime-1.5 | Image | $5.00 | $0.50 | — |
| gpt-realtime-mini | Audio | $10.00 | $0.30 | $20.00 |
| gpt-realtime-mini | Text | $0.60 | $0.06 | $2.40 |
| gpt-realtime-mini | Image | $0.80 | $0.08 | — |

---

## Image Generation Models

| Model | Modality | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) |
|---|---|---|---|---|
| gpt-image-1.5 | Image | $8.00 | $2.00 | $32.00 |
| gpt-image-1.5 | Text | $5.00 | $1.25 | $10.00 |
| gpt-image-1-mini | Image | $2.50 | $0.25 | $8.00 |
| gpt-image-1-mini | Text | $2.00 | $0.20 | — |

> Per-image output pricing for DALL·E models listed in the image generation guide.

---

## Video Generation Models (per second)

| Model | Resolution | Price / second |
|---|---|---|
| sora-2 | 720p | $0.10 |
| sora-2-pro | 720p | $0.30 |
| sora-2-pro | 1024p | $0.50 |
| sora-2-pro | 1080p | $0.70 |

> Batch: 50% off — sora-2 at $0.05/sec, sora-2-pro 720p at $0.15/sec.

---

## Fine-Tuning (o4-mini)

| Model | Training | Input ($/MTok) | Cached ($/MTok) | Output ($/MTok) |
|---|---|---|---|---|
| o4-mini-2025-04-16 | $100.00 / hr | $4.00 | $1.00 | $16.00 |
| o4-mini-2025-04-16 (data sharing) | $100.00 / hr | $2.00 | $0.50 | $8.00 |

> Batch fine-tuning: $2.00/$0.50/$8.00 (standard) or $1.00/$0.25/$4.00 (data sharing).

---

## Individual Model Cards

### GPT-5.4

| Field | Detail |
|---|---|
| **Provider** | OpenAI |
| **Model Name** | GPT-5.4 |
| **Model ID** | `gpt-5.4` |
| **Input Price** | $2.50 / MTok (short ctx) · $5.00 / MTok (long ctx >270K) |
| **Cached Input** | $0.25 / MTok (short ctx) · $0.50 / MTok (long ctx) |
| **Output Price** | $15.00 / MTok (short ctx) · $22.50 / MTok (long ctx) |
| **Batch Input** | $1.25 / MTok |
| **Batch Output** | $7.50 / MTok |
| **Priority Input** | $5.00 / MTok |
| **Priority Output** | $30.00 / MTok |
| **Context Window** | 1,050,000 tokens |
| **Knowledge Cutoff** | Aug 31, 2025 |
| **Availability** | OpenAI API (v1/chat/completions, v1/responses, v1/batch) |
| **Supported Features** | Streaming, Function calling, Structured outputs, Distillation, Image input, Computer use |
| **Data Residency** | +10% for regional processing endpoints |
| **Status** | ✅ Active — Current flagship model |
| **Notes** | Best intelligence at scale for agentic, coding, and professional workflows. |

---

### 🆕 GPT-5.4 Pro

| Field | Detail |
|---|---|
| **Provider** | OpenAI |
| **Model Name** | GPT-5.4 Pro |
| **Model ID** | `gpt-5.4-pro` |
| **First Tracked** | 2026-04-11 |
| **Input Price** | $30.00 / MTok (short ctx) · $60.00 / MTok (long ctx >270K) |
| **Output Price** | $180.00 / MTok (short ctx) · $270.00 / MTok (long ctx) |
| **Batch Input** | $15.00 / MTok |
| **Batch Output** | $90.00 / MTok |
| **Data Residency** | +10% for regional processing endpoints |
| **Status** | ✅ Active — Extended reasoning / Pro tier |
| **Notes** | Premium reasoning model; 6× the cost of standard GPT-5.4. Built for ChatGPT Pro-class workloads. |

---

### GPT-5.4 mini

| Field | Detail |
|---|---|
| **Provider** | OpenAI |
| **Model Name** | GPT-5.4 mini |
| **Model ID** | `gpt-5.4-mini` |
| **Input Price** | $0.75 / MTok |
| **Cached Input** | $0.075 / MTok *(confirmed this refresh)* |
| **Output Price** | $4.50 / MTok |
| **Context Window** | 400,000 tokens |
| **Knowledge Cutoff** | Aug 31, 2025 |
| **Availability** | OpenAI API |
| **Status** | ✅ Active |
| **Notes** | Strongest mini model for coding, computer use, and subagents. |

---

### GPT-5.4 nano

| Field | Detail |
|---|---|
| **Provider** | OpenAI |
| **Model Name** | GPT-5.4 nano |
| **Model ID** | `gpt-5.4-nano` |
| **Input Price** | $0.20 / MTok |
| **Cached Input** | $0.020 / MTok *(confirmed this refresh)* |
| **Output Price** | $1.25 / MTok |
| **Context Window** | 400,000 tokens |
| **Knowledge Cutoff** | Aug 31, 2025 |
| **Availability** | OpenAI API |
| **Status** | ✅ Active |
| **Notes** | Cheapest GPT-5.4-class model for simple high-volume tasks. |

---

### GPT-5.3 Chat / Codex

| Field | Detail |
|---|---|
| **Provider** | OpenAI |
| **Model Name** | GPT-5.3 Chat / Codex |
| **Model IDs** | `gpt-5.3-chat-latest` · `gpt-5.3-codex` |
| **Input Price** | $1.75 / MTok |
| **Cached Input** | $0.175 / MTok |
| **Output Price** | $14.00 / MTok |
| **Context Window** | 400,000 tokens |
| **Availability** | OpenAI API |
| **Status** | ✅ Active (specialized ChatGPT / Codex tier) |
| **Notes** | Codex Priority mode: $3.50/$28.00 per MTok. |

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
| **Knowledge Cutoff** | Jun 1, 2024 |
| **Availability** | OpenAI API (incl. fine-tuning) |
| **Fine-Tuning** | Training ~$3.00/MTok; Inference ~$3.00 input / $12.00 output per MTok |
| **Status** | ✅ Active |
| **Notes** | 1M context; strong instruction-following and coding benchmark scores. |

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
| **Knowledge Cutoff** | Jun 1, 2024 |
| **Availability** | OpenAI API (incl. fine-tuning) |
| **Status** | ✅ Active (succeeded by GPT-5 mini) |
| **Notes** | Chain-of-thought reasoning model. Reasoning tokens billed as output. |

---

## Feature-Specific Pricing

### Context Tiers
- **Short context** (<270K tokens): standard prices.
- **Long context** (>270K tokens): 2× input / 1.5× output premium for `gpt-5.4` and `gpt-5.4-pro`.

### Batch API
- **50% off** all token costs (input + output); results within 24 hours.

### Flex Processing
- Same pricing as Batch; slower response times; not guaranteed availability.

### Priority Processing
- Available for `gpt-5.4` only: **2× input / 2× output** vs. standard.

### Prompt Caching
- OpenAI automatically caches repeated input prefixes.
- Example: `gpt-5.4` short-ctx cached = $0.25/MTok (90% off standard $2.50).

### Data Residency / Regional Processing
- Regional endpoints for `gpt-5.4`, `gpt-5.4-mini`, `gpt-5.4-nano`, `gpt-5.4-pro`: **+10% uplift**.
- Applies to models released after March 5, 2026.

### Web Search Tool
- `gpt-4o` / `gpt-4.1` models: **$10 / 1,000 calls**; search content tokens billed at model rates.
- Reasoning models incl. `gpt-5` and newer: **$25 / 1,000 calls**; search content tokens are free.

### Container / Code Interpreter
- 1 GB: $0.03; 4 GB: $0.12; 16 GB: $0.48; 64 GB: $1.92 per 20-minute session.

### File Search
- Storage: **$0.10 / GB per day** (1 GB free).
- Tool call (Responses API): **$2.50 / 1,000 calls**.

---

## Availability
- **Direct API:** [platform.openai.com](https://platform.openai.com)
- **Azure OpenAI Service:** Comparable PAYG rates; PTUs available for reserved capacity.

---

*Source: [developers.openai.com/api/docs/pricing](https://developers.openai.com/api/docs/pricing) — Verified 2026-04-11*
