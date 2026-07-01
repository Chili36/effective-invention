# 🟠 Anthropic — Claude Model Cards

> **Last updated:** 2026-07-01
> **Source:** https://www.anthropic.com/pricing · https://platform.claude.com/docs/en/about-claude/models/overview · https://platform.claude.com/docs/en/about-claude/pricing
> **Scraped / verified:** 2026-07-01 — 🆕 **Claude Sonnet 5 launched June 30, 2026** — new default Sonnet-tier model, replacing Claude Sonnet 4.6 as Anthropic's recommended mid-tier model. Introductory pricing $2/$10 per MTok through August 31, 2026, then $3/$15 standard from September 1, 2026. Also confirmed: Opus 4.7 Fast Mode is now deprecated (removal July 24, 2026); Opus 4.6 Fast Mode has already been removed (requests billed at standard rates as of June 29, 2026).

All prices are **USD per million tokens (MTok)**. Batch API gives a flat **50% discount** on all models. Prompt caching gives up to **90% off** on repeated input context.

> 🚫 **June 12, 2026 — CRITICAL: Claude Fable 5 + Mythos 5 SUSPENDED BY US GOVERNMENT.** The US government issued an export control directive requiring Anthropic to suspend **all access** to Claude Fable 5 and Claude Mythos 5. Anthropic is complying with the order and has disabled both Mythos-class models for **all customers globally** — including Project Glasswing partners. All other Claude models (Opus 4.8, Sonnet 5, Sonnet 4.6, Haiku 4.5) are **NOT affected** and remain fully accessible. See [Anthropic's official statement](https://www.anthropic.com/news/fable-mythos-access).
>
> - **Recommended fallback while Fable 5 is suspended:** Claude Opus 4.8 ($5/$25 per MTok).
> - No timeline for reinstatement has been announced as of July 1, 2026.

> 🆕 **June 30, 2026 — Claude Sonnet 5 launched.** Anthropic's most agentic Sonnet-tier model yet, replacing Claude Sonnet 4.6 as the default model for Free and Pro plans (also available on Max, Team, Enterprise, Claude Code, and the Claude Platform). Narrows the performance gap with Opus 4.8 on agentic coding, tool use, and knowledge work while remaining priced at the Sonnet tier. Ships with **introductory pricing** of $2/$10 per MTok (input/output) through August 31, 2026, moving to standard $3/$15 per MTok on September 1, 2026. Uses a newer tokenizer (like Opus 4.7+) that produces ~1.0–1.35× more tokens for the same input text depending on content type — the introductory price is calibrated to keep the transition roughly cost-neutral. Model ID: `claude-sonnet-5`. See [announcement](https://www.anthropic.com/news/claude-sonnet-5).

> 🆕 **June 23, 2026 — Claude Tag launched.** @Claude is a new Teams/workspace product integration that allows teams to mention and interact with Claude directly in platforms. This is a **product feature**, not a new API model — billed at standard API token rates using the underlying model. See [announcement](https://www.anthropic.com/news/introducing-claude-tag).

> 🚨 **June 9, 2026 — Claude Fable 5 + Mythos 5 launched** (subsequently suspended June 12). Claude Fable 5 (`claude-fable-5`) was Anthropic's most capable widely released model, at **$10/$50 per MTok**. Claude Mythos 5 (`claude-mythos-5`) joined Project Glasswing (limited access). Full launch details: `anthropic.com/news/claude-fable-5-mythos-5`.
>
> - Claude Opus 4.8 is now the recommended model for complex reasoning and agentic coding for all developers while Fable 5 is suspended.
> - Cybersecurity and biology queries to Fable 5 automatically fall back to Opus 4.8 — you are **not** charged Fable 5 prices for rerouted requests (moot while suspended).
> - Fable 5 requires **30-day data retention** for safety monitoring.

> ✅ **Claude Sonnet 4 + Opus 4 RETIRED on June 15, 2026. ❌** API calls to `claude-sonnet-4-20250514` and `claude-opus-4-20250514` now return errors (except via Amazon Bedrock and Google Cloud, where they remain available per Anthropic's model deprecation policy). Migration: Sonnet 4 → Sonnet 5 or Sonnet 4.6 (same price, 1M context); Opus 4 → Opus 4.8 ($5/$25, 67% cheaper).

---

## 🔒 Restricted / Preview Models (Limited Access)

### 🚫 Claude Mythos 5 *(SUSPENDED June 12, 2026 — US Government Export Control)*

> **Launched:** June 9, 2026
> **Status:** 🚫 **SUSPENDED** — Access suspended by US government export control directive on June 12, 2026. Project Glasswing access also halted for all partners. See [Anthropic's official statement](https://www.anthropic.com/news/fable-mythos-access).
> **Access:** Suspended — was available via [Project Glasswing](https://anthropic.com/glasswing) only.
> **Last-known Pricing:** $10 / MTok input · $50 / MTok output (same as Fable 5)
> **Context:** 1M tokens · Max output: 128K tokens
> **Capabilities:** Adaptive thinking (always on); no extended thinking. Successor to Claude Mythos Preview within Project Glasswing.
> **Note:** All access suspended June 12, 2026 per US government export control directive. No reinstatement timeline announced.

### Claude Mythos Preview *(Restricted — Project Glasswing)*

> **Status:** 🔒 RESTRICTED — Superseded by Claude Mythos 5 within Project Glasswing (June 9, 2026); all Glasswing access currently suspended per June 12 government directive. Offered as a research preview model for defensive cybersecurity workflows; invitation-only, no self-serve sign-up.

---

## 🚫 Suspended Models (US Government Export Control — June 12, 2026)

> **⚠️ The following model(s) were active at launch but have been suspended by US government export control directive on June 12, 2026. API calls are not possible. See [Anthropic's statement](https://www.anthropic.com/news/fable-mythos-access).**

### 🚫 Claude Fable 5 *(SUSPENDED June 12, 2026 — US Government Export Control)*

> **Launched June 9, 2026 — Suspended June 12, 2026:** Claude Fable 5 was Anthropic's most capable widely released model, built for ambitious, long-running, asynchronous work. It was suspended by US government export control directive on June 12, 2026 — just 3 days after launch. Model ID: `claude-fable-5`.
>
> **Use Claude Opus 4.8 ($5/$25) as fallback while Fable 5 is suspended.**

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-fable-5` |
| **AWS Bedrock ID** | `anthropic.claude-fable-5` |
| **Vertex AI ID** | `claude-fable-5` |
| **Released** | June 9, 2026 |
| **Suspended** | June 12, 2026 (US government export control directive) |
| **Status** | 🚫 **SUSPENDED** — Access halted for all customers globally per US government order. See [Anthropic's statement](https://www.anthropic.com/news/fable-mythos-access). |
| **Last-known Input price** | $10.00 / MTok |
| **Last-known Output price** | $50.00 / MTok |
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
| **Availability** | 🚫 SUSPENDED — was available on Claude API · Amazon Bedrock · Google Vertex AI · Microsoft Foundry |
| **Safety fallback** | Cybersecurity/biology queries auto-route to Opus 4.8 — billed at Opus 4.8 rates |
| **Data retention** | 30-day data retention required for safety monitoring |
| **Notable** | Most capable Anthropic model for general release at launch; suspended June 12, 2026 by US government order 3 days after launch; uses newer tokenizer (~30% more tokens for same text vs Sonnet 4.6-and-earlier tokenizer) |

> 📝 **While Fable 5 is suspended:** Use Claude Opus 4.8 ($5/$25 per MTok) for complex reasoning and agentic coding — it's half the price of Fable 5 and remains fully accessible.

---

## ✅ Active / Recommended Models

### Claude Opus 4.8 *(Current Top-Tier / Daily Driver — Recommended while Fable 5 is suspended)*

> **May 28, 2026 — Opus 4.8** is Anthropic's most capable **currently accessible** model. Following the June 12 US government suspension of Fable 5, Opus 4.8 is the recommended top-tier model for all developers until Fable 5 access is restored. Fast Mode available at 2× pricing for latency-sensitive workloads (research preview).

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-8` |
| **AWS Bedrock ID** | `anthropic.claude-opus-4-83` (Messages-API Bedrock endpoint only) |
| **Vertex AI ID** | `claude-opus-4-8` |
| **Released** | May 2026 |
| **Status** | ✅ Active — **Current Top-Tier / Daily Driver (Fable 5 suspended)** |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode (input)** | $10.00 / MTok *(2× standard — research preview, up to 2.5× faster speeds)* |
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
| **Notable** | Top-tier daily driver for complex reasoning and agentic coding; 1M context at standard pricing; Fast Mode at 2× base rate (research preview); Batch API up to 300k output tokens with beta header; Fable 5 safety fallback target for cybersecurity/biology queries |

> ⚠️ **Bedrock note:** Claude Opus 4.8 is available on Bedrock through the **Messages-API Bedrock endpoint** only.

---

### 🆕 Claude Sonnet 5 *(New Default Sonnet-Tier Model — Released June 30, 2026)*

> **June 30, 2026 — Claude Sonnet 5** is Anthropic's most agentic Sonnet-class model yet, replacing **Claude Sonnet 4.6** (released February 2026) as the default model for Claude Free and Pro plans. It narrows the capability gap with Opus 4.8 on agentic coding, tool use, computer use, and knowledge work — on one benchmark scoring 63.2% on agentic coding vs. Sonnet 4.6's 58.1% and Opus 4.8's 69.2% — while remaining priced at the Sonnet tier. Ships with cyber safeguards enabled by default (similar to Opus 4.7/4.8) though it was not deliberately trained on cybersecurity tasks and shows substantially weaker cyber capability than Opus 4.8 or Mythos 5.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-5` |
| **AWS Bedrock ID** | `anthropic.claude-sonnet-5` (Messages-API Bedrock endpoint) |
| **Vertex AI ID** | `claude-sonnet-5` |
| **Released** | June 30, 2026 |
| **Status** | ✅ Active — **New Default Sonnet-Tier Model** |
| **Introductory input price** | $2.00 / MTok *(through August 31, 2026)* |
| **Introductory output price** | $10.00 / MTok *(through August 31, 2026)* |
| **Standard input price (from Sept 1, 2026)** | $3.00 / MTok |
| **Standard output price (from Sept 1, 2026)** | $15.00 / MTok |
| **Cache write (5 min, intro)** | $2.50 / MTok |
| **Cache write (1 hr, intro)** | $4.00 / MTok |
| **Cache read (intro)** | $0.20 / MTok |
| **Cache write (5 min, standard)** | $3.75 / MTok |
| **Cache write (1 hr, standard)** | $6.00 / MTok |
| **Cache read (standard)** | $0.30 / MTok |
| **Batch input (intro)** | $1.00 / MTok |
| **Batch output (intro)** | $5.00 / MTok |
| **Batch input (standard)** | $1.50 / MTok |
| **Batch output (standard)** | $7.50 / MTok |
| **Context window** | 1,000,000 tokens (at standard pricing — no surcharge) |
| **Max output** | 128,000 tokens (sync) / 300,000 tokens (Batch API with `output-300k-2026-03-24` beta header) |
| **Knowledge cutoff (reliable)** | January 2026 |
| **Training data cutoff** | January 2026 |
| **Extended thinking** | ❌ No |
| **Adaptive thinking** | ✅ Yes (effort defaults to `high` on Claude API and Claude Code) |
| **Tokenizer** | Newer tokenizer (same generation as Opus 4.7+) — produces ~1.0–1.35× more tokens than Sonnet 4.6 for the same input, depending on content type |
| **Availability** | Claude API · Claude.ai (Free/Pro/Max/Team/Enterprise) · Claude Code · Claude Platform on AWS · Amazon Bedrock (Messages API endpoint) · Google Cloud · Microsoft Foundry |
| **Notable** | Default model for Free/Pro plans; strict improvement over Sonnet 4.6 on agentic benchmarks; lower rates of hallucination, sycophancy, and undesirable agentic behaviors vs Sonnet 4.6; part of Cyber Verification Program (native Claude Platform, Claude Platform on AWS, Microsoft Foundry — Google Vertex coming later) |

> 💰 **Introductory pricing window:** $2/$10 per MTok is available through **August 31, 2026**. Budget for the jump to $3/$15 per MTok starting **September 1, 2026**. Anthropic states the intro price is calibrated to offset the new tokenizer's higher token counts, making the transition "roughly cost-neutral."
> 🔄 **Replaces Claude Sonnet 4.6** as Anthropic's recommended default mid-tier model — see the note on Sonnet 4.6 below.

---

### Claude Sonnet 4.6 *(🔄 Replaced by Sonnet 5 as default — still active)*

> 🔄 **REPLACED (June 30, 2026):** Claude Sonnet 5 has replaced Sonnet 4.6 as Anthropic's default Sonnet-tier / recommended model. Sonnet 4.6 remains fully API-accessible at unchanged pricing and is not deprecated, but new projects should evaluate **Claude Sonnet 5** first — it is a strict improvement over Sonnet 4.6 on Anthropic's published agentic benchmarks.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4-6` |
| **Released** | February 17, 2026 |
| **Status** | ✅ Active — 🔄 Replaced by Sonnet 5 as default recommendation (June 30, 2026) |
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
| **Notable** | Still a solid balance of intelligence, cost, and speed; 1M context no premium; extended + adaptive thinking; **superseded by Sonnet 5** for new projects as of June 30, 2026 |

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
| Claude Fable 5 | ❌ No | ✅ Yes (always on) | 🚫 **SUSPENDED** June 12, 2026 — US gov't export control. Use Opus 4.8 as fallback. |
| Claude Mythos 5 | ❌ No | ✅ Yes (always on) | 🚫 **SUSPENDED** June 12, 2026 — US gov't export control. |
| Claude Opus 4.8 | ❌ No | ✅ Yes | **Current top-tier** while Fable 5 is suspended; Fast Mode at 2× pricing (research preview) |
| Claude Sonnet 5 | ❌ No | ✅ Yes | 🆕 **New default** — narrows gap with Opus 4.8 on agentic tasks; effort defaults to `high` |
| Claude Sonnet 4.6 | ✅ Yes | ✅ Yes | 🔄 Replaced by Sonnet 5 as default; still active, has extended thinking (Sonnet 5 does not) |
| Claude Haiku 4.5 | ✅ Yes | ❌ No | Fastest; extended thinking for budget reasoning |

> Source: `platform.claude.com/docs/en/about-claude/models/overview`, re-verified July 1, 2026.

---

## 🆕 Platform Feature: Fallback API (Fable 5 — currently moot while suspended)

> **June 9, 2026:** API customers using Claude Fable 5 must configure the **Fallback API** (`support.claude.com/en/articles/15363606`) so that cybersecurity/biology queries automatically route to Opus 4.8. Claude.ai and other hosted surfaces handle the fallback automatically.
>
> **Note (June 12, 2026):** Fable 5 is currently suspended. This configuration guide is for when access is restored.

---

## 🆕 Platform Feature: Claude Security (Enterprise — Public Beta)

> **May 2026:** Anthropic launched **Claude Security** in public beta for Claude Enterprise customers. Purpose-built for security operations workflows. Billed at standard API token rates using the underlying model.

---

## 🆕 Platform Feature: Claude Tag *(Teams Product — June 23, 2026)*

> **June 23, 2026:** Anthropic launched **Claude Tag** (`@Claude`) — a new way for teams to mention and interact with Claude directly within shared workspaces and collaboration surfaces. This is a **product/teams feature**, not a new API model. Billed at standard API token rates using the underlying Claude model. See [announcement](https://www.anthropic.com/news/introducing-claude-tag).

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new projects. **LEGACY** = still API-accessible but in the provider's legacy section. **DEPRECATED** = still accessible, published retirement date. **RETIRED** = API calls return errors ❌. **SUSPENDED** = access halted by external directive.

---

### ⚠️ LEGACY — Claude Opus 4.7 *(Fast Mode deprecated — removal July 24, 2026)*

> **📝 July 1, 2026 update:** Fast Mode for Claude Opus 4.7 is now officially **deprecated** and will be **removed on July 24, 2026**. Until removal, Fast Mode remains billable at $30/$150 per MTok (6×). After July 24, 2026, `speed: "fast"` requests to `claude-opus-4-7` are expected to run at standard speed/pricing (consistent with the change already made to Opus 4.6 — see below).

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-7` |
| **Status** | ⚠️ LEGACY — Still API-accessible; moved to Legacy section May 28, 2026; Fast Mode deprecated, removal July 24, 2026 |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode (input)** | $30.00 / MTok *(6× standard — ⚠️ DEPRECATED, removal July 24, 2026)* |
| **Fast Mode (output)** | $150.00 / MTok *(⚠️ DEPRECATED, removal July 24, 2026)* |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok |
| **Context window** | 1,000,000 tokens |
| **Max output** | 128,000 tokens (sync) / 300,000 tokens (Batch API with `output-300k-2026-03-24` beta header) |
| **Migration** | Upgrade to **Claude Opus 4.8** — same price ($5/$25), improved performance, much cheaper Fast Mode (2× vs 6×, research preview) |

---

### ⚠️ LEGACY — Claude Opus 4.6 *(Fast Mode REMOVED June 29, 2026)*

> **📝 July 1, 2026 update:** As of **June 29, 2026**, Fast Mode is **no longer available** on Claude Opus 4.6 — requests to `claude-opus-4-6` with `speed: "fast"` now run at standard speed and are billed at standard rates ($5/$25).

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-6` |
| **Status** | ⚠️ LEGACY — Still API-accessible; Fast Mode removed June 29, 2026 |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode** | ❌ **REMOVED June 29, 2026** — `speed: "fast"` now billed at standard rates |
| **Context window** | 1,000,000 tokens |
| **Migration** | → **Claude Opus 4.8** ($5/$25, Fast Mode still available at 2×, research preview) |

---

### ⚠️ LEGACY — Claude Sonnet 4.5 *(Moved to Legacy May 2026)*

| Field | Value |
|---|---|
| **Model ID** | `claude-sonnet-4-5` |
| **Status** | ⚠️ LEGACY — 1M context beta RETIRED April 30, 2026; max context now 200K |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Migration** | → **Claude Sonnet 5** (new default, intro $2/$10 through Aug 31) or **Claude Sonnet 4.6** (same price, 1M context, 64k output) |

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

### ⚠️ RETIRED — Claude Sonnet 4 *(Retired June 15, 2026 ❌ — except Bedrock/Google Cloud)*

| Field | Value |
|---|---|
| **Model ID** | `claude-sonnet-4-20250514` |
| **Status** | ⚠️ RETIRED — **API calls return errors ❌ on Claude API — Retired June 15, 2026** (still available on Amazon Bedrock and Google Cloud) |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Migration** | → **Claude Sonnet 5** or **Claude Sonnet 4.6** — same price, 1M context |

---

### ⚠️ RETIRED — Claude Opus 4 *(Retired June 15, 2026 ❌ — except Google Cloud)*

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-20250514` |
| **Status** | ⚠️ RETIRED — **API calls return errors ❌ on Claude API — Retired June 15, 2026** (still available on Google Cloud) |
| **Input price** | $15.00 / MTok |
| **Output price** | $75.00 / MTok |
| **Migration** | → **Claude Opus 4.8** ($5/$25) — 67% cheaper |

---

### ⚠️ LEGACY — Claude Haiku 3.5 *(RETIRED February 19, 2026 on Claude API — except Bedrock/Google Cloud)*

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
| **Migration** | → **Claude Sonnet 5** or **Claude Sonnet 4.6** ($3/$15) |

---

### ⚠️ LEGACY — Claude 3 Series

| Model | Status | Migration |
|---|---|---|
| Claude 3 Opus | ⚠️ DEPRECATED Jan 2026 — available by request for paying customers | → Claude Opus 4.8 |
| Claude 3.5 Sonnet (v1 & v2) | ⚠️ **RETIRED January 5, 2026** | → Claude Sonnet 5 or Sonnet 4.6 |
| Claude 3 Sonnet | ⚠️ RETIRED | → Claude Sonnet 5 or Sonnet 4.6 |
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
| **🆕 Sonnet 5 introductory pricing** | $2/$10 per MTok through Aug 31, 2026 — cheaper than GPT-5.5 and Gemini 3.1 Pro; lock in savings before the Sept 1 jump to $3/$15 |
| **🚫 Fable 5 SUSPENDED** | Fable 5 ($10/$50) access is suspended by US gov't order. Route to Opus 4.8 ($5/$25) instead — half the per-token cost. |
| **Opus 4.8 vs Opus 4.7 Fast Mode** | Opus 4.8 Fast Mode is $10/$50 (2× standard, research preview); Opus 4.7 Fast Mode was $30/$150 (6×) and is now deprecated (removal July 24, 2026) |
| **⚠️ Opus 4.6 Fast Mode removed** | As of June 29, 2026, Opus 4.6 no longer supports Fast Mode — all requests billed at standard $5/$25 |
| **US-only inference (data residency)** | 1.1× pricing on Opus 4.6+, Sonnet 4.6+, Sonnet 5, and Fable 5 (when restored) |
| **Thinking modes** | Adaptive: Opus 4.8 + Sonnet 5 + Sonnet 4.6 (Fable 5 suspended). Extended: Sonnet 4.6 + Haiku 4.5 (**not** available on Sonnet 5). |
| **⚠️ Sonnet 4 + Opus 4 RETIRED** | **Retired June 15, 2026 ❌** on Claude API — API calls return errors — Sonnet 4 → Sonnet 5/4.6, Opus 4 → Opus 4.8 |

---

*Sources last verified: July 1, 2026 against `platform.claude.com/docs/en/about-claude/pricing` and `platform.claude.com/docs/en/about-claude/models/overview` · 🆕 Claude Sonnet 5 confirmed ($2/$10 intro through Aug 31, 2026 → $3/$15 standard from Sept 1, 2026) — replaces Sonnet 4.6 as default · Opus 4.7 Fast Mode deprecation (removal July 24, 2026) and Opus 4.6 Fast Mode removal (June 29, 2026) confirmed · Opus 4.8 $5/$25, Sonnet 4.6 $3/$15, Haiku 4.5 $1/$5 re-confirmed unchanged · Fable 5 + Mythos 5 suspension status re-confirmed.*
