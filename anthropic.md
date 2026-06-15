# 🟠 Anthropic — Claude Model Cards

> **Last updated:** 2026-06-15
> **Source:** https://platform.claude.com/docs/en/about-claude/pricing · https://claude.com/pricing#api · https://www.anthropic.com/claude/mythos
> **Scraped / verified:** 2026-06-15 — Claude Sonnet 4 + Opus 4 confirmed RETIRED as of June 15, 2026; all active prices re-verified unchanged.

All prices are **USD per million tokens (MTok)**. Batch API gives a flat **50% discount** on all models. Prompt caching gives up to **90% off** on repeated input context.

> 🚨 **June 9, 2026 — BREAKING: Claude Fable 5 + Mythos 5 launched.** Claude Fable 5 (`claude-fable-5`) is Anthropic's most capable widely released model, now the new top of the Claude lineup at **$10/$50 per MTok**. Claude Mythos 5 (`claude-mythos-5`) joins Project Glasswing (limited access). Full launch details: `anthropic.com/news/claude-fable-5-mythos-5`.
>
> - Claude Opus 4.8 remains the recommended model for complex reasoning and agentic coding for most developers ("daily driver"). Fable 5 is positioned for the most ambitious, long-running, asynchronous work.
> - Cybersecurity and biology queries to Fable 5 automatically fall back to Opus 4.8 — you are **not** charged Fable 5 prices for rerouted requests.
> - Fable 5 requires **30-day data retention** for safety monitoring.

> ✅ **Claude Sonnet 4 + Opus 4 RETIRED on June 15, 2026. ❌** API calls to `claude-sonnet-4-20250514` and `claude-opus-4-20250514` now return errors. Migration: Sonnet 4 → Sonnet 4.6 (same price, 1M context); Opus 4 → Opus 4.8 ($5/$25, 67% cheaper).

---

## 🔒 Restricted / Preview Models (Limited Access)

### Claude Mythos 5 *(Project Glasswing — Limited Availability)*

