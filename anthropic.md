# 🟠 Anthropic — Claude Model Cards

> **Last updated:** 2026-04-11  
> **Source:** https://www.metacto.com/blogs/anthropic-api-pricing-a-full-breakdown-of-costs-and-integration · https://platform.claude.com/docs/en/about-claude/pricing · https://platform.claude.com/docs/en/release-notes/overview  
> **Scraped / verified:** 2026-04-11  

All prices are **USD per million tokens (MTok)**. Batch API gives a flat **50% discount** on all models. Prompt caching gives up to **90% off** on repeated input context.

---

## ✅ Active / Recommended Models

### Claude Opus 4.6

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-6` |
| **Released** | February 5, 2026 |
| **Status** | ✅ Active — Flagship |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode (input)** | $30.00 / MTok |
| **Fast Mode (output)** | $150.00 / MTok |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Context window** | 1,000,000 tokens (at standard pricing — no surcharge) |
| **Max output** | 32,000 tokens (sync) / 300,000 tokens (Batch API with beta header) |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Rate limits** | Tiered by usage tier; contact Anthropic for enterprise limits |
| **Notable** | Full 1M context at standard rate; Fast Mode 6× pricing for low-latency; extended thinking billed as output tokens |

---

### Claude Sonnet 4.6

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4-6` |
| **Released** | February 17, 2026 |
| **Status** | ✅ Active — Balanced |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Cache write (5 min)** | $3.75 / MTok |
| **Cache write (1 hr)** | $6.00 / MTok |
| **Cache read** | $0.30 / MTok |
| **Batch input** | $1.50 / MTok |
| **Batch output** | $7.50 / MTok |
| **Context window** | 1,000,000 tokens (at standard pricing — no surcharge) |
| **Max output** | 16,000 tokens (sync) / 300,000 tokens (Batch API with beta header) |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Notable** | Improved agentic search; 1M context no premium; extended thinking supported; 1M beta for Sonnet 4.5 retired April 30 2026 — migrate here |

---

### Claude Haiku 4.5

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-haiku-4-5` |
| **Released** | Late 2025 |
| **Status** | ✅ Active — Speed / Volume |
| **Input price** | $1.00 / MTok |
| **Output price** | $5.00 / MTok |
| **Cache write (5 min)** | $1.25 / MTok |
| **Cache write (1 hr)** | $2.00 / MTok |
| **Cache read** | $0.10 / MTok |
| **Batch input** | $0.50 / MTok |
| **Batch output** | $2.50 / MTok |
| **Context window** | 200,000 tokens |
| **Max output** | 8,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Notable** | Fastest model; extended thinking supported; recommended replacement for Haiku 3 and Haiku 3.5 |

---

### Claude Opus 4.5

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-5` |
| **Released** | November 24, 2025 |
| **Status** | ✅ Active — Previous Flagship |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache read** | $0.50 / MTok |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Notable** | Strong coding and reasoning; same price as Opus 4.6 but 200K context |

---

### Claude Sonnet 4.5

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4-5` |
| **Released** | 2025 |
| **Status** | ✅ Active |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Long context input (>200K)** | $6.00 / MTok *(beta retiring April 30, 2026)* |
| **Long context output (>200K)** | $22.50 / MTok *(beta retiring April 30, 2026)* |
| **Cache write (5 min)** | $3.75 / MTok |
| **Cache read** | $0.30 / MTok |
| **Batch input** | $1.50 / MTok |
| **Batch output** | $7.50 / MTok |
| **Context window** | 200,000 tokens standard; 1M via beta (retiring April 30, 2026) |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Notable** | Migrate to Sonnet 4.6 for 1M context at standard pricing |

---

### Claude Sonnet 4

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4` |
| **Status** | ✅ Supported (older generation) |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Batch input** | $1.50 / MTok |
| **Batch output** | $7.50 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI |
| **Notable** | 1M context beta retiring April 30, 2026 — migrate to Sonnet 4.6 |

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new projects. Some have been retired entirely (API calls return errors). Migrate to current-generation models.

---

### ⚠️ LEGACY — Claude Opus 4.1

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-1` |
| **Status** | ⚠️ LEGACY — Available but superseded |
| **Input price** | $15.00 / MTok |
| **Output price** | $75.00 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI |
| **Migration** | Upgrade to **Claude Opus 4.6** ($5/$25) — 67% cheaper, better performance |

---

### ⚠️ LEGACY — Claude Opus 4

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4` |
| **Status** | ⚠️ LEGACY — Available but superseded |
| **Input price** | $15.00 / MTok |
| **Output price** | $75.00 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI |
| **Migration** | Upgrade to **Claude Opus 4.6** ($5/$25) — 67% cheaper, better performance |

---

### ⚠️ LEGACY — Claude Haiku 3 *(DEPRECATED — retiring April 19, 2026)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-haiku-20240307` |
| **Status** | ⚠️ LEGACY — **DEPRECATED · Retirement: April 19, 2026** |
| **Input price** | $0.25 / MTok |
| **Output price** | $1.25 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API (until April 19, 2026 only) |
| **Migration** | Migrate to **Claude Haiku 4.5** ($1/$5) immediately |

---

### ⚠️ LEGACY — Claude Haiku 3.5 *(RETIRED)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-5-haiku-20241022` |
| **Status** | ⚠️ LEGACY — **RETIRED** (API calls return errors) |
| **Last price** | $0.80 input / $4.00 output per MTok |
| **Migration** | Use **Claude Haiku 4.5** ($1/$5) |

---

### ⚠️ LEGACY — Claude Sonnet 3.7 *(RETIRED)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-7-sonnet-20250219` |
| **Status** | ⚠️ LEGACY — **RETIRED February 19, 2026** (API calls return errors) |
| **Last price** | $3.00 input / $15.00 output per MTok |
| **Migration** | Use **Claude Sonnet 4.6** ($3/$15) |

---

### ⚠️ LEGACY — Claude 3 Series *(RETIRED)*

| Model | Status | Migration |
|---|---|---|
| Claude 3 Opus | ⚠️ RETIRED (Jan 5, 2026) | → Claude Opus 4.6 |
| Claude 3.5 Sonnet (v1 & v2) | ⚠️ RETIRED | → Claude Sonnet 4.6 |
| Claude 3 Sonnet | ⚠️ RETIRED | → Claude Sonnet 4.6 |
| Claude 3 Haiku | ⚠️ RETIRING April 19, 2026 | → Claude Haiku 4.5 |

---

### ⚠️ LEGACY — Claude 2.x Series *(RETIRED)*

| Model | Last Known Price |
|---|---|
| Claude 2.0 / 2.1 | ~$8.00 input / $24.00 output per MTok |

> **Status:** RETIRED. API access discontinued. Migrate to current Claude 4 generation.

---

## 💡 Cost Optimization Notes

| Feature | Savings |
|---|---|
| **Batch API** | 50% off input + output (all models, 24 hr turnaround) |
| **Prompt caching — cache read (5-min TTL)** | 90% off repeated input tokens |
| **Prompt caching — cache write (5-min TTL)** | 1.25× standard input (break-even after 2 reads) |
| **Prompt caching — cache write (1-hr TTL)** | 2× standard input (break-even after 8 reads) |
| **Batch + caching stacked** | Up to 95% total cost reduction |
| **US-only inference (data residency)** | 1.1× pricing on models released after Feb 1, 2026 |

---

*Sources verified April 11, 2026.*
