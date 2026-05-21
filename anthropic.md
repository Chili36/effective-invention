# 🟠 Anthropic — Claude Model Cards

> **Last updated:** 2026-05-21  
> **Source:** https://platform.claude.com/docs/en/about-claude/pricing (official — verified May 21, 2026) · https://docs.anthropic.com/en/docs/about-claude/model-deprecations · https://platform.claude.com/docs/en/release-notes/overview · https://releasebot.io/updates/anthropic  
> **Scraped / verified:** 2026-05-21  

All prices are **USD per million tokens (MTok)**. Batch API gives a flat **50% discount** on all models. Prompt caching gives up to **90% off** on repeated input context.

> ✅ **May 21, 2026 re-verification:** All active model prices confirmed unchanged since May 18, 2026. No new retirements or price changes detected.

---

## 🔒 Restricted / Preview Models (Not Public API)

### Claude Mythos Preview *(Restricted — Project Glasswing)*

> **Announced:** April 7, 2026  
> **Status:** 🔒 RESTRICTED — Not publicly available via API  
> **Access:** Select organizations only via Project Glasswing (cybersecurity initiative)  
> **Capability:** Described as a "step change" over Opus 4.7; 93.9% SWE-bench Verified. Autonomously discovers and exploits zero-day vulnerabilities. Anthropic is committing $100M in usage credits to vetted security organizations.  
> **Note:** No public API pricing. Claude Opus 4.7 is the most capable **commercially available** model.  

---

## ✅ Active / Recommended Models

### Claude Opus 4.7 *(Current Flagship — Released April 16, 2026)*

> **Updated May 11, 2026:** Claude Opus 4.7 remains Anthropic's most capable generally available model. Available in Bedrock console self-serve across 27 AWS regions.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-7` |
| **Released** | April 16, 2026 |
| **Status** | ✅ Active — **Current Flagship** |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Context window** | 1,000,000 tokens (at standard pricing — no surcharge) |
| **Max output** | 32,000 tokens (sync) / 300,000 tokens (Batch API with `output-300k-2026-03-24` beta header) |
| **Availability** | API, Claude Platform, AWS Bedrock (all regions, self-serve), Google Vertex AI, Microsoft Foundry, GitHub Copilot Pro+ |
| **Rate limits** | Tiered by usage tier; contact Anthropic for enterprise limits |
| **Notable** | `xhigh` effort level (coding/agentic tasks); **task budgets beta** (caps token spend in agentic loops); `/ultrareview` (multi-agent code review in Claude Code); **3.75MP vision** (2,576px long edge); **new tokenizer** (up to 35% more tokens/request vs Opus 4.6 — same price/token but monitor per-request costs); automated cybersecurity safeguard detection/blocking; SWE-bench Verified 87.6%; GPQA Diamond 94.2%; CursorBench 70%; US-only data residency: 1.1× multiplier |

> ⚠️ **Tokenizer change:** Opus 4.7 uses a new tokenizer that may produce up to 35% more tokens for the same text compared to Opus 4.6. The per-token price is unchanged at $5/$25, but your effective cost per request may increase depending on content type. Monitor actual usage after migration.

> ✏️ **Fast Mode correction (May 11, 2026):** A previous version of this card listed Fast Mode ($30/$150) for Opus 4.7. This was incorrect. Per the **official Anthropic pricing page** (platform.claude.com/docs/en/about-claude/pricing, verified May 21, 2026), Fast Mode (beta) is available **only on Claude Opus 4.6**, not Opus 4.7. See the Opus 4.6 card below for Fast Mode details.

---

### Claude Opus 4.6

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-6` |
| **Released** | February 5, 2026 |
| **Status** | ✅ Active — Previous Flagship *(superseded by Opus 4.7)* |
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
| **Notable** | Full 1M context at standard rate; **Fast Mode 6× pricing** for low-latency (only Opus model with Fast Mode); extended thinking billed as output tokens; US-only data residency: 1.1× multiplier |

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
| **Notable** | Improved agentic search; 1M context no premium; extended thinking supported; recommended migration target from Sonnet 4 (retired Apr 20, 2026) and Sonnet 4.5 |

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
| **Max output** | 8,000 tokens |
| **Availability** | API, AWS Bedrock (all regions, self-serve), Google Vertex AI, Microsoft Foundry |
| **Notable** | Fastest model; extended thinking supported; recommended migration target from retired Claude Haiku 3 (retired Feb 19, 2026) and Haiku 3.5 (retired Feb 19, 2026) |

---

### Claude Opus 4.5

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-5` |
| **Released** | November 24, 2025 |
| **Status** | ✅ Active — Previous Generation |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache read** | $0.50 / MTok |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Notable** | Strong coding and reasoning; same price as Opus 4.7 but 200K context and older generation |

---

### Claude Sonnet 4.5

> ✅ **CONFIRMED (May 4, 2026):** The 1M-token context window beta (`context-1m-2025-08-07`) for **Claude Sonnet 4.5 was officially retired on April 30, 2026.** The beta header now has no effect. Requests exceeding the standard 200K-token context window return an error. Migrate to **Claude Sonnet 4.6**, which supports 1M context at standard pricing with no beta header required.

