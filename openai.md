# 🟢 OpenAI — Model Cards

> **Last updated:** 2026-04-16  
> **Source:** https://openai.com/api/pricing/ · https://pecollective.com/tools/openai-api-pricing/ · https://devtk.ai/en/blog/openai-api-pricing-guide-2026/ · https://help.openai.com/en/articles/9624314-model-release-notes  
> **Scraped / verified:** 2026-04-16 (no pricing changes since Apr 15 — date bump only)  

All prices are **USD per million tokens (MTok)** unless noted. Batch API gives a flat **50% discount** on all models. Cached input tokens get **50–90% off** depending on model.

> **Context tiers for GPT-5.4:** Standard pricing applies for prompts **under 270K tokens**. Long-context (>270K) tier applies a surcharge. See per-model table below.

---

## 🔒 Restricted / Preview Models (Not General API)

### GPT-5.4-Cyber *(Restricted — Limited Access)*

> **Announced:** April 14, 2026  
> **Status:** 🔒 RESTRICTED — Not generally available via public API  
> **Access:** Vetted security vendors, organizations, and researchers only via OpenAI's Trusted Access for Cyber program (launched February 2026). Higher verification tiers unlock more permissive capabilities.  
> **Capability:** Fine-tuned variant of GPT-5.4, optimized for defensive cybersecurity; fewer restrictions on vulnerability research and analysis for authorized users.  
> **Note:** No public API pricing. Broader rollout expected to "thousands of partners" in coming weeks, but still restricted to vetted participants.  

---

## ✅ Active / Recommended Models

### GPT-5.4 *(released March 5, 2026)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4` |
| **Released** | March 5, 2026 |
| **Status** | ✅ Active — Current Flagship |
| **Input price (short ctx <270K)** | $2.50 / MTok |
| **Cached input (short ctx)** | $0.25 / MTok |
| **Output price (short ctx)** | $15.00 / MTok |
| **Input price (long ctx >270K)** | $5.00 / MTok |
| **Cached input (long ctx)** | $0.50 / MTok |
| **Output price (long ctx)** | $22.50 / MTok |
| **Batch input** | $1.25 / MTok |
| **Batch output** | $7.50 / MTok |
| **Context window** | 1,050,000 tokens (922K input + 128K output) |
| **Max output** | 128,000 tokens |
| **Availability** | API |
| **Rate limits** | Regional processing endpoints: +10% uplift |
| **Notable** | Unifies Codex and GPT into one architecture; 57.7% SWE-bench Pro; 75% OSWorld; multimodal (text + image); native computer-use capabilities |

---

### GPT-5.4 Pro

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4-pro` |
| **Released** | March 2026 |
| **Status** | ✅ Active — Ultra-Premium |
| **Input price** | $30.00 / MTok |
| **Output price** | $180.00 / MTok |
| **Context window** | 1,050,000 tokens |
| **Availability** | API |
| **Rate limits** | Regional processing: +10% uplift |
| **Notable** | Maximum reasoning depth; for highest-complexity professional workloads |

---

### GPT-5.4 mini *(released March 17, 2026)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4-mini` |
| **Released** | March 17, 2026 |
| **Status** | ✅ Active — Mid-Tier |
| **Input price** | $0.75 / MTok |
| **Cached input** | $0.075 / MTok |
| **Output price** | $4.50 / MTok |
| **Batch input** | $0.375 / MTok |
| **Batch output** | $2.25 / MTok |
| **Context window** | 400,000 tokens |
| **Availability** | API; ChatGPT Free/Go via Thinking feature |
| **Rate limits** | Regional processing: +10% uplift |
| **Notable** | 54.38% SWE-bench Pro (≈90% of flagship quality at ~6× lower cost) |

---

### GPT-5.4 nano *(released March 17, 2026)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4-nano` |
| **Released** | March 17, 2026 |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.20 / MTok |
| **Cached input** | $0.020 / MTok |
| **Output price** | $1.25 / MTok |
| **Batch input** | $0.10 / MTok |
| **Batch output** | $0.625 / MTok |
| **Context window** | 400,000 tokens |
| **Availability** | API |
| **Rate limits** | Regional processing: +10% uplift |
| **Notable** | Cheapest proprietary model; ideal for classification, extraction, high-volume simple tasks |

---

### GPT-4.1

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4.1` |
| **Released** | April 14, 2025 |
| **Status** | ✅ Active — Recommended for long-context workloads |
| **Input price** | $2.00 / MTok |
| **Cached input** | $0.50 / MTok |
| **Output price** | $8.00 / MTok |
| **Batch input** | $1.00 / MTok |
| **Batch output** | $4.00 / MTok |
| **Context window** | 1,040,000 tokens |
| **Availability** | API; ChatGPT Plus/Pro/Team (model picker) |
| **Notable** | Recommended replacement for GPT-4o; better instruction-following, coding, long-context; cheaper than GPT-4o ($2.50/$10); now available in ChatGPT model picker |

---

### GPT-4.1 mini

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4.1-mini` |
| **Status** | ✅ Active — Balanced, Long-Context Budget |
| **Input price** | $0.40 / MTok |
| **Cached input** | $0.10 / MTok |
| **Output price** | $1.60 / MTok |
| **Batch input** | $0.20 / MTok |
| **Batch output** | $0.80 / MTok |
| **Context window** | 1,000,000 tokens |
| **Availability** | API; fallback model for ChatGPT paid users |
| **Notable** | 4× cheaper than GPT-4.1 with the same 1M context window; replaces GPT-4o mini in ChatGPT model picker for paid users |

