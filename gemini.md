# 🔵 Google Gemini — Model Cards

> **Last updated:** 2026-05-21  
> **Sources:** https://ai.google.dev/gemini-api/docs/models · https://ai.google.dev/gemini-api/docs/pricing · https://ai.google.dev/gemini-api/docs/models/gemini-3.5-flash · https://ai.google.dev/gemini-api/docs/models/gemini-3.1-flash-lite · https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5/  
> **Scraped / verified:** 2026-05-21  

All prices are **USD per million tokens (MTok)** unless noted. All current Gemini models support a **1,048,576-token (~1M) context window**. Pro models use **context-tiered pricing** (≤200K vs >200K tokens). Batch API: **50% off**. Context caching: **up to 90% off** repeated prefixes.

> 🆕 **May 21, 2026 update:** Gemini 3.5 Flash added as new stable GA flagship (released May 19, 2026, Google I/O). Gemini 3.1 Flash-Lite stable GA added. Gemini 2.0 Flash officially deprecated — **shutdown June 1, 2026**.

---

## ✅ Active / Recommended Models

### 🆕 Gemini 3.5 Flash *(New Flagship — Released May 19, 2026 — GA Stable)*

> **🆕 ADDED May 21, 2026:** Gemini 3.5 Flash is Google's new stable flagship released at Google I/O 2026 (May 19, 2026). It delivers sustained frontier-level intelligence optimized for real-world agentic tasks, coding, and long-horizon workflows. It outperforms Gemini 3.1 Pro Preview on challenging coding and agentic benchmarks at a *lower price point*, and runs 4× faster than other frontier models. This is the default model for the Gemini app, AI Mode in Google Search, Google Antigravity, and the Gemini API.

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI / Gemini app) |
| **Model ID** | `gemini-3.5-flash` |
| **Released** | May 19, 2026 (Google I/O 2026) |
| **Status** | ✅ Active — **Current Flagship (Stable GA)** |
| **Input price (standard)** | $1.50 / MTok |
| **Output price (standard, incl. thinking tokens)** | $9.00 / MTok |
| **Batch input** | $0.75 / MTok |
| **Batch output** | $4.50 / MTok |
| **Priority input** | $2.70 / MTok |
| **Priority output** | $16.20 / MTok |
| **Flex input** | $0.75 / MTok |
| **Flex output** | $4.50 / MTok |
| **Context caching price** | $0.15 / MTok (standard); $1.00 / MTok / hr (storage) |
| **Grounding with Google Search** | 5,000 prompts/month free (shared across Gemini 3); then $14 / 1,000 queries |
| **Grounding with Google Maps** | 5,000 prompts/month free; then $14 / 1,000 queries |
| **Context window** | 1,048,576 tokens (~1M) |
| **Max output** | 65,536 tokens |
| **Knowledge cutoff** | January 2025 |
| **Availability** | Google AI Studio API (free tier + paid), Vertex AI / Gemini Enterprise Agent Platform, Google Antigravity, Gemini app (global default), AI Mode in Search |
| **Multimodal** | Text, Image, Video, Audio, PDF inputs; Text output |
| **Capabilities** | Batch API ✓, Context caching ✓, Code execution ✓, File search ✓, Flex inference ✓, Function calling ✓, Grounding with Google Maps ✓, Priority inference ✓, Search grounding ✓, Structured outputs ✓, Thinking ✓, URL context ✓ |
| **Notable** | New stable GA flagship (May 19, 2026); outperforms Gemini 3.1 Pro Preview on Terminal-Bench 2.1 (76.2%), GDPval-AA (1656 Elo), MCP Atlas (83.6%), CharXiv Reasoning (84.2%); 4× faster than other frontier models; designed for agentic sub-agent deployment, multi-step workflows, long-horizon coding; powers Gemini Spark (24/7 personal AI agent); $1.50 input is 25% cheaper than 3.1 Pro Preview ($2.00) at better performance |

> 📝 **vs Gemini 3.1 Pro Preview:** 3.5 Flash ($1.50/$9.00) outperforms 3.1 Pro Preview ($2.00/$12.00) on agentic and coding benchmarks while being faster and cheaper. For most new use cases, prefer 3.5 Flash. Use 3.1 Pro Preview for workloads that specifically need the Pro-class model while 3.5 Pro is still in development.

