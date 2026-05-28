# 🟠 Anthropic — Claude Model Cards

> **Last updated:** 2026-05-28
> **Source:** https://platform.claude.com/docs/en/about-claude/models/overview (official — verified May 28, 2026) · https://platform.claude.com/docs/en/about-claude/pricing · https://docs.anthropic.com/en/docs/about-claude/model-deprecations · https://claude.com/pricing#api
> **Scraped / verified:** 2026-05-28

All prices are **USD per million tokens (MTok)**. Batch API gives a flat **50% discount** on all models. Prompt caching gives up to **90% off** on repeated input context.

> 🚨 **May 28, 2026 update:** **Claude Opus 4.8 is now the active flagship** — released and confirmed as the new recommended model at `platform.claude.com/docs/en/about-claude/models/overview` (verified May 28, 2026). The official Anthropic pricing page (`claude.com/pricing#api`) now lists **Opus 4.7, Opus 4.6, Sonnet 4.5, Opus 4.5, Opus 4.1, Sonnet 4, and Opus 4** in the Legacy section. **Fast Mode is now available on Opus 4.8 at 2× standard pricing ($10 input / $50 output per MTok)** for up to 2.5× faster speeds. Sonnet 4.6 and Haiku 4.5 remain active at unchanged prices.

---

## 🔒 Restricted / Preview Models (Not Public API)

### Claude Mythos Preview *(Restricted — Project Glasswing)*

> **Announced:** April 7, 2026
> **Status:** 🔒 RESTRICTED — Not publicly available via API
> **Access:** Select organizations only via Project Glasswing (cybersecurity initiative)
> **Capability:** Described as a "step change" over Opus 4.7; 93.9% SWE-bench Verified. Autonomously discovers and exploits zero-day vulnerabilities. Anthropic is committing $100M in usage credits to vetted security organizations.
> **Note:** No public API pricing. Claude Opus 4.8 is the most capable **commercially available** model.

---

## ✅ Active / Recommended Models

### Claude Opus 4.8 *(Current Flagship — Released May 2026)*

> **🆕 NEW (May 28, 2026):** Claude Opus 4.8 is now Anthropic's most capable generally available model, confirmed at `platform.claude.com/docs/en/about-claude/models/overview`. Fast Mode returns: get up to 2.5× faster speeds at 2× standard pricing ($10/$50 per MTok). The `effort` parameter defaults to `high` on all surfaces including the Claude API and Claude Code. Migrate from Opus 4.7 — same per-token price, improved capabilities.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-8` |
| **AWS Bedrock ID** | `anthropic.claude-opus-4-83` (Messages-API Bedrock endpoint only) |
| **Vertex AI ID** | `claude-opus-4-8` |
| **Released** | May 2026 |
| **Status** | ✅ Active — **Current Flagship** |
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
| **Availability** | Claude API, Claude Platform on AWS, Amazon Bedrock (Messages API endpoint), Google Vertex AI, Microsoft Foundry (200k ctx) |
| **Rate limits** | Tiered by usage tier; contact Anthropic for enterprise limits |
| **Notable** | Current top model for complex reasoning and long-horizon agentic coding; adaptive thinking; 1M token context at standard pricing; Fast Mode at 2× base rate for latency-sensitive workloads; Batch API up to 300k output tokens with beta header |