---

### GPT-4.1 nano

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4.1-nano` |
| **Status** | ✅ Active — Budget long-context |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.40 / MTok |
| **Batch input** | $0.05 / MTok |
| **Batch output** | $0.20 / MTok |
| **Context window** | 1,000,000+ tokens |
| **Availability** | API |
| **Notable** | One of the cheapest capable models with 1M+ context; ideal for document chunking pipelines |

---

### o3 *(Reasoning model)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `o3` |
| **Status** | ✅ Active — Reasoning Flagship |
| **Input price** | $2.00 / MTok |
| **Cached input** | $0.50 / MTok |
| **Output price** | $8.00 / MTok |
| **Batch input** | $1.00 / MTok |
| **Batch output** | $4.00 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API |
| **Notable** | Chain-of-thought reasoning; best for math, logic, multi-step coding; reasoning tokens billed as output |

---

### o4-mini *(Reasoning model)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `o4-mini` |
| **Status** | ✅ Active — Budget Reasoning |
| **Input price** | $1.10 / MTok |
| **Cached input** | $0.275 / MTok |
| **Output price** | $4.40 / MTok |
| **Batch input** | $0.55 / MTok |
| **Batch output** | $2.20 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API |
| **Notable** | Replaced o3-mini; best value reasoning model; outperforms o3-mini on most benchmarks |

---

## ⚠️ Legacy / Deprecated / Retired Models

> Not recommended for new projects. Migrate to current GPT-5.4 or GPT-4.1 family.

---

### ⚠️ LEGACY — GPT-5.3 / Codex *(being phased out)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.3` / `gpt-5.3-codex` |
| **Status** | ⚠️ LEGACY — Being phased out (June 2026 target retirement) |
| **Input price** | $1.75 / MTok |
| **Output price** | $14.00 / MTok |
| **Context window** | 400,000 tokens |
| **Migration** | Move to **GPT-5.4** for better performance at comparable cost |

---

### ⚠️ LEGACY — GPT-5.2

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.2` |
| **Status** | ⚠️ LEGACY — Retiring June 2026 |
| **Input price** | $1.75 / MTok |
| **Output price** | $14.00 / MTok |
| **Context window** | 400,000 tokens |
| **Migration** | Move to **GPT-5.4** ($2.50/$15) |

---

### ⚠️ LEGACY — GPT-5.1 *(RETIRED March 11, 2026)*

> **🆕 UPDATE (Apr 15, 2026):** GPT-5.1 models were retired from ChatGPT and the API as of March 11, 2026. Existing conversations were automatically migrated to successor models.

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model IDs** | `gpt-5.1`, `gpt-5.1-instant`, `gpt-5.1-thinking`, `gpt-5.1-pro` |
| **Status** | ⚠️ LEGACY — **RETIRED March 11, 2026** |
| **Note** | Replaced by GPT-5.3 Instant, GPT-5.4 Thinking, and GPT-5.4 Pro respectively |
| **Migration** | Use **GPT-5.4** family for equivalent capabilities |

---

### ⚠️ LEGACY — GPT-4o

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4o` |
| **Released** | May 13, 2024 |
| **Status** | ⚠️ LEGACY — Superseded by GPT-4.1 |
| **Input price** | $2.50 / MTok |
| **Cached input** | $1.25 / MTok |
| **Output price** | $10.00 / MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Migrate to **GPT-4.1** ($2/$8, 1M context) — cheaper and larger context |

---

### ⚠️ LEGACY — GPT-4o mini

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4o-mini` |
| **Status** | ⚠️ LEGACY |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.60 / MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Migrate to **GPT-5.4 nano** ($0.20/$1.25) or **GPT-4.1 nano** ($0.10/$0.40) |

---

### ⚠️ LEGACY — o1 *(Deep Reasoning)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `o1` |
| **Status** | ⚠️ LEGACY — Very expensive, limited use cases |
| **Input price** | $15.00 / MTok |
| **Output price** | $60.00 / MTok |
| **Context window** | 200,000 tokens |
| **Migration** | Use **o3** ($2/$8) — covers most o1 reasoning use cases at 87% lower cost |

---

### ⚠️ LEGACY — GPT-4 Turbo / GPT-3.5 Turbo *(RETIRED)*

| Model | Status |
|---|---|
| GPT-4 Turbo | ⚠️ RETIRED |
| GPT-3.5 Turbo | ⚠️ RETIRED |

---

## 💡 Cost Optimization Notes

| Feature | Savings |
|---|---|
| **Batch API** | 50% off all tokens (24 hr turnaround) — all models |
| **Cached input tokens** | 50–90% off depending on model |
| **GPT-5.4 short vs long ctx** | Stay under 270K input to avoid 2× surcharge |
| **Regional processing** | +10% uplift for GPT-5.4 family data residency endpoints |
| **Model tiering** | GPT-4.1 nano ($0.10/M) → GPT-4.1 mini ($0.40/M) → GPT-4.1 ($2/M) → GPT-5.4 ($2.50/M) — choose by task complexity |

---

*Sources last verified: April 16, 2026 against openai.com/api/pricing/, help.openai.com/en/articles/9624314-model-release-notes, and pecollective.com/tools/openai-api-pricing/ — no pricing changes since Apr 15 2026*