> 📝 **Gemini 3.5 Pro:** Coming next month (June 2026) — already in internal use at Google. Will be the highest-capability model in the 3.5 series.

---

### Gemini 3.1 Pro Preview

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-3.1-pro-preview` |
| **Released** | March 9, 2026 (replaced Gemini 3 Pro Preview) |
| **Status** | ✅ Active — Flagship (Preview) *(superseded by Gemini 3.5 Flash for most workloads)* |
| **Input price (≤200K tokens)** | $2.00 / MTok |
| **Input price (>200K tokens)** | $4.00 / MTok |
| **Output price (≤200K tokens)** | $12.00 / MTok |
| **Output price (>200K tokens)** | $18.00 / MTok |
| **Batch input (≤200K)** | $1.00 / MTok |
| **Batch output (≤200K)** | $6.00 / MTok |
| **Flex input (≤200K)** | $1.00 / MTok |
| **Priority input (≤200K)** | $3.60 / MTok |
| **Priority output (≤200K)** | $21.60 / MTok |
| **Context caching** | $0.20 (≤200K) / $0.40 (>200K) per MTok; $4.50 / MTok / hr storage |
| **Context window** | 1,000,000 tokens |
| **Availability** | Google AI Studio API (paid tier), Vertex AI |
| **Multimodal** | Text, code, audio, images, video |
| **Notable** | Google's most capable **reasoning** model (Preview tier); GPQA Diamond competitive with GPT-5.4; use when maximum Pro-class reasoning depth is required and 3.5 Pro is not yet available |

> ⚠️ Preview model — pricing may change before GA. Gemini 3 Pro Preview was **deprecated/shut down March 9, 2026** — migrate to 3.1 Pro Preview.

---

### 🆕 Gemini 3.1 Flash-Lite *(Stable GA — May 2026)*

> **🆕 ADDED May 21, 2026:** Gemini 3.1 Flash-Lite now has a stable GA version (`gemini-3.1-flash-lite`), updated May 2026. Same pricing as the preview version. The stable model supports Thinking, Batch API, Caching, and the full multimodal input suite.

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-3.1-flash-lite` *(stable)* |
| **Released / Updated** | May 2026 (stable GA) |
| **Status** | ✅ Active — High-Volume Budget (Stable GA) |
| **Input price (standard)** | $0.25 / MTok (text / image / video); $0.50 / MTok (audio) |
| **Output price (standard, incl. thinking tokens)** | $1.50 / MTok |
| **Batch input** | $0.125 / MTok (text/image/video); $0.25 / MTok (audio) |
| **Batch output** | $0.75 / MTok |
| **Priority input** | $0.45 / MTok (text/image/video); $0.90 / MTok (audio) |
| **Priority output** | $2.70 / MTok |
| **Context caching** | $0.025 (text/image/video); $0.05 (audio); $1.00 / MTok / hr storage |
| **Context window** | 1,048,576 tokens (~1M) |
| **Max output** | 65,536 tokens |
| **Knowledge cutoff** | January 2025 |
| **Availability** | Google AI Studio (free tier + paid), Vertex AI |
| **Multimodal** | Text, Image, Video, Audio, PDF inputs; Text output |
| **Capabilities** | Batch API ✓, Caching ✓, Code execution ✓, File search ✓, Flex inference ✓, Function calling ✓, Grounding ✓, Priority inference ✓, Search grounding ✓, Structured outputs ✓, Thinking ✓, URL context ✓ |
| **Notable** | Low-latency, cost-effective; optimized for high-volume agentic tasks, translation, transcription, lightweight data extraction; model routing classifier; thinking (`thinking_level` param) for better accuracy |

---

