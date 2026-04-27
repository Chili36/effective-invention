# 🟠 Anthropic — Claude Model Cards

> **Last updated:** 2026-04-27  
> **Source:** https://platform.claude.com/docs/en/about-claude/pricing (official — verified Apr 27, 2026) · https://platform.claude.com/docs/en/release-notes/overview · https://releasebot.io/updates/anthropic · https://findskill.ai/blog/claude-opus-4-7-release-tracker/ · https://dev.to/flarecanary/claude-3-haiku-20240307-just-started-returning-errors-57he  
> **Scraped / verified:** 2026-04-27  

All prices are **USD per million tokens (MTok)**. Batch API gives a flat **50% discount** on all models. Prompt caching gives up to **90% off** on repeated input context.

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

> **Updated Apr 27, 2026:** Claude Opus 4.7 remains Anthropic's most capable generally available model. Now broadly available in Bedrock console self-serve across 27 AWS regions.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-7` |
| **Released** | April 16, 2026 |
| **Status** | ✅ Active — **Current Flagship** |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode (input)** | $30.00 / MTok *(beta — same as Opus 4.6)* |
| **Fast Mode (output)** | $150.00 / MTok *(beta)* |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Context window** | 1,000,000 tokens (at standard pricing — no surcharge) |
| **Max output** | 32,000 tokens (sync) / 300,000 tokens (Batch API with beta header) |
| **Availability** | API, Claude Platform, AWS Bedrock (all regions, self-serve), Google Vertex AI, Microsoft Foundry, GitHub Copilot Pro+ |
| **Rate limits** | Tiered by usage tier; contact Anthropic for enterprise limits |
| **Notable** | **xhigh effort level** (new, above high — best for coding/agentic tasks); **task budgets beta** (caps token spending in agentic loops); **/ultrareview** (multi-agent code review in Claude Code); **3.75MP vision** (2,576px long edge — up from 1,568px/1.15MP); **new tokenizer** (up to 35% more tokens/request vs Opus 4.6 — same price/token but monitor per-request costs); automated cybersecurity safeguard detection/blocking; SWE-bench Verified 87.6%; GPQA Diamond 94.2%; CursorBench 70%; US-only data residency: 1.1× multiplier |

> ⚠️ **Tokenizer change:** Opus 4.7 uses a new tokenizer that may produce up to 35% more tokens for the same text compared to Opus 4.6. The per-token price is unchanged at $5/$25, but your effective cost per request may increase depending on content type. Monitor actual usage after migration.

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
| **Notable** | Full 1M context at standard rate; Fast Mode 6× pricing for low-latency; extended thinking billed as output tokens; US-only data residency: 1.1× multiplier |

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
| **Notable** | Improved agentic search; 1M context no premium; extended thinking supported; 1,633 GDPval-AA Elo benchmark leader for agentic workflows |

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
| **Availability** | API, AWS Bedrock (all regions, self-serve as of Apr 2026), Google Vertex AI, Microsoft Foundry |
| **Notable** | Fastest model; extended thinking supported; recommended migration target from retired Claude Haiku 3 (retired April 19-20, 2026) and Haiku 3.5 |

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

> ⏰ **URGENT (Apr 27, 2026):** The 1M-token context window beta for **Claude Sonnet 4.5 retires in 3 days — April 30, 2026.** Requests using the `context-1m-2025-08-07` beta header will return errors after that date. Migrate to **Claude Sonnet 4.6** which supports 1M context at standard pricing with no beta header.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4-5` |
| **Released** | 2025 |
| **Status** | ✅ Active |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Long context input (>200K)** | $6.00 / MTok *(beta — RETIRING APRIL 30, 2026 🚨)* |
| **Long context output (>200K)** | $22.50 / MTok *(beta — RETIRING APRIL 30, 2026 🚨)* |
| **Cache write (5 min)** | $3.75 / MTok |
| **Cache read** | $0.30 / MTok |
| **Batch input** | $1.50 / MTok |
| **Batch output** | $7.50 / MTok |
| **Context window** | 200,000 tokens standard; 1M via beta (RETIRING April 30, 2026) |
| **Availability** | API, AWS Bedrock, Google Vertex AI, Microsoft Foundry |
| **Notable** | Migrate to Sonnet 4.6 for 1M context at standard pricing — beta retiring April 30, 2026 |

---

### Claude Haiku 3.5 *(Previous Generation — Still Available)*

> **✏️ CORRECTION (Apr 13, 2026):** This model was incorrectly marked RETIRED in a prior update. The official Anthropic pricing page confirms Haiku 3.5 is still active and accessible. Haiku 4.5 is recommended for new projects.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-5-haiku-20241022` |
| **Status** | ✅ Active — Previous generation (migration advisory) |
| **Input price** | $0.80 / MTok |
| **Output price** | $4.00 / MTok |
| **Cache write (5 min)** | $1.00 / MTok |
| **Cache write (1 hr)** | $1.60 / MTok |
| **Cache read** | $0.08 / MTok |
| **Batch input** | $0.40 / MTok |
| **Batch output** | $2.00 / MTok |
| **Context window** | 128,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI |
| **Notable** | Still listed on official pricing page; for new projects use **Haiku 4.5** ($1/$5, 200K context, extended thinking) |