> ⚠️ **DEPRECATION ADVISORY:** Claude Sonnet 4.5 retirement date has not been formally announced as of May 21, 2026. However, given Claude Sonnet 4 and Opus 4 retired April 20, 2026, plan migration to **Claude Sonnet 4.6** promptly.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4-5` |
| **Released** | 2025 |
| **Status** | ✅ Active (200K context) — *formal retirement date pending announcement* |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **1M context beta** | ❌ **RETIRED April 30, 2026** — `context-1m-2025-08-07` header now has no effect; requests >200K return error |
| **Cache write (5 min)** | $3.75 / MTok |
| **Cache read** | $0.30 / MTok |
| **Batch input** | $1.50 / MTok |
| **Batch output** | $7.50 / MTok |
| **Context window** | 200,000 tokens (standard — 1M beta retired) |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Notable** | Migrate to Sonnet 4.6 for 1M context at standard pricing. |

---

## 🆕 Platform Feature: Claude Security (Enterprise — Public Beta)

> **May 2026:** Anthropic launched **Claude Security** in public beta for Claude Enterprise customers. Purpose-built for security operations workflows including threat detection, vulnerability analysis, and incident response. Billed at standard API token rates using the underlying model. No separate pricing tier announced.

---

## 🆕 Platform Feature: Managed Agents Memory (Public Beta)

> **Apr 25, 2026:** Memory for Claude Managed Agents is now in **public beta** under the standard `managed-agents-2026-04-01` header. This allows agents to persist memory across sessions. No pricing change — billed at standard token rates for the underlying model.

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new projects. **DEPRECATED** models may still be API-accessible but are phasing out. **RETIRED** models return API errors.

---

### ⚠️ LEGACY — Claude Sonnet 4 *(RETIRED April 20, 2026)*

> **Update (Apr 14, 2026):** Anthropic notified developers of the upcoming retirement of Claude Sonnet 4. Per the **official Anthropic model deprecations page** (docs.anthropic.com/en/docs/about-claude/model-deprecations, verified May 21, 2026), **Claude Sonnet 4 was retired on April 20, 2026**. All API requests to `claude-sonnet-4-20250514` now return errors. Migrate to Claude Sonnet 4.6 immediately.

> ✏️ **CORRECTION (May 18, 2026):** A previous version of this card listed the retirement date as June 15, 2026. The official Anthropic deprecation documentation confirms the actual retirement date was **April 20, 2026** — not June 15.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4-20250514` |
| **Status** | ⚠️ LEGACY — **RETIRED April 20, 2026 ❌ API CALLS WILL FAIL** |
| **Input price** | $3.00 / MTok *(last known price — shown for reference only)* |
| **Output price** | $15.00 / MTok *(last known price)* |
| **Context window** | 200,000 tokens (1M beta also retired April 30, 2026) |
| **Availability** | ❌ NONE — All requests return errors |
| **Migration** | Upgrade to **Claude Sonnet 4.6** — same price, 1M context, better performance |

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
| **Migration** | Upgrade to **Claude Opus 4.7** ($5/$25) — 67% cheaper, far better performance |

---

### ⚠️ LEGACY — Claude Opus 4 *(RETIRED April 20, 2026)*

> **Update (Apr 14, 2026):** Anthropic notified developers of the upcoming retirement of Claude Opus 4. Per the **official Anthropic model deprecations page** (docs.anthropic.com/en/docs/about-claude/model-deprecations, verified May 21, 2026), **Claude Opus 4 was retired on April 20, 2026**. All API requests to `claude-opus-4-20250514` now return errors. Migrate to Claude Opus 4.7 immediately.

> ✏️ **CORRECTION (May 18, 2026):** A previous version of this card listed the retirement date as June 15, 2026. The official Anthropic deprecation documentation confirms the actual retirement date was **April 20, 2026** — not June 15.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-20250514` |
| **Status** | ⚠️ LEGACY — **RETIRED April 20, 2026 ❌ API CALLS WILL FAIL** |
| **Input price** | $15.00 / MTok *(last known price — shown for reference only)* |
| **Output price** | $75.00 / MTok *(last known price)* |
| **Context window** | 200,000 tokens |
| **Availability** | ❌ NONE — All requests return errors |
| **Migration** | Upgrade to **Claude Opus 4.7** ($5/$25) — 67% cheaper, far better performance |

---

### ⚠️ LEGACY — Claude Haiku 3.5 *(RETIRED February 19, 2026)*

> **✏️ CORRECTION (May 18, 2026):** This model was previously listed as Active. Per the **official Anthropic model deprecations page** (docs.anthropic.com/en/docs/about-claude/model-deprecations, verified May 21, 2026), Claude Haiku 3.5 was **retired on the Claude API on February 19, 2026**. API calls will fail. Migrate to **Claude Haiku 4.5** ($1/$5, 200K context, extended thinking).

> **Note:** Claude Haiku 3.5 may still be accessible on AWS Bedrock and Google Vertex AI, which set their own independent retirement schedules.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-5-haiku-20241022` |
| **Status** | ⚠️ LEGACY — **RETIRED February 19, 2026 ❌ API CALLS WILL FAIL (Claude API)** |
| **Input price** | $0.80 / MTok *(last known price — shown for reference only)* |
| **Output price** | $4.00 / MTok *(last known price)* |
| **Cache write (5 min)** | $1.00 / MTok *(last known)* |
| **Cache write (1 hr)** | $1.60 / MTok *(last known)* |
| **Cache read** | $0.08 / MTok *(last known)* |
| **Batch input** | $0.40 / MTok *(last known)* |
| **Batch output** | $2.00 / MTok *(last known)* |
| **Context window** | 128,000 tokens |
| **Availability** | ❌ Claude API — RETIRED. Bedrock/Vertex AI may retain access on their own schedules. |
| **Migration** | **Migrate to Claude Haiku 4.5** ($1/$5) — 25% more expensive but dramatically more capable: 200K context, extended thinking, higher quality across all tasks |

