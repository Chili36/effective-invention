# 🟠 Anthropic — Claude Model Cards

> **Source:** [Anthropic Claude API Pricing Docs](https://platform.claude.com/docs/en/about-claude/pricing)  
> **Date Scraped:** 2026-04-11  
> **Prices in USD per million tokens (MTok)**

---

## Model Pricing Overview

| Model | Input ($/MTok) | 5-min Cache Write | 1-hr Cache Write | Cache Hit | Output ($/MTok) | Status |
|---|---|---|---|---|---|---|
| Claude Opus 4.6 | $5.00 | $6.25 | $10.00 | $0.50 | $25.00 | ✅ Active |
| Claude Opus 4.5 | $5.00 | $6.25 | $10.00 | $0.50 | $25.00 | ✅ Active |
| Claude Opus 4.1 | $15.00 | $18.75 | $30.00 | $1.50 | $75.00 | ✅ Active |
| Claude Opus 4 | $15.00 | $18.75 | $30.00 | $1.50 | $75.00 | ✅ Active |
| Claude Sonnet 4.6 | $3.00 | $3.75 | $6.00 | $0.30 | $15.00 | ✅ Active |
| Claude Sonnet 4.5 | $3.00 | $3.75 | $6.00 | $0.30 | $15.00 | ✅ Active |
| Claude Sonnet 4 | $3.00 | $3.75 | $6.00 | $0.30 | $15.00 | ✅ Active |
| Claude Sonnet 3.7 | $3.00 | $3.75 | $6.00 | $0.30 | $15.00 | ⚠️ Deprecated |
| Claude Haiku 4.5 | $1.00 | $1.25 | $2.00 | $0.10 | $5.00 | ✅ Active |
| Claude Haiku 3.5 | $0.80 | $1.00 | $1.60 | $0.08 | $4.00 | ✅ Active |
| Claude Opus 3 | $15.00 | $18.75 | $30.00 | $1.50 | $75.00 | ⚠️ Deprecated |
| Claude Haiku 3 | $0.25 | $0.30 | $0.50 | $0.03 | $1.25 | ✅ Active |

---

## Individual Model Cards

### Claude Opus 4.6

| Field | Detail |
|---|---|
| **Provider** | Anthropic |
| **Model Name** | Claude Opus 4.6 |
| **Model ID** | `claude-opus-4-6` |
| **Input Price** | $5.00 / MTok |
| **Output Price** | $25.00 / MTok |
| **Batch Input** | $2.50 / MTok (50% off) |
| **Batch Output** | $12.50 / MTok (50% off) |
| **5-min Cache Write** | $6.25 / MTok |
| **1-hr Cache Write** | $10.00 / MTok |
| **Cache Hit** | $0.50 / MTok |
| **Context Window** | 1,000,000 tokens (standard pricing, no long-context surcharge) |
| **Availability** | Anthropic API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Fast Mode** | Available at 6× standard rates ($30 input / $150 output per MTok) |
| **Data Residency** | US-only inference: +10% pricing multiplier |
| **Rate Limits** | Tier-based (Tier 1–4 + Enterprise) |
| **Status** | ✅ Active — Flagship model |
| **Notes** | Full 1M context at standard rates; 1M-context surcharge removed as of early 2026. |

---

### Claude Opus 4.5

| Field | Detail |
|---|---|
| **Provider** | Anthropic |
| **Model Name** | Claude Opus 4.5 |
| **Model ID** | `claude-opus-4-5-20251101` |
| **Input Price** | $5.00 / MTok |
| **Output Price** | $25.00 / MTok |
| **Batch Input** | $2.50 / MTok |
| **Batch Output** | $12.50 / MTok |
| **Context Window** | 200,000 tokens |
| **Availability** | Anthropic API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Status** | ✅ Active |
| **Notes** | Released November 2025. Best-in-class for coding, agents, and computer use. Includes effort control parameter. |

---

### Claude Opus 4.1

| Field | Detail |
|---|---|
| **Provider** | Anthropic |
| **Model Name** | Claude Opus 4.1 |
| **Input Price** | $15.00 / MTok |
| **Output Price** | $75.00 / MTok |
| **Batch Input** | $7.50 / MTok |
| **Batch Output** | $37.50 / MTok |
| **Context Window** | 200,000 tokens |
| **Availability** | Anthropic API, AWS Bedrock, Google Vertex AI |
| **Status** | ✅ Active (legacy tier) |
| **Notes** | Upgraded agentic performance and real-world coding. Released August 2025. |

---

### Claude Sonnet 4.6

| Field | Detail |
|---|---|
| **Provider** | Anthropic |
| **Model Name** | Claude Sonnet 4.6 |
| **Input Price** | $3.00 / MTok |
| **Output Price** | $15.00 / MTok |
| **Batch Input** | $1.50 / MTok |
| **Batch Output** | $7.50 / MTok |
| **5-min Cache Write** | $3.75 / MTok |
| **1-hr Cache Write** | $6.00 / MTok |
| **Cache Hit** | $0.30 / MTok |
| **Context Window** | 1,000,000 tokens (standard pricing, no long-context surcharge) |
| **Availability** | Anthropic API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Status** | ✅ Active |
| **Notes** | High-throughput general-purpose model. 1M-context surcharge removed early 2026. |

---

### Claude Sonnet 4.5

| Field | Detail |
|---|---|
| **Provider** | Anthropic |
| **Model Name** | Claude Sonnet 4.5 |
| **Input Price** | $3.00 / MTok |
| **Output Price** | $15.00 / MTok |
| **Batch Input** | $1.50 / MTok |
| **Batch Output** | $7.50 / MTok |
| **Context Window** | 200,000 tokens |
| **Availability** | Anthropic API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Status** | ✅ Active |

---

### Claude Sonnet 4

| Field | Detail |
|---|---|
| **Provider** | Anthropic |
| **Model Name** | Claude Sonnet 4 |
| **Input Price** | $3.00 / MTok |
| **Output Price** | $15.00 / MTok |
| **Batch Input** | $1.50 / MTok |
| **Batch Output** | $7.50 / MTok |
| **Context Window** | 200,000 tokens (1M token public beta as of Aug 2025) |
| **Availability** | Anthropic API, AWS Bedrock, Google Vertex AI |
| **Status** | ✅ Active |

---

### Claude Haiku 4.5

| Field | Detail |
|---|---|
| **Provider** | Anthropic |
| **Model Name** | Claude Haiku 4.5 |
| **Input Price** | $1.00 / MTok |
| **Output Price** | $5.00 / MTok |
| **5-min Cache Write** | $1.25 / MTok |
| **1-hr Cache Write** | $2.00 / MTok |
| **Cache Hit** | $0.10 / MTok |
| **Context Window** | 200,000 tokens |
| **Availability** | Anthropic API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Status** | ✅ Active |
| **Notes** | Fastest and most affordable model; optimized for high-volume, low-latency tasks. |

---

### Claude Haiku 3.5

| Field | Detail |
|---|---|
| **Provider** | Anthropic |
| **Model Name** | Claude Haiku 3.5 |
| **Input Price** | $0.80 / MTok |
| **Output Price** | $4.00 / MTok |
| **Context Window** | 200,000 tokens |
| **Availability** | Anthropic API, AWS Bedrock, Google Vertex AI |
| **Status** | ✅ Active |

---

### Claude Haiku 3

| Field | Detail |
|---|---|
| **Provider** | Anthropic |
| **Model Name** | Claude Haiku 3 |
| **Input Price** | $0.25 / MTok |
| **Output Price** | $1.25 / MTok |
| **Context Window** | 200,000 tokens |
| **Availability** | Anthropic API, AWS Bedrock, Google Vertex AI |
| **Status** | ✅ Active (legacy) |

---

## Feature-Specific Pricing

### Batch API
- **Discount:** 50% off standard input and output token prices.
- **Use case:** Asynchronous large-volume processing; results within 24 hours.

### Prompt Caching

| Cache Operation | Multiplier | Duration |
|---|---|---|
| 5-minute cache write | 1.25× base input | 5 minutes |
| 1-hour cache write | 2× base input | 1 hour |
| Cache read (hit) | 0.1× base input | Same as preceding write |

> Cache pays off after just one read for 5-minute TTL; after two reads for 1-hour TTL.

### Web Search Tool
- **$10 per 1,000 searches**, plus standard token costs.

### Code Execution Tool
- Free when bundled with web search or web fetch.
- Standalone: 1,550 free hours/month per org; additional hours at **$0.05/hr/container**.

### Fast Mode (Opus 4.6 only, Beta)
- **$30 / MTok input**, **$150 / MTok output** (6× standard rates).
- Not available with Batch API.

### Data Residency
- US-only inference: **+10% pricing multiplier** on all token categories (Opus 4.6 and newer).

---

## Rate Limits
- Enforced by usage tier: Tier 1–4, plus Enterprise custom limits.
- Weekly rate limits added (Aug 2025) specifically for heavy Claude Code users.
- Typical Tier 1 limits (Claude 3 Sonnet example): ~5 RPM, 20K TPM, 300K tokens/day.

## Availability
- **Direct API:** [console.anthropic.com](https://console.anthropic.com)
- **AWS Bedrock:** Regional & global endpoints; regional adds 10% premium (Claude 4.5+ models).
- **Google Vertex AI:** Global, multi-region, and regional endpoints; 10% premium for non-global.
- **Microsoft Foundry:** Available for select models.

---

*Source: [platform.claude.com/docs/en/about-claude/pricing](https://platform.claude.com/docs/en/about-claude/pricing) — Verified 2026-04-11*
