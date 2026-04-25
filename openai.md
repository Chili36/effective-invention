# 🟢 OpenAI — Model Cards

> **Last updated:** 2026-04-25  
> **Source:** https://openai.com/api/pricing/ · https://openai.com/index/introducing-gpt-5-5/ · https://developers.openai.com/api/docs/pricing · https://www.aipricing.guru/openai-pricing/ · https://www.cloudzero.com/blog/openai-pricing/  
> **Scraped / verified:** 2026-04-25  

All prices are **USD per million tokens (MTok)** unless noted. Batch API gives a flat **50% discount** on all models. Cached input tokens get **50–90% off** depending on model.

> **Context tiers for GPT-5.4:** Standard pricing applies for prompts **under 272K tokens**. Long-context (>272K) tier applies a surcharge. GPT-5.5 uses **flat pricing** with no context tier surcharge at standard rates.

---

## 🔒 Restricted / Preview Models (Not General API)

### GPT-5.4-Cyber *(Restricted — Limited Access)*

> **Announced:** April 14, 2026  
> **Status:** 🔒 RESTRICTED — Not generally available via public API  
> **Access:** Vetted security vendors, organizations, and researchers only via OpenAI's Trusted Access for Cyber program. Higher verification tiers unlock more permissive capabilities.  
> **Capability:** Fine-tuned variant of GPT-5.4, optimized for defensive cybersecurity.  
> **Note:** No public API pricing.

---

## ✅ Active / Recommended Models

### GPT-5.5 *(🆕 NEW FLAGSHIP — Released April 23-24, 2026)*

> **🆕 UPDATE (Apr 25, 2026):** GPT-5.5 launched April 23, 2026 in ChatGPT and Codex; became available in the API on **April 24, 2026**. It is now OpenAI's most capable and most expensive standard model. First fully retrained base model since GPT-4.5 — natively omnimodal (text, image, audio, video). Tops the Artificial Analysis Intelligence Index at score 60, 3 points ahead of Claude Opus 4.7 and Gemini 3.1 Pro. Note: API price doubled vs GPT-5.4 ($2.50→$5.00 input) — OpenAI argues token efficiency offsets ~20% of the increase.

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.5` |
| **Released** | April 23, 2026 (ChatGPT/Codex) · April 24, 2026 (API) |
| **Status** | ✅ Active — **Current Flagship** |
| **Input price** | $5.00 / MTok |
| **Cached input** | $0.50 / MTok *(~90% discount)* |
| **Output price** | $30.00 / MTok |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $15.00 / MTok |
| **Context window** | 1,000,000 tokens (API) / 400,000 tokens (Codex) |
| **Max output** | 128,000 tokens |
| **Availability** | API (Responses + Chat Completions), ChatGPT Plus/Pro/Business/Enterprise, Codex |
| **Rate limits** | Regional processing (data residency) endpoints: +10% uplift |
| **Notable** | First fully retrained base since GPT-4.5; natively omnimodal (text+image+audio+video); Terminal-Bench 2.0: 82.7% (#1); SWE-bench Pro: 58.6%; GDPval: 84.9%; OSWorld-Verified: 78.7%; FrontierMath Tier 4: 35.4%; AI Index score 60 (#1 overall); token-efficient (fewer retries vs GPT-5.4 for agent tasks); Codex Fast mode: 1.5× speed, 2.5× cost |

> ⚠️ **Pricing vs GPT-5.4:** GPT-5.5 standard ($5/$30) is 2× the per-token price of GPT-5.4 standard ($2.50/$15). OpenAI claims ~40% token reduction for Codex workloads, netting ~20% higher effective cost vs GPT-5.4 at equivalent quality. Measure on your own traffic before migrating high-volume workloads.

---

### GPT-5.5 Pro

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.5-pro` |
| **Released** | April 24, 2026 (API) |
| **Status** | ✅ Active — Ultra-Premium |
| **Input price** | $30.00 / MTok |
| **Output price** | $180.00 / MTok |
| **Context window** | 1,000,000 tokens |
| **Availability** | API; ChatGPT Pro/Business/Enterprise only |
| **Rate limits** | Regional processing: +10% uplift |
| **Notable** | Extra parallel test-time compute on harder questions; BrowseComp 90.1% vs 84.4% standard; designed for legal, financial, scientific, and deep research workloads |

---