> 📝 **Migration from Opus 4.7:** Per the official Anthropic docs, if you are currently using `claude-opus-4-7`, see the [Migrating to Claude Opus 4.8](https://platform.claude.com/docs/en/about-claude/models/migration-guide#migrating-from-claude-opus-47) guide. Same per-token price ($5/$25), improved capabilities.

> ⚠️ **Fast Mode on Opus 4.8:** Fast Mode costs 2× standard pricing ($10 input / $50 output per MTok) and provides up to 2.5× faster speed. Previously Fast Mode was only available on Opus 4.6 (legacy) at 6× pricing ($30/$150). Opus 4.8's Fast Mode is significantly cheaper (2× vs 6×). Source: `claude.com/pricing#api`, verified May 28, 2026.

> ⚠️ **Bedrock note:** Claude Opus 4.8 is available on Bedrock through the **Messages-API Bedrock endpoint** only. See [Claude in Amazon Bedrock](https://platform.claude.com/docs/en/build-with-claude/claude-in-amazon-bedrock) for details.

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
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Notable** | Improved agentic search; 1M context no premium; extended + adaptive thinking supported; recommended migration target from retired Sonnet 4 (Apr 20, 2026) and legacy Sonnet 4.5 |

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
| **Availability** | API, AWS Bedrock (all regions, self-serve), Google Vertex AI, Microsoft Foundry |
| **Notable** | Fastest model; extended thinking supported; recommended migration target from retired Claude Haiku 3 (retired Feb 19, 2026) and Haiku 3.5 (retired Feb 19, 2026) |

---

## 📊 Thinking Capabilities Matrix (Active Models)

| Model | Extended Thinking | Adaptive Thinking | Notes |
|---|---|---|---|
| Claude Opus 4.8 | ❌ No | ✅ Yes | Best for agentic, coding tasks; Fast Mode at 2× pricing |
| Claude Sonnet 4.6 | ✅ Yes | ✅ Yes | Recommended for reasoning + speed balance |
| Claude Haiku 4.5 | ✅ Yes | ❌ No | Fastest; extended thinking for budget reasoning |

> Source: `platform.claude.com/docs/en/about-claude/models/overview`, verified May 28, 2026.

---

## 🆕 Platform Feature: Claude Security (Enterprise — Public Beta)

> **May 2026:** Anthropic launched **Claude Security** in public beta for Claude Enterprise customers. Purpose-built for security operations workflows including threat detection, vulnerability analysis, and incident response. Billed at standard API token rates using the underlying model. No separate pricing tier announced.

---

## 🆕 Platform Feature: Managed Agents Memory (Public Beta)

> **Apr 25, 2026:** Memory for Claude Managed Agents is now in **public beta** under the standard `managed-agents-2026-04-01` header. This allows agents to persist memory across sessions. No pricing change — billed at standard token rates for the underlying model.

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new projects. **LEGACY** models are still API-accessible at listed prices but have been moved to the "Legacy models" section of Anthropic's official pricing page. **DEPRECATED** models are phasing out. **RETIRED** models return API errors.

---

### ⚠️ LEGACY — Claude Opus 4.7 *(Moved to Legacy May 28, 2026)*

> **Update (May 28, 2026):** Claude Opus 4.7 has been moved to the **"Legacy models"** section on Anthropic's official pricing page (`claude.com/pricing#api`, verified May 28, 2026). The model remains API-accessible at the same price. **Migrate to Claude Opus 4.8** — same price ($5/$25), improved performance, and Fast Mode now available at 2× pricing ($10/$50). Note: Opus 4.7 and Opus 4.6 still support the Batch API `output-300k-2026-03-24` beta header for up to 300k output tokens.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-7` |
| **Released** | April 16, 2026 |
| **Status** | ⚠️ LEGACY — Moved to Legacy section (May 28, 2026); still API-accessible |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Context window** | 1,000,000 tokens |
| **Max output** | 128,000 tokens (sync) / 300,000 tokens (Batch API with `output-300k-2026-03-24` beta header) |
| **Extended thinking** | ❌ No |
| **Adaptive thinking** | ✅ Yes |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry, GitHub Copilot Pro+ |
| **Migration** | Upgrade to **Claude Opus 4.8** — same price ($5/$25), improved performance, Fast Mode now available |

> ✏️ **Tokenizer note:** Opus 4.7 uses a new tokenizer that may produce up to 35% more tokens for the same text compared to Opus 4.6. Monitor actual usage when migrating. Fast Mode was NOT available on Opus 4.7 (it is available on Opus 4.8 at 2× pricing and on Opus 4.6 at 6× pricing).

---

### ⚠️ LEGACY — Claude Opus 4.6 *(Moved to Legacy May 2026)*

> **Update (May 25, 2026):** Claude Opus 4.6 has been moved to the **"Legacy models"** section on Anthropic's official pricing page. The model remains API-accessible at the same price. Migrate to **Claude Opus 4.8** for the current flagship. Note: Fast Mode is also available on Opus 4.8 (at 2× standard / $10/$50) which is cheaper than Opus 4.6's Fast Mode (6× / $30/$150).

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-6` |
| **Released** | February 5, 2026 |
| **Status** | ⚠️ LEGACY — Moved to Legacy section (May 2026); still API-accessible |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode (input)** | $30.00 / MTok *(6× standard — note: Opus 4.8 Fast Mode is cheaper at 2× / $10/$50)* |
| **Fast Mode (output)** | $150.00 / MTok |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Context window** | 1,000,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Migration** | Upgrade to **Claude Opus 4.8** ($5/$25) — same price, improved performance, cheaper Fast Mode (2× vs 6×) |

---

### ⚠️ LEGACY — Claude Sonnet 4.5 *(Moved to Legacy May 2026)*

> **Update (May 25, 2026):** Claude Sonnet 4.5 has been moved to the **"Legacy models"** section on Anthropic's official pricing page. The model remains API-accessible. The 1M-token context window beta (`context-1m-2025-08-07`) was **retired April 30, 2026**. Migrate to **Claude Sonnet 4.6** ($3/$15, 1M context at standard pricing, 64k max output).

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4-5` |
| **Status** | ⚠️ LEGACY — Moved to Legacy section (May 2026); still API-accessible |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **1M context beta** | ❌ **RETIRED April 30, 2026** — `context-1m-2025-08-07` header now has no effect; requests >200K return error |
| **Context window** | 200,000 tokens (standard — 1M beta retired) |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Migration** | Upgrade to **Claude Sonnet 4.6** — same price, 1M context, 64k max output, better performance |

---

### ⚠️ LEGACY — Claude Opus 4.5 *(Moved to Legacy May 2026)*

> **Update (May 25, 2026):** Claude Opus 4.5 has been moved to the **"Legacy models"** section on Anthropic's official pricing page. The model remains API-accessible.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-5` |
| **Released** | November 24, 2025 |
| **Status** | ⚠️ LEGACY — Moved to Legacy section (May 2026); still API-accessible |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Migration** | Upgrade to **Claude Opus 4.8** ($5/$25) — same price, 1M context, 128k max output, much better performance |

---

### ⚠️ LEGACY — Claude Opus 4.1

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-1` |
| **Status** | ⚠️ LEGACY — Available but superseded |
| **Input price** | $15.00 / MTok |
| **Output price** | $75.00 / MTok |
| **Batch input** | $7.50 / MTok |
| **Batch output** | $37.50 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI |
| **Migration** | Upgrade to **Claude Opus 4.8** ($5/$25) — 67% cheaper, far better performance |

---

### ⚠️ LEGACY — Claude Sonnet 4 *(RETIRED April 20, 2026)*

> **Status:** Per the official Anthropic model deprecations page, **Claude Sonnet 4 was retired on April 20, 2026**. All API requests now return errors.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4-20250514` |
| **Status** | ⚠️ LEGACY — **RETIRED April 20, 2026 ❌ API CALLS WILL FAIL** |
| **Input price** | $3.00 / MTok *(last known price — shown for reference only)* |
| **Output price** | $15.00 / MTok *(last known price)* |
| **Availability** | ❌ NONE — All requests return errors |
| **Migration** | Upgrade to **Claude Sonnet 4.6** — same price, 1M context, better performance |

---

### ⚠️ LEGACY — Claude Opus 4 *(RETIRED April 20, 2026)*

> **Status:** Per the official Anthropic model deprecations page, **Claude Opus 4 was retired on April 20, 2026**. All API requests now return errors.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-20250514` |
| **Status** | ⚠️ LEGACY — **RETIRED April 20, 2026 ❌ API CALLS WILL FAIL** |
| **Input price** | $15.00 / MTok *(last known price — shown for reference only)* |
| **Output price** | $75.00 / MTok *(last known price)* |
| **Availability** | ❌ NONE — All requests return errors |
| **Migration** | Upgrade to **Claude Opus 4.8** ($5/$25) — 67% cheaper, far better performance |

---

### ⚠️ LEGACY — Claude Haiku 3.5 *(RETIRED February 19, 2026)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-5-haiku-20241022` |
| **Status** | ⚠️ LEGACY — **RETIRED February 19, 2026 ❌ API CALLS WILL FAIL (Claude API)** |
| **Input price** | $0.80 / MTok *(last known price)* |
| **Output price** | $4.00 / MTok *(last known price)* |
| **Availability** | ❌ Claude API — RETIRED. Bedrock/Vertex AI may retain access on their own schedules. |
| **Migration** | **Migrate to Claude Haiku 4.5** ($1/$5) |

---

### ⚠️ LEGACY — Claude Haiku 3 *(RETIRED February 19, 2026)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-haiku-20240307` |
| **Status** | ⚠️ LEGACY — **RETIRED February 19, 2026 ❌ API CALLS WILL FAIL** |
| **Input price** | $0.25 / MTok *(last known price)* |
| **Output price** | $1.25 / MTok *(last known price)* |
| **Availability** | ❌ NONE — All requests return errors |
| **Migration** | **Migrate to Claude Haiku 4.5 ($1/$5)** |

---

### ⚠️ LEGACY — Claude Sonnet 3.7 *(RETIRED October 28, 2025)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-7-sonnet-20250219` |
| **Status** | ⚠️ LEGACY — **RETIRED October 28, 2025 ❌ API CALLS WILL FAIL** |
| **Input price** | $3.00 / MTok *(last known price)* |
| **Output price** | $15.00 / MTok *(last known price)* |
| **Migration** | Use **Claude Sonnet 4.6** ($3/$15) |

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

> **Status:** RETIRED. API access discontinued.

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
| **Opus 4.7 tokenizer** | New tokenizer may add up to 35% more tokens/request vs Opus 4.6 — monitor per-request spend if using Opus 4.7 (now legacy) |
| **Fast Mode — Opus 4.8** | $10/$50 input/output (2× standard) — up to 2.5× faster speeds |
| **Fast Mode — Opus 4.6 (Legacy only)** | $30/$150 input/output (6× standard) — significantly more expensive than Opus 4.8 Fast Mode |
| **Thinking modes** | Adaptive thinking: Opus 4.8 + Sonnet 4.6. Extended thinking: Sonnet 4.6 + Haiku 4.5 (not on Opus 4.8). |

---

*Sources last verified: May 28, 2026 against the official Anthropic models overview page at `platform.claude.com/docs/en/about-claude/models/overview` (Claude Opus 4.8 confirmed as new flagship, model ID `claude-opus-4-8`, 1M context, 128k max output, adaptive thinking, Fast Mode at 2× pricing), official pricing page at `claude.com/pricing#api` (Opus 4.8 active at $5/$25; Opus 4.7, 4.6, Sonnet 4.5, Opus 4.5, Opus 4.1, Sonnet 4, Opus 4 confirmed in Legacy section), and model deprecations at `docs.anthropic.com/en/docs/about-claude/model-deprecations`. No price changes on active models detected — Opus 4.8 carries forward the same $5/$25 rate as Opus 4.7.*
