# 🔵 Google Gemini — Model Cards

> **Last updated:** 2026-04-12  
> **Sources:** https://ai.google.dev/gemini-api/docs/pricing · https://cloud.google.com/vertex-ai/generative-ai/pricing · https://www.metacto.com/blogs/the-true-cost-of-google-gemini-a-guide-to-api-pricing-and-integration · https://www.finout.io/blog/gemini-pricing-in-2026  
> **Scraped / verified:** 2026-04-12  

All prices are **USD per million tokens (MTok)**. All current Gemini models support a **1,000,000-token context window**. Pro models use **context-tiered pricing** (≤200K vs >200K tokens). Batch API: **50% off**. Context caching: **up to 90% off** repeated prefixes.

---

## ✅ Active / Recommended Models

### Gemini 3.1 Pro Preview *(Preview — Latest Flagship)*

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-3.1-pro-preview` |
| **Released** | March 9, 2026 (replaced Gemini 3 Pro Preview) |
| **Status** | ✅ Active — **Latest Flagship (Preview)** |
| **Input price (≤200K tokens)** | $2.00 / MTok |
| **Input price (>200K tokens)** | $4.00 / MTok |
| **Output price (≤200K tokens)** | $12.00 / MTok |
| **Output price (>200K tokens)** | $18.00 / MTok |
| **Context window** | 1,000,000 tokens |
| **Availability** | Google AI Studio API (paid tier), Vertex AI |
| **Multimodal** | Text, code, audio, images, video |
| **Notable** | Google's most capable reasoning model; GPQA Diamond scores competitive with GPT-5.4; production pricing expected to settle ~$1.50/$10 in GA (Q2 2026) |

> ⚠️ Preview model — pricing may change before GA. Gemini 3 Pro Preview was **deprecated March 9, 2026**. Migrate to 3.1 Pro Preview.

---

### Gemini 3.1 Flash-Lite Preview

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-3.1-flash-lite-preview` |
| **Released** | March 2026 |
| **Status** | ✅ Active — Cost-Efficient (Preview) |
| **Input price** | $0.25 / MTok |
| **Output price** | $1.50 / MTok |
| **Context window** | 1,000,000 tokens |
| **Availability** | Google AI Studio (free tier limited), Vertex AI |
| **Multimodal** | Text, code, images |
| **Notable** | Fastest model in the 3.x generation; high-volume workloads; flat pricing (no context tier surcharge) |

---

### Gemini 2.5 Pro

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-2.5-pro` |
| **Released** | 2025 |
| **Status** | ✅ Active — GA Flagship |
| **Input price (≤200K tokens)** | $1.25 / MTok |
| **Input price (>200K tokens)** | $2.50 / MTok |
| **Output price (≤200K tokens)** | $10.00 / MTok |
| **Output price (>200K tokens)** | $15.00 / MTok |
| **Batch input** | $0.625 / MTok |
| **Batch output** | $5.00 / MTok |
| **Context window** | 1,000,000 tokens |
| **Availability** | Google AI Studio (paid tier), Vertex AI |
| **Multimodal** | Text, code, audio, images, video |
| **Notable** | Best GA model for coding; $1.25 input undercuts GPT-5.4 ($2.50); leading Chatbot Arena scores; supports thinking/reasoning tokens |

---

### Gemini 2.5 Flash

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-2.5-flash` |
| **Released** | 2025 |
| **Status** | ✅ Active — Balanced |
| **Input price** | $0.30 / MTok |
| **Output price** | $2.50 / MTok |
| **Batch input** | $0.15 / MTok |
| **Batch output** | $1.25 / MTok |
| **Context window** | 1,000,000 tokens |
| **Availability** | Google AI Studio (free tier), Vertex AI |
| **Multimodal** | Text, code, audio, images, video |
| **Notable** | Excellent price-performance; hybrid reasoning (thinking can be enabled via API); 1M context with flat pricing |

---

### Gemini 2.5 Flash-Lite

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-2.5-flash-lite` |
| **Released** | July 22, 2025 |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.40 / MTok |
| **Batch input** | $0.05 / MTok |
| **Batch output** | $0.20 / MTok |
| **Context window** | 1,048,576 tokens |
| **Availability** | Google AI Studio (free tier), Vertex AI |
| **Multimodal** | Text, code, images |
| **Notable** | Lowest-cost GA Gemini model; thinking disabled by default (enable via API); best for classification, routing, extraction |

---

### Gemini 2.0 Flash

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-2.0-flash` |
| **Released** | 2024 |
| **Status** | ✅ Active — Previous-Gen Workhorse |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.40 / MTok |
| **Context window** | 1,000,000 tokens |
| **Availability** | Google AI Studio (free tier), Vertex AI |
| **Multimodal** | Text, code, audio, images, video |
| **Notable** | Still supported; superseded by 2.5 Flash-Lite for most new workloads |

---

## ⚠️ Legacy / Deprecated / Retired Models

### ⚠️ LEGACY — Gemini 2.0 Flash-Lite *(DEPRECATED — shutting down June 1, 2026)*

| Field | Value |
|---|---|
| **Provider** | Google |
| **Model ID** | `gemini-2.0-flash-lite` |
| **Status** | ⚠️ LEGACY — **DEPRECATED · Shutdown: June 1, 2026** |
| **Last price** | $0.075 input / $0.30 output per MTok |
| **Migration** | Migrate to **Gemini 2.5 Flash-Lite** ($0.10/$0.40) |

---

### ⚠️ LEGACY — Gemini 3 Pro Preview *(RETIRED)*

| Field | Value |
|---|---|
| **Provider** | Google |
| **Model ID** | `gemini-3-pro-preview` |
| **Status** | ⚠️ LEGACY — **RETIRED March 9, 2026** |
| **Migration** | Migrate to **Gemini 3.1 Pro Preview** |

---

### ⚠️ LEGACY — Gemini 1.5 Series

| Model | Status | Migration |
|---|---|---|
| Gemini 1.5 Pro | ⚠️ LEGACY | → Gemini 2.5 Pro |
| Gemini 1.5 Flash | ⚠️ LEGACY | → Gemini 2.5 Flash |
| Gemini 1.5 Flash-8B | ⚠️ LEGACY | → Gemini 2.5 Flash-Lite |

---

## 💡 Cost Optimization Notes

| Feature | Details |
|---|---|
| **Batch API** | 50% off all paid models for async workloads (24 hr turnaround) |
| **Context caching** | 90% off repeated input prefixes (cache reads at 10% of base input rate) — best for RAG and repeated system prompts |
| **Context tier** | Pro models double input cost for prompts >200K tokens — keep prompts under 200K if possible |
| **Free tier** | Google AI Studio offers free access to select models (2.5 Flash, 2.5 Flash-Lite, 3.1 Flash-Lite) with rate limits |
| **Thinking tokens** | Reasoning (thinking) tokens are billed as output — can increase costs for complex queries |
| **Grounding** | Grounding with Google Search: $35/1K requests for Pro models, $14/1K for Flash models (1,500/500 RPD free) |
| **Model routing** | Typical optimal split: 10% Pro / 60% Flash / 30% Flash-Lite — reduces effective cost by 60-70% vs all-Pro |

---

*Sources verified April 12, 2026.*