### GPT-5.4 *(released March 5, 2026)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4` |
| **Released** | March 5, 2026 |
| **Status** | ✅ Active — Previous Flagship *(superseded by GPT-5.5)* |
| **Input price (short ctx <272K)** | $2.50 / MTok |
| **Cached input (short ctx)** | $0.25 / MTok |
| **Output price (short ctx)** | $15.00 / MTok |
| **Input price (long ctx >272K)** | $5.00 / MTok |
| **Cached input (long ctx)** | $0.50 / MTok |
| **Output price (long ctx)** | $22.50 / MTok |
| **Batch input** | $1.25 / MTok |
| **Batch output** | $7.50 / MTok |
| **Context window** | 1,050,000 tokens (922K input + 128K output) |
| **Max output** | 128,000 tokens |
| **Availability** | API |
| **Rate limits** | Regional processing endpoints: +10% uplift |
| **Notable** | Unifies Codex and GPT into one architecture; 57.7% SWE-bench Pro; 75% OSWorld; multimodal (text + image); native computer-use capabilities. Still recommended for cost-sensitive workloads vs GPT-5.5 |

---

### GPT-5.4 Pro

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4-pro` |
| **Released** | March 2026 |
| **Status** | ✅ Active — Previous Ultra-Premium *(superseded by GPT-5.5 Pro at same price)* |
| **Input price** | $30.00 / MTok |
| **Output price** | $180.00 / MTok |
| **Context window** | 1,050,000 tokens |
| **Availability** | API |
| **Rate limits** | Regional processing: +10% uplift |
| **Notable** | Maximum reasoning depth; for highest-complexity professional workloads; GPT-5.5 Pro replaces at identical pricing with better benchmarks |

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
| **Notable** | 54.38% SWE-bench Pro (≈90% of flagship quality at ~6× lower cost vs GPT-5.4); as of April 2026, most competitive mid-tier model on the market |

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
| **Notable** | Cheapest proprietary model in the GPT-5.4 family; ideal for classification, extraction, high-volume simple tasks |

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
| **Notable** | 1M context window at lower cost than GPT-5.4; better instruction-following and coding vs GPT-4o; now available in ChatGPT model picker |

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

### o3-pro *(Reasoning model — Maximum Depth)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `o3-pro` |
| **Status** | ✅ Active — Maximum Reasoning |
| **Input price** | $20.00 / MTok |
| **Output price** | $80.00 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API |
| **Notable** | 10× more expensive than o3; designed for the hardest reasoning problems where accuracy justifies premium; BrowseComp and FrontierMath-class tasks |

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

> Not recommended for new projects. Migrate to current GPT-5.5, GPT-5.4, or GPT-4.1 family.

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
| **Migration** | Move to **GPT-5.5** or **GPT-5.4** for better performance |

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
| **Migration** | Move to **GPT-5.4** ($2.50/$15) or **GPT-5.5** ($5/$30) |

> **Note:** GPT-5.2 Thinking variant retires **June 5, 2026**.

---

### ⚠️ LEGACY — GPT-5.1 *(RETIRED March 11, 2026)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model IDs** | `gpt-5.1`, `gpt-5.1-instant`, `gpt-5.1-thinking`, `gpt-5.1-pro` |
| **Status** | ⚠️ LEGACY — **RETIRED March 11, 2026** |
| **Note** | Replaced by GPT-5.3 Instant, GPT-5.4 Thinking, and GPT-5.4 Pro respectively |
| **Migration** | Use **GPT-5.5** family for equivalent capabilities |

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
| **Migration** | Use **o3** ($2/$8) or **o3-pro** ($20/$80) — covers most o1 reasoning use cases at lower cost |

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
| **GPT-5.4 short vs long ctx** | Stay under 272K input to avoid 2× surcharge |
| **GPT-5.5 vs GPT-5.4 routing** | GPT-5.5 at $5/$30 is 2× the per-token cost of GPT-5.4 $2.50/$15 — route only agent-heavy workloads to 5.5 |
| **Regional processing** | +10% uplift for GPT-5.5 and GPT-5.4 family data residency endpoints |
| **Model tiering** | GPT-4.1 nano ($0.10/M) → GPT-4.1 mini ($0.40/M) → GPT-4.1 ($2/M) → GPT-5.4 ($2.50/M) → GPT-5.5 ($5/M) — choose by task complexity |
| **Reasoning models** | o4-mini ($1.10/M) → o3 ($2/M) → o3-pro ($20/M); use o3-pro only for hardest reasoning tasks |

---

*Sources last verified: April 25, 2026 against openai.com/api/pricing/, openai.com/index/introducing-gpt-5-5/, developers.openai.com/api/docs/pricing, aipricing.guru/openai-pricing/*