> **Launched:** June 9, 2026
> **Status:** 🔒 LIMITED — Available to approved customers via [Project Glasswing](https://anthropic.com/glasswing) only
> **Access:** AWS Bedrock (limited availability) · Google Vertex AI (limited availability) · Contact your Anthropic, AWS, or Google Cloud account team
> **Pricing:** $10 / MTok input · $50 / MTok output (same as Fable 5)
> **Context:** 1M tokens · Max output: 128K tokens
> **Capabilities:** Adaptive thinking (always on); no extended thinking. Successor to Claude Mythos Preview within Project Glasswing.
> **Note:** Not generally available. To get access to Mythos 5 for cybersecurity and biology research, [sign up for notifications](https://claude.com/form/mythos-access-interest).

### Claude Mythos Preview *(Restricted — Project Glasswing)*

> **Status:** 🔒 RESTRICTED — Superseded by Claude Mythos 5 within Project Glasswing (June 9, 2026)
> **Note:** Claude Mythos Preview has been replaced by Claude Mythos 5 as the Project Glasswing model.

---

## ✅ Active / Recommended Models

### Claude Fable 5 *(New Top-Tier — Released June 9, 2026)*

> **🆕 NEW (June 9, 2026):** Claude Fable 5 is Anthropic's most capable widely released model. It is built for ambitious, long-running, asynchronous work — multi-day agentic sessions, complex migrations, enterprise workflows, and hard knowledge work. It represents a new 5th model generation. Model ID: `claude-fable-5`. Available immediately on Claude API, AWS Bedrock, Vertex AI, and Microsoft Foundry.
>
> ⚠️ **Safety fallback:** Cybersecurity and biology queries are automatically rerouted to Claude Opus 4.8 by Fable 5's built-in safeguards — those requests are billed at Opus 4.8 rates, not Fable 5 rates.
>
> ⚠️ **Data retention:** Using Fable 5 requires 30-day data retention for safety monitoring ([learn more](https://support.claude.com/en/articles/15425996)).

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-fable-5` |
| **AWS Bedrock ID** | `anthropic.claude-fable-5` |
| **Vertex AI ID** | `claude-fable-5` |
| **Released** | June 9, 2026 |
| **Status** | ✅ Active — **Top-Tier / Most Capable** |
| **Input price** | $10.00 / MTok |
| **Output price** | $50.00 / MTok |
| **Cache write (5 min)** | $12.50 / MTok |
| **Cache write (1 hr)** | $20.00 / MTok |
| **Cache read** | $1.00 / MTok |
| **Batch input** | $5.00 / MTok *(50% off)* |
| **Batch output** | $25.00 / MTok *(50% off)* |
| **US-only inference** | 1.1× pricing ($11.00 input / $55.00 output) |
| **Context window** | 1,000,000 tokens |
| **Max output** | 128,000 tokens |
| **Extended thinking** | ❌ No |
| **Adaptive thinking** | ✅ Yes (always on) |
| **Availability** | Claude API · Claude Platform on AWS · Amazon Bedrock · Google Vertex AI · Microsoft Foundry |
| **Safety fallback** | Cybersecurity/biology queries auto-route to Opus 4.8 — billed at Opus 4.8 rates |
| **Data retention** | 30-day data retention required for safety monitoring |
| **Notable** | Most capable Anthropic model for general release; long-horizon agentic coding (CursorBench #1); multi-day autonomous sessions; vision for design fidelity; enterprise deep research and analysis; new 5th generation architecture; self-validates work and writes its own tests |

> 📝 **When to use Fable 5 vs Opus 4.8:** Use Fable 5 for problems you couldn't solve with previous models — multi-day autonomous tasks, complex migrations, long-horizon R&D. Use Opus 4.8 for everyday complex reasoning and agentic coding at half the per-token cost.

---

### Claude Opus 4.8 *(Daily Driver — Recommended for Most Developers)*

> **May 28, 2026 — Opus 4.8** is Anthropic's most capable Opus-tier model for complex reasoning, long-horizon agentic coding, and high-autonomy work. Following the June 9 launch of Fable 5, Opus 4.8 is the recommended "daily driver" for most developers. Fast Mode available at 2× pricing for latency-sensitive workloads.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-8` |
| **AWS Bedrock ID** | `anthropic.claude-opus-4-83` (Messages-API Bedrock endpoint only) |
| **Vertex AI ID** | `claude-opus-4-8` |
| **Released** | May 2026 |
| **Status** | ✅ Active — **Most Capable Opus-Tier / Daily Driver** |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode (input)** | $10.00 / MTok *(2× standard — up to 2.5× faster speeds)* |
| **Fast Mode (output)** | $50.00 / MTok |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Context window** | 1,000,000 tokens (standard API) · 200,000 tokens (Microsoft Foundry only) |
| **Max output** | 128,000 tokens (sync) / 300,000 tokens (Batch API with `output-300k-2026-03-24` beta header) |
| **Knowledge cutoff (reliable)** | January 2026 |
| **Training data cutoff** | January 2026 |
| **Extended thinking** | ❌ No |
| **Adaptive thinking** | ✅ Yes |
| **Effort param default** | `high` on all surfaces (Claude API, Claude Code, etc.) — set `effort` explicitly for other levels |
| **Availability** | Claude API · Claude Platform on AWS · Amazon Bedrock (Messages API endpoint) · Google Vertex AI · Microsoft Foundry (200k ctx) |
| **Notable** | Best-value daily driver for complex reasoning and agentic coding; 1M context at standard pricing; Fast Mode at 2× base rate; Batch API up to 300k output tokens with beta header; safety fallback for Fable 5 cybersecurity/biology queries |

> ⚠️ **Bedrock note:** Claude Opus 4.8 is available on Bedrock through the **Messages-API Bedrock endpoint** only.

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
| **Max output** | 64,000 tokens (sync) / 300,000 tokens (Batch API with `output-300k-2026-03-24` beta header) |
| **Knowledge cutoff (reliable)** | August 2025 |
| **Training data cutoff** | January 2026 |
| **Extended thinking** | ✅ Yes |
| **Adaptive thinking** | ✅ Yes |
| **Availability** | API · AWS Bedrock · Google Vertex AI · Microsoft Foundry |
| **Notable** | Optimal balance of intelligence, cost, and speed; 1M context no premium; extended + adaptive thinking; recommended migration target from retired Sonnet 4 |

---

### Claude Haiku 4.5

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-haiku-4-5` *(alias for `claude-haiku-4-5-20251001`)* |
| **Released** | October 2025 |
| **Status** | ✅ Active — Speed / Volume |
| **Input price** | $1.00 / MTok |
| **Output price** | $5.00 / MTok |
| **Cache write (5 min)** | $1.25 / MTok |
| **Cache write (1 hr)** | $2.00 / MTok |
| **Cache read** | $0.10 / MTok |
| **Batch input** | $0.50 / MTok |
| **Batch output** | $2.50 / MTok |
| **Context window** | 200,000 tokens |
| **Max output** | 64,000 tokens |
| **Knowledge cutoff (reliable)** | February 2025 |
| **Training data cutoff** | July 2025 |
| **Extended thinking** | ✅ Yes |
| **Adaptive thinking** | ❌ No |
| **Availability** | API · AWS Bedrock (all regions, self-serve) · Google Vertex AI · Microsoft Foundry |
| **Notable** | Fastest model; extended thinking supported; cheapest model in the Claude lineup |

---

## 📊 Thinking Capabilities Matrix (Active Models)

| Model | Extended Thinking | Adaptive Thinking | Notes |
|---|---|---|---|
| Claude Fable 5 | ❌ No | ✅ Yes (always on) | Top-tier; autonomous long-horizon work; safety fallback on cyber/bio queries |
| Claude Opus 4.8 | ❌ No | ✅ Yes | Recommended daily driver; Fast Mode at 2× pricing |
| Claude Sonnet 4.6 | ✅ Yes | ✅ Yes | Best for reasoning + speed balance |
| Claude Haiku 4.5 | ✅ Yes | ❌ No | Fastest; extended thinking for budget reasoning |

> Source: `platform.claude.com/docs/en/about-claude/models/overview`, verified June 15, 2026.

---

## 🆕 Platform Feature: Fallback API (Fable 5)

> **June 9, 2026:** API customers using Claude Fable 5 must configure the **Fallback API** (`support.claude.com/en/articles/15363606`) so that cybersecurity/biology queries automatically route to Opus 4.8. Claude.ai and other hosted surfaces handle the fallback automatically.

---

## 🆕 Platform Feature: Claude Security (Enterprise — Public Beta)

> **May 2026:** Anthropic launched **Claude Security** in public beta for Claude Enterprise customers. Purpose-built for security operations workflows. Billed at standard API token rates using the underlying model.

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new projects. **LEGACY** = still API-accessible but in the provider's legacy section. **DEPRECATED** = still accessible, published retirement date. **RETIRED** = API calls return errors ❌.

---

### ⚠️ LEGACY — Claude Opus 4.7 *(Moved to Legacy May 28, 2026)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-7` |
| **Status** | ⚠️ LEGACY — Still API-accessible; moved to Legacy section May 28, 2026 |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode (input)** | $30.00 / MTok *(6× standard — far more expensive than Opus 4.8 Fast Mode at 2×)* |
| **Fast Mode (output)** | $150.00 / MTok |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok |
| **Context window** | 1,000,000 tokens |
| **Max output** | 128,000 tokens (sync) / 300,000 tokens (Batch API with `output-300k-2026-03-24` beta header) |
| **Migration** | Upgrade to **Claude Opus 4.8** — same price ($5/$25), improved performance, much cheaper Fast Mode (2× vs 6×) |

---

### ⚠️ LEGACY — Claude Opus 4.6 *(Moved to Legacy May 2026)*

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-6` |
| **Status** | ⚠️ LEGACY — Still API-accessible |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode** | $30.00 / $150.00 per MTok (6×) |
| **Context window** | 1,000,000 tokens |
| **Migration** | → **Claude Opus 4.8** ($5/$25, cheaper Fast Mode at 2×) |

---

### ⚠️ LEGACY — Claude Sonnet 4.5 *(Moved to Legacy May 2026)*

| Field | Value |
|---|---|
| **Model ID** | `claude-sonnet-4-5` |
| **Status** | ⚠️ LEGACY — 1M context beta RETIRED April 30, 2026; max context now 200K |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Migration** | → **Claude Sonnet 4.6** (same price, 1M context, 64k output) |

---

### ⚠️ LEGACY — Claude Opus 4.5 *(Moved to Legacy May 2026)*

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-5` |
| **Status** | ⚠️ LEGACY — Still API-accessible |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Context window** | 200,000 tokens |
| **Migration** | → **Claude Opus 4.8** ($5/$25, 1M context, 128k output) |

---

### ⚠️ LEGACY — Claude Opus 4.1

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-1` |
| **Status** | ⚠️ LEGACY (deprecated) |
| **Input price** | $15.00 / MTok |
| **Output price** | $75.00 / MTok |
| **Migration** | → **Claude Opus 4.8** ($5/$25) — 67% cheaper, far better performance |

---

### ⚠️ RETIRED — Claude Sonnet 4 *(Retired June 15, 2026 ❌)*

| Field | Value |
|---|---|
| **Model ID** | `claude-sonnet-4-20250514` |
| **Status** | ⚠️ RETIRED — **API calls return errors ❌ — Retired June 15, 2026** |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Migration** | → **Claude Sonnet 4.6** — same price, 1M context |

---

### ⚠️ RETIRED — Claude Opus 4 *(Retired June 15, 2026 ❌)*

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-20250514` |
| **Status** | ⚠️ RETIRED — **API calls return errors ❌ — Retired June 15, 2026** |
| **Input price** | $15.00 / MTok |
| **Output price** | $75.00 / MTok |
| **Migration** | → **Claude Opus 4.8** ($5/$25) — 67% cheaper |

---

### ⚠️ LEGACY — Claude Haiku 3.5 *(RETIRED February 19, 2026 on Claude API)*

| Field | Value |
|---|---|
| **Model ID** | `claude-3-5-haiku-20241022` |
| **Status** | ⚠️ LEGACY — **RETIRED February 19, 2026 ❌ API CALLS WILL FAIL (Claude API)** — still on Bedrock/Vertex AI |
| **Input price** | $0.80 / MTok *(last known)* |
| **Output price** | $4.00 / MTok *(last known)* |
| **Migration** | → **Claude Haiku 4.5** ($1/$5) |

---

### ⚠️ LEGACY — Claude Haiku 3 *(RETIRED February 19, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `claude-3-haiku-20240307` |
| **Status** | ⚠️ LEGACY — **RETIRED February 19, 2026 ❌ API CALLS WILL FAIL** |
| **Migration** | → **Claude Haiku 4.5** ($1/$5) |

---

### ⚠️ LEGACY — Claude Sonnet 3.7 *(RETIRED October 28, 2025)*

| Field | Value |
|---|---|
| **Model ID** | `claude-3-7-sonnet-20250219` |
| **Status** | ⚠️ LEGACY — **RETIRED October 28, 2025 ❌ API CALLS WILL FAIL** |
| **Migration** | → **Claude Sonnet 4.6** ($3/$15) |

---

### ⚠️ LEGACY — Claude 3 Series

| Model | Status | Migration |
|---|---|---|
| Claude 3 Opus | ⚠️ DEPRECATED Jan 2026 — available by request for paying customers | → Claude Opus 4.8 |
| Claude 3.5 Sonnet (v1 & v2) | ⚠️ **RETIRED January 5, 2026** | → Claude Sonnet 4.6 |
| Claude 3 Sonnet | ⚠️ RETIRED | → Claude Sonnet 4.6 |
| Claude 3 Haiku | ⚠️ **RETIRED February 19, 2026 ❌** | → Claude Haiku 4.5 |

---

### ⚠️ LEGACY — Claude 2.x Series *(RETIRED)*

| Model | Last Known Price |
|---|---|
| Claude 2.0 / 2.1 | ~$8.00 input / $24.00 output per MTok |

---

## 💡 Cost Optimization Notes

| Feature | Savings |
|---|---|
| **Batch API** | 50% off input + output (all models, 24 hr turnaround) |
| **Prompt caching — cache read (5-min TTL)** | 90% off repeated input tokens |
| **Prompt caching — cache write (5-min TTL)** | 1.25× standard input (break-even after 2 reads) |
| **Prompt caching — cache write (1-hr TTL)** | 2× standard input (break-even after 8 reads) |
| **Fable 5 vs Opus 4.8** | Fable 5 at $10/$50 is 2× the per-token cost of Opus 4.8 ($5/$25) — route only problems requiring multi-day autonomous work to Fable 5 |
| **US-only inference (data residency)** | 1.1× pricing on Opus 4.6, Sonnet 4.6, Fable 5 and later models |
| **Opus 4.8 Fast Mode** | $10/$50 (2× standard) — up to 2.5× faster speeds |
| **Fable 5 safety fallback** | Cybersecurity/biology queries auto-route to Opus 4.8 and are billed at Opus 4.8 rates |
| **Thinking modes** | Adaptive: Fable 5 + Opus 4.8 + Sonnet 4.6. Extended: Sonnet 4.6 + Haiku 4.5. |
| **⚠️ Sonnet 4 + Opus 4 RETIRED** | **Retired June 15, 2026 ❌** — API calls return errors — Sonnet 4 → Sonnet 4.6, Opus 4 → Opus 4.8 |

---

*Sources last verified: June 15, 2026 against `claude.com/pricing#api` and `platform.claude.com/docs/en/about-claude/pricing` — Claude Sonnet 4 (`claude-sonnet-4-20250514`) RETIRED ❌ June 15, 2026; Claude Opus 4 (`claude-opus-4-20250514`) RETIRED ❌ June 15, 2026; Fable 5 $10/$50 re-confirmed; Mythos 5 $10/$50 limited access re-confirmed; Opus 4.8 $5/$25 re-confirmed; Sonnet 4.6 $3/$15 re-confirmed; Haiku 4.5 $1/$5 re-confirmed; all cache/batch pricing unchanged.*