### Gemini 3.1 Flash-Lite Preview

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-3.1-flash-lite-preview` |
| **Released** | March 2026 |
| **Status** | ✅ Active — Cost-Efficient (Preview) |
| **Input price** | $0.25 / MTok (text / image / video); $0.50 / MTok (audio) |
| **Output price** | $1.50 / MTok |
| **Context window** | 1,048,576 tokens (~1M) |
| **Availability** | Google AI Studio (free tier limited), Vertex AI |
| **Multimodal** | Text, code, images, audio, video, PDF |
| **Notable** | Preview version — use stable `gemini-3.1-flash-lite` for new production deployments |

---

### Gemini 2.5 Pro

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-2.5-pro` |
| **Released** | 2025 |
| **Status** | ✅ Active — GA Flagship (2.5 series) |
| **Input price (≤200K tokens)** | $1.25 / MTok |
| **Input price (>200K tokens)** | $2.50 / MTok |
| **Output price (≤200K tokens)** | $10.00 / MTok |
| **Output price (>200K tokens)** | $15.00 / MTok |
| **Batch input** | $0.625 / MTok (≤200K) |
| **Batch output** | $5.00 / MTok (≤200K) |
| **Flex input** | $0.625 / MTok |
| **Priority input** | $2.25 / MTok |
| **Priority output** | $18.00 / MTok |
| **Context caching** | $0.125 (≤200K) per MTok; $4.50 / MTok / hr storage |
| **Grounding with Google Search** | 1,500 RPD (free), then $35 / 1,000 grounded prompts |
| **Context window** | 1,000,000 tokens |
| **Availability** | Google AI Studio (paid tier), Vertex AI |
| **Multimodal** | Text, code, audio, images, video |
| **Notable** | Best GA model for deep coding and reasoning; $1.25 input undercuts GPT-5.4 ($2.50); leading Chatbot Arena scores; supports thinking/reasoning tokens |

---