---

### ⚠️ LEGACY — Claude Haiku 3 *(RETIRED February 19, 2026)*

> **✅ RETIRED (Feb 19, 2026):** Claude Haiku 3 has been officially retired per the official Anthropic model deprecations page. All API requests to `claude-3-haiku-20240307` now return errors. There is no automatic fallback — update your code to use Haiku 4.5 immediately. Note: Anthropic's pricing page continues to display pricing for reference purposes, but the model is not operational.

> ✏️ **CORRECTION (May 18, 2026):** A previous version of this card listed the retirement date as April 19-20, 2026. The official Anthropic deprecation documentation confirms the retirement date was **February 19, 2026**.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-haiku-20240307` |
| **Status** | ⚠️ LEGACY — **RETIRED February 19, 2026 ❌ API CALLS WILL FAIL** |
| **Input price** | $0.25 / MTok *(last known price — shown on pricing page for reference only)* |
| **Output price** | $1.25 / MTok *(last known price)* |
| **Context window** | 200,000 tokens |
| **Availability** | ❌ NONE — All requests return errors |
| **Migration** | **Migrate to Claude Haiku 4.5 ($1/$5)** |

---

### ⚠️ LEGACY — Claude Sonnet 3.7 *(RETIRED October 28, 2025)*

> **✏️ UPDATE (May 18, 2026):** Per the official Anthropic model deprecations page (docs.anthropic.com/en/docs/about-claude/model-deprecations, verified May 21, 2026), Claude Sonnet 3.7 was **retired on October 28, 2025**. A previous version of this card listed the model as deprecated but API-accessible. The model is no longer operational.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-7-sonnet-20250219` |
| **Status** | ⚠️ LEGACY — **RETIRED October 28, 2025 ❌ API CALLS WILL FAIL** |
| **Input price** | $3.00 / MTok *(last known price)* |
| **Output price** | $15.00 / MTok *(last known price)* |
| **Batch input** | $1.50 / MTok *(last known)* |
| **Batch output** | $7.50 / MTok *(last known)* |
| **Migration** | Use **Claude Sonnet 4.6** ($3/$15) |

---

### ⚠️ LEGACY — Claude 3 Series

| Model | Status | Migration |
|---|---|---|
| Claude 3 Opus | ⚠️ DEPRECATED Jan 2026 — available by request for paying customers | → Claude Opus 4.7 |
| Claude 3.5 Sonnet (v1 & v2) | ⚠️ **RETIRED January 5, 2026** | → Claude Sonnet 4.6 |
| Claude 3 Sonnet | ⚠️ RETIRED | → Claude Sonnet 4.6 |
| Claude 3 Haiku | ⚠️ **RETIRED February 19, 2026 ❌** | → Claude Haiku 4.5 |

> **Note:** Claude 3 Opus was deprecated in January 2026 but Anthropic has made it available again by request for paying customers (Anthropic has committed to preserve weights). Claude 3.5 Sonnet variants are fully retired (January 5, 2026). Claude 3 Haiku is fully retired (February 19, 2026) — API calls fail.

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
| **Opus 4.7 tokenizer** | New tokenizer may add up to 35% more tokens/request vs Opus 4.6 — downsample images and monitor per-request spend |
| **Haiku 4.5 migration** | Replaces retired Haiku 3 (Feb 19, 2026) and Haiku 3.5 (Feb 19, 2026); $1/$5 vs $0.25/$1.25 (Haiku 3) — use Batch API to offset |
| **Fast Mode** | Only available on **Opus 4.6** ($30/$150 input/output, 6× standard) — NOT available on Opus 4.7 |

---

*Sources last verified: May 21, 2026 against the official Anthropic pricing page at platform.claude.com/docs/en/about-claude/pricing, model deprecations at docs.anthropic.com/en/docs/about-claude/model-deprecations (retirement dates confirmed), and release notes at platform.claude.com/docs/en/release-notes/overview. No price changes detected since May 18, 2026.*