---

## 🆕 Platform Feature: Managed Agents Memory (Public Beta)

> **Apr 25, 2026:** Memory for Claude Managed Agents is now in **public beta** under the standard `managed-agents-2026-04-01` header. This allows agents to persist memory across sessions. No pricing change — billed at standard token rates for the underlying model.

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new projects. **DEPRECATED** models are still API-accessible but phasing out. **RETIRED** models return API errors.

---

### ⚠️ LEGACY — Claude Sonnet 4 *(DEPRECATED — Retiring June 15, 2026)*

> **Update (Apr 15, 2026):** Anthropic has officially announced deprecation of Claude Sonnet 4, with retirement on the Claude API scheduled for **June 15, 2026**. Migrate to Claude Sonnet 4.6 immediately.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4-20250514` |
| **Status** | ⚠️ LEGACY — **DEPRECATED · Retiring June 15, 2026** |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Batch input** | $1.50 / MTok |
| **Batch output** | $7.50 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI (until June 15, 2026) |
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

### ⚠️ LEGACY — Claude Opus 4 *(DEPRECATED — Retiring June 15, 2026)*

> **Update (Apr 15, 2026):** Anthropic has officially announced deprecation of Claude Opus 4, with retirement on the Claude API scheduled for **June 15, 2026**.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-20250514` |
| **Status** | ⚠️ LEGACY — **DEPRECATED · Retiring June 15, 2026** |
| **Input price** | $15.00 / MTok |
| **Output price** | $75.00 / MTok |
| **Batch input** | $7.50 / MTok |
| **Batch output** | $37.50 / MTok |
| **Context window** | 200,000 tokens |
| **Availability** | API, AWS Bedrock, Google Vertex AI (until June 15, 2026) |
| **Migration** | Upgrade to **Claude Opus 4.7** ($5/$25) — 67% cheaper, far better performance |

---

### ⚠️ LEGACY — Claude Haiku 3 *(RETIRED — April 19-20, 2026)*

> **✅ RETIRED (Apr 19-20, 2026):** Claude Haiku 3 has been officially retired. All API requests to `claude-3-haiku-20240307` now return errors. There is no automatic fallback — update your code to use Haiku 4.5 immediately.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-haiku-20240307` |
| **Status** | ⚠️ LEGACY — **RETIRED April 19-20, 2026 ❌ API CALLS WILL FAIL** |
| **Input price** | $0.25 / MTok *(last known price)* |
| **Output price** | $1.25 / MTok *(last known price)* |
| **Context window** | 200,000 tokens |
| **Availability** | ❌ NONE — All requests return errors |
| **Migration** | **Migrate to Claude Haiku 4.5 ($1/$5)** — Note: Haiku 4.5 has breaking API changes (temperature + top_p cannot both be set; new stop reasons) |

---

### ⚠️ LEGACY — Claude Sonnet 3.7 *(DEPRECATED)*

> **✏️ CORRECTION (Apr 13, 2026):** Previously marked as RETIRED (API errors). The official Anthropic pricing page lists Sonnet 3.7 as *deprecated* — still accessible but not recommended for new projects.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-3-7-sonnet-20250219` |
| **Status** | ⚠️ LEGACY — **DEPRECATED** (API still accessible; being phased out) |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Batch input** | $1.50 / MTok |
| **Batch output** | $7.50 / MTok |
| **Migration** | Use **Claude Sonnet 4.6** ($3/$15) |

---

### ⚠️ LEGACY — Claude 3 Series

| Model | Status | Migration |
|---|---|---|
| Claude 3 Opus | ⚠️ DEPRECATED (API accessible, phasing out) | → Claude Opus 4.7 |
| Claude 3.5 Sonnet (v1 & v2) | ⚠️ RETIRED | → Claude Sonnet 4.6 |
| Claude 3 Sonnet | ⚠️ RETIRED | → Claude Sonnet 4.6 |
| Claude 3 Haiku | ⚠️ **RETIRED April 19-20, 2026 ❌** | → Claude Haiku 4.5 |

> **Note:** Claude 3 Opus is listed as *deprecated* on the official pricing page at $15/$75; API may still be accessible. Claude 3.5 Sonnet variants and Claude 3 Sonnet are fully retired. Claude 3 Haiku is now fully retired — API calls fail.

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
| **Haiku 4.5 migration** | 4× price increase vs Haiku 3 ($1/$5 vs $0.25/$1.25) — use Batch API to offset |

---

*Sources last verified: April 27, 2026 against the official Anthropic pricing page at platform.claude.com/docs/en/about-claude/pricing, release notes at platform.claude.com/docs/en/release-notes/overview, releasebot.io/updates/anthropic, and dev.to/flarecanary (Haiku 3 retirement confirmation)*