### Gemini 2.5 Flash

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-2.5-flash` |
| **Released** | 2025 |
| **Status** | ✅ Active — Balanced GA |
| **Input price (standard)** | $0.30 / MTok (text/image/video); $1.00 / MTok (audio) |
| **Output price (standard, incl. thinking tokens)** | $2.50 / MTok |
| **Batch input** | $0.15 / MTok |
| **Batch output** | $1.25 / MTok |
| **Priority input** | $0.54 / MTok |
| **Priority output** | $4.50 / MTok |
| **Context caching** | $0.03 / MTok; $1.00 / MTok / hr storage |
| **Grounding with Google Search** | 1,500 RPD free (shared with Flash-Lite); then $35 / 1,000 grounded prompts |
| **Context window** | 1,000,000 tokens |
| **Availability** | Google AI Studio (free tier), Vertex AI |
| **Multimodal** | Text, code, audio, images, video |
| **Notable** | Excellent price-performance; hybrid reasoning (thinking budgets enabled via API); 1M context at flat pricing |

---

### Gemini 2.5 Flash-Lite

| Field | Value |
|---|---|
| **Provider** | Google (AI Studio / Vertex AI) |
| **Model ID** | `gemini-2.5-flash-lite` |
| **Released** | July 22, 2025 |
| **Status** | ✅ Active — Budget / High-Volume GA |
| **Input price (standard)** | $0.10 / MTok (text/image/video); $0.30 / MTok (audio) |
| **Output price (standard, incl. thinking tokens)** | $0.40 / MTok |
| **Batch input** | $0.05 / MTok |
| **Batch output** | $0.20 / MTok |
| **Priority input** | $0.18 / MTok |
| **Priority output** | $0.72 / MTok |
| **Context caching** | $0.01 / MTok; $1.00 / MTok / hr storage |
| **Context window** | 1,048,576 tokens |
| **Availability** | Google AI Studio (free tier), Vertex AI |
| **Multimodal** | Text, code, images, audio, video |
| **Notable** | Cheapest GA Gemini model; thinking disabled by default (enable via API); best for classification, routing, extraction |

---

## ⚠️ Legacy / Deprecated / Retired Models

### ⚠️ LEGACY — Gemini 2.0 Flash *(DEPRECATED — Shutdown June 1, 2026)*

> **⚠️ STATUS CHANGE (May 21, 2026):** Gemini 2.0 Flash was previously listed as Active. The official Gemini API pricing page (ai.google.dev/gemini-api/docs/pricing, verified May 21, 2026) now shows a **DEPRECATED** warning: "Gemini 2.0 Flash is deprecated and will be shut down June 1, 2026. Migrate to a newer model to avoid service disruption."

| Field | Value |
|---|---|
| **Provider** | Google |
| **Model ID** | `gemini-2.0-flash` |
| **Status** | ⚠️ LEGACY — **DEPRECATED · Shutdown: June 1, 2026** |
| **Last price (text/image/video)** | $0.10 input / $0.40 output per MTok |
| **Context window** | 1,000,000 tokens |
| **Migration** | Migrate to **Gemini 2.5 Flash** ($0.30/$2.50) for better capabilities, or **Gemini 3.5 Flash** ($1.50/$9.00) for frontier agentic performance |

---

### ⚠️ LEGACY — Gemini 2.0 Flash-Lite *(DEPRECATED — Shutdown June 1, 2026)*

| Field | Value |
|---|---|
| **Provider** | Google |
| **Model ID** | `gemini-2.0-flash-lite` |
| **Status** | ⚠️ LEGACY — **DEPRECATED · Shutdown: June 1, 2026** |
| **Last price** | $0.075 input / $0.30 output per MTok |
| **Migration** | Migrate to **Gemini 2.5 Flash-Lite** ($0.10/$0.40) |

---

### ⚠️ LEGACY — Gemini 3 Pro Preview *(RETIRED March 9, 2026)*

| Field | Value |
|---|---|
| **Provider** | Google |
| **Model ID** | `gemini-3-pro-preview` |
| **Status** | ⚠️ LEGACY — **RETIRED March 9, 2026 / Shut down** |
| **Migration** | Migrate to **Gemini 3.1 Pro Preview** or **Gemini 3.5 Flash** |

---

### ⚠️ LEGACY — Gemini 1.5 Series

| Model | Status | Migration |
|---|---|---|
| Gemini 1.5 Pro | ⚠️ LEGACY | → Gemini 2.5 Pro or Gemini 3.5 Flash |
| Gemini 1.5 Flash | ⚠️ LEGACY | → Gemini 2.5 Flash or Gemini 3.5 Flash |
| Gemini 1.5 Flash-8B | ⚠️ LEGACY | → Gemini 2.5 Flash-Lite |

---

## 💡 Cost Optimization Notes

| Feature | Details |
|---|---|
| **Batch API** | 50% off all paid models for async workloads (24 hr turnaround) |
| **Context caching** | ~90% off repeated input prefixes (cache reads at ~10% of base input rate) — best for RAG and repeated system prompts |
| **Context tier (Pro models)** | 2.5 Pro and 3.1 Pro double input cost for prompts >200K tokens — keep prompts under 200K if possible |
| **Free tier** | Google AI Studio offers free access to select models (2.5 Flash, 2.5 Flash-Lite, 3.1 Flash-Lite, 3.5 Flash on free tier) with rate limits |
| **Thinking tokens** | Reasoning (thinking) tokens billed as output — can increase costs for complex queries |
| **Grounding pricing** | Gemini 2.5 models: $35/1K for Pro, included free up to 1,500 RPD. Gemini 3.x models: $14/1K search queries (5,000/month free, shared across Gemini 3) |
| **Model routing** | Typical optimal split: 5% Pro / 30% 3.5 Flash / 40% 2.5 Flash / 25% Flash-Lite — reduces effective cost by 60–70% vs all-Pro |
| **Priority tier** | 1.8× standard pricing — use for latency-critical production workloads needing guaranteed throughput |
| **3.5 Flash vs 3.1 Pro** | 3.5 Flash ($1.50/$9.00) outperforms 3.1 Pro ($2.00/$12.00) on agentic/coding benchmarks at lower cost — prefer 3.5 Flash for new builds |
| **June 1, 2026 deadline** | Gemini 2.0 Flash and 2.0 Flash-Lite shut down June 1 — migrate immediately |

---

*Sources last verified: May 21, 2026 against ai.google.dev/gemini-api/docs/pricing (Gemini 3.5 Flash pricing confirmed, Gemini 2.0 Flash deprecation confirmed), ai.google.dev/gemini-api/docs/models (full active model listing), ai.google.dev/gemini-api/docs/models/gemini-3.5-flash (context window 1,048,576; max output 65,536; capabilities), ai.google.dev/gemini-api/docs/models/gemini-3.1-flash-lite (stable GA confirmed May 2026), blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-5/ (May 19, 2026 launch blog post).*
