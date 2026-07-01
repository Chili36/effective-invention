# 🟠 Anthropic — Claude Model Cards

> **Last updated:** 2026-07-01
> **Source:** https://www.anthropic.com/pricing · https://platform.claude.com/docs/en/about-claude/models/overview · https://platform.claude.com/docs/en/about-claude/pricing
> **Scraped / verified:** 2026-07-01 — 🔓 **BREAKING: Claude Fable 5 + Mythos 5 RESTORED.** The US export control directive that suspended both models on June 12, 2026 was **lifted June 30, 2026**. Fable 5 returns globally today, July 1, 2026, on the Claude Platform, Claude.ai, Claude Code, and Claude Cowork (AWS/Google Cloud/Microsoft Foundry access being re-enabled "as quickly as possible"). Mythos 5 access has been restored for an approved set of US organizations via Project Glasswing following June 26, 2026 government approval. See [Anthropic's "Redeploying Fable 5" post](https://www.anthropic.com/news/redeploying-fable-5).

All prices are **USD per million tokens (MTok)**. Batch API gives a flat **50% discount** on all models. Prompt caching gives up to **90% off** on repeated input context.

> 🔓 **July 1, 2026 — Fable 5 and Mythos 5 RESTORED after US government lifts export controls.** On June 12, 2026, the US government issued an export control directive suspending all access to Fable 5 and Mythos 5 (citing a reported non-universal jailbreak). On **June 30, 2026**, the Trump administration lifted those export controls after Anthropic worked with the government (including CAISI/NIST) to deploy an improved safety classifier that blocks the reported bypass technique in **over 99%** of cases. **Fable 5 becomes available globally starting July 1, 2026** across the Claude Platform, Claude.ai, Claude Code, and Claude Cowork; AWS Bedrock, Google Cloud, and Microsoft Foundry access is being re-enabled as quickly as possible. **Mythos 5** was restored earlier, on June 26, 2026, for an approved set of US organizations under Project Glasswing, with broader international/domestic expansion ongoing. See [Anthropic's full statement](https://www.anthropic.com/news/redeploying-fable-5).
>
> - **Subscription access:** For Pro, Max, Team, and select Enterprise plans, Fable 5 is included for **up to 50% of weekly usage limits through July 7, 2026**, after which it moves to a **usage-credits** model (no longer bundled free).
> - Anthropic, together with Amazon, Microsoft, Google, and other Project Glasswing partners, is developing a **shared industry framework for scoring AI jailbreak severity**, and is deepening pre-release testing collaboration with the US government under the June 2, 2026 executive order on frontier AI security.

> 🆕 **June 30, 2026 — Claude Sonnet 5 launched.** Anthropic's most agentic Sonnet-tier model yet, replacing Claude Sonnet 4.6 as the default model for Free and Pro plans (also available on Max, Team, Enterprise, Claude Code, and the Claude Platform). Narrows the performance gap with Opus 4.8 on agentic coding, tool use, and knowledge work while remaining priced at the Sonnet tier. Ships with **introductory pricing** of $2/$10 per MTok (input/output) through August 31, 2026, moving to standard $3/$15 per MTok on September 1, 2026. Model ID: `claude-sonnet-5`. See [announcement](https://www.anthropic.com/news/claude-sonnet-5).

> 🆕 **June 23, 2026 — Claude Tag launched.** @Claude is a new Teams/workspace product integration that allows teams to mention and interact with Claude directly in platforms. This is a **product feature**, not a new API model — billed at standard API token rates using the underlying model. See [announcement](https://www.anthropic.com/news/introducing-claude-tag).

> ✅ **Claude Sonnet 4 + Opus 4 RETIRED on June 15, 2026. ❌** API calls to `claude-sonnet-4-20250514` and `claude-opus-4-20250514` now return errors (except via Amazon Bedrock and Google Cloud, where they remain available per Anthropic's model deprecation policy). Migration: Sonnet 4 → Sonnet 5 or Sonnet 4.6 (same price, 1M context); Opus 4 → Opus 4.8 ($5/$25, 67% cheaper).

---

## ✅ Active / Recommended Models

### 🔓 Claude Fable 5 *(RESTORED July 1, 2026 — Most Capable Widely-Released Model)*

> **Released June 9, 2026 → Suspended June 12, 2026 → Restored July 1, 2026.** Claude Fable 5 is Anthropic's most capable widely released model, built for ambitious, long-running, asynchronous work. It was suspended for 18 days under a US government export control directive and has now been fully redeployed with an improved safety classifier. Model ID: `claude-fable-5`.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-fable-5` |
| **AWS Bedrock ID** | `anthropic.claude-fable-5` |
| **Vertex AI ID** | `claude-fable-5` |
| **Released** | June 9, 2026 · Suspended June 12–30, 2026 · **Restored July 1, 2026** |
| **Status** | ✅ Active — Restored globally July 1, 2026 |
| **Input price** | $10.00 / MTok |
| **Output price** | $50.00 / MTok |
| **Cache write (5 min)** | $12.50 / MTok |
| **Cache write (1 hr)** | $20.00 / MTok |
| **Cache read** | $1.00 / MTok |
| **Batch input** | $5.00 / MTok *(50% off)* |
| **Batch output** | $25.00 / MTok *(50% off)* |
| **US-only inference** | 1.1× pricing |
| **Context window** | 1,000,000 tokens (standard pricing — no long-context surcharge) |
| **Max output** | 128,000 tokens |
| **Thinking mode** | Adaptive only (always on); no extended thinking |
| **Tokenizer** | Newer tokenizer (shared with Opus 4.7+, Sonnet 5) — produces ~30% more tokens for the same text vs. the Sonnet 4.6-and-earlier tokenizer |
| **Availability** | Claude API · Claude.ai · Claude Code · Claude Cowork · Claude Platform on AWS · Amazon Bedrock · Google Vertex AI · Microsoft Foundry *(cloud partner access being re-enabled)* |
| **Safety** | Includes safety classifiers that can decline cybersecurity/biology/chemistry/distillation requests; flagged queries auto-route to Opus 4.8 and are billed at Opus 4.8 rates, not Fable 5 rates |
| **Data retention** | 30-day data retention required for safety monitoring (no zero-data-retention option) |
| **Subscription access** | Pro/Max/Team/select Enterprise: included for up to 50% of weekly usage limits through **July 7, 2026**, then usage-credits billing |
| **Notable** | 2× Opus 4.8 pricing; state-of-the-art on Anthropic's coding, knowledge-work, and vision evals; restored after a new safety classifier was deployed that blocks the reported jailbreak technique in >99% of cases |

---

### 🔒 Claude Mythos 5 *(Restricted — Project Glasswing, access restored to approved orgs)*

> **Released June 9, 2026 → Suspended June 12, 2026 → Restored June 26, 2026** for an approved set of US organizations, ahead of Fable 5's broader July 1 restoration. Same underlying model as Fable 5 but with cybersecurity safeguards lifted for vetted cyber-defense partners.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-mythos-5` |
| **Status** | 🔒 Restricted — restored June 26, 2026 for approved Project Glasswing organizations; international/broader domestic expansion ongoing |
| **Pricing** | $10.00 / MTok input · $50.00 / MTok output (identical to Fable 5) |
| **Context window** | 1,000,000 tokens · Max output: 128,000 tokens |
| **Capabilities** | Adaptive thinking (always on); no safety classifiers on cybersecurity/biology queries |
| **Access** | [Project Glasswing](https://anthropic.com/glasswing) — contact Anthropic, AWS, or Google Cloud account team |
| **Data retention** | 30-day mandatory retention (Covered Model) |

---

### Claude Opus 4.8 *(Top-Tier / Daily Driver)*

> **May 28, 2026 — Opus 4.8** is Anthropic's most capable general-availability model below the Mythos-class tier. Fast Mode available at 2× pricing for latency-sensitive workloads (research preview).

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-8` |
| **AWS Bedrock ID** | `anthropic.claude-opus-4-83` (Messages-API Bedrock endpoint only) |
| **Vertex AI ID** | `claude-opus-4-8` |
| **Released** | May 2026 |
| **Status** | ✅ Active — Top-tier daily driver; safety fallback target for Fable 5 |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode (input)** | $10.00 / MTok *(2× standard — research preview, up to 2.5× faster)* |
| **Fast Mode (output)** | $50.00 / MTok |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Context window** | 1,000,000 tokens (standard API) · 200,000 tokens (Microsoft Foundry only) |
| **Max output** | 128,000 tokens (sync) / 300,000 tokens (Batch API with beta header) |
| **Extended thinking** | ❌ No |
| **Adaptive thinking** | ✅ Yes |
| **Availability** | Claude API · Claude Platform on AWS · Amazon Bedrock (Messages API) · Google Vertex AI · Microsoft Foundry (200k ctx) |
| **Notable** | 1M context at standard pricing; Fast Mode at 2× base rate; Fable 5 safety-fallback target for cybersecurity/biology queries |

---

### Claude Sonnet 5 *(New Default Sonnet-Tier Model — Released June 30, 2026)*

> **June 30, 2026 — Claude Sonnet 5** is Anthropic's most agentic Sonnet-class model yet, replacing **Claude Sonnet 4.6** as the default model for Claude Free and Pro plans. It narrows the capability gap with Opus 4.8 on agentic coding, tool use, computer use, and knowledge work, while remaining priced at the Sonnet tier. Ships with cyber safeguards enabled by default (same as Opus 4.7/4.8), though it was not deliberately trained on cybersecurity tasks and shows substantially weaker cyber capability than Opus 4.8 or Mythos 5 (0.0% working-exploit rate on a Mozilla Firefox evaluation, vs. 68.8% for Opus 4.8 and 88.4% for Mythos 5).

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-5` |
| **AWS Bedrock ID** | `anthropic.claude-sonnet-5` |
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
| **Max output** | 128,000 tokens (sync) / 300,000 tokens (Batch API with beta header) |
| **Extended thinking** | ❌ No |
| **Adaptive thinking** | ✅ Yes (effort defaults to `high` on Claude API and Claude Code) |
| **Tokenizer** | Newer tokenizer (same generation as Opus 4.7+/Fable 5) — produces ~30% more tokens than Sonnet 4.6 for the same text |
| **Availability** | Claude API · Claude.ai (Free/Pro/Max/Team/Enterprise) · Claude Code · Claude Platform on AWS · Amazon Bedrock · Google Cloud · Microsoft Foundry |
| **Notable** | Default model for Free/Pro plans; strict improvement over Sonnet 4.6 on agentic benchmarks (SWE-Bench Pro +5.1%, Terminal-Bench 2.1 +13.4%); lower hallucination and sycophancy rates than Sonnet 4.6 |

> 💰 **Introductory pricing window:** $2/$10 per MTok through **August 31, 2026**, then $3/$15 standard from **September 1, 2026**.
> 🔄 **Replaces Claude Sonnet 4.6** as Anthropic's recommended default mid-tier model.

---

### Claude Sonnet 4.6 *(🔄 Replaced by Sonnet 5 as default — still active)*

> 🔄 **REPLACED (June 30, 2026):** Claude Sonnet 5 has replaced Sonnet 4.6 as Anthropic's default Sonnet-tier / recommended model. Sonnet 4.6 remains fully API-accessible at unchanged pricing and is not deprecated.

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
| **Max output** | 64,000 tokens (sync) / 300,000 tokens (Batch API with beta header) |
| **Extended thinking** | ✅ Yes |
| **Adaptive thinking** | ✅ Yes |
| **Availability** | API · AWS Bedrock · Google Vertex AI · Microsoft Foundry |
| **Notable** | Still a solid balance of intelligence, cost, and speed; 1M context no premium; extended + adaptive thinking; **superseded by Sonnet 5** for new projects |

---

### Claude Haiku 4.5

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-haiku-4-5` |
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
| **Extended thinking** | ✅ Yes |
| **Adaptive thinking** | ❌ No |
| **Availability** | API · AWS Bedrock (all regions) · Google Vertex AI · Microsoft Foundry |
| **Notable** | Fastest model; cheapest in the Claude lineup |

---

## 📊 Thinking Capabilities Matrix (Active Models)

| Model | Extended Thinking | Adaptive Thinking | Notes |
|---|---|---|---|
| Claude Fable 5 | ❌ No | ✅ Yes (always on) | 🔓 **Restored July 1, 2026**. Cyber/bio queries auto-route to Opus 4.8. |
| Claude Mythos 5 | ❌ No | ✅ Yes (always on) | 🔒 Restricted to Project Glasswing (restored June 26, 2026). |
| Claude Opus 4.8 | ❌ No | ✅ Yes | Top-tier daily driver; Fast Mode at 2× pricing |
| Claude Sonnet 5 | ❌ No | ✅ Yes | New default — narrows gap with Opus 4.8; effort defaults to `high` |
| Claude Sonnet 4.6 | ✅ Yes | ✅ Yes | Replaced by Sonnet 5 as default; still active |
| Claude Haiku 4.5 | ✅ Yes | ❌ No | Fastest; extended thinking for budget reasoning |

> Source: `platform.claude.com/docs/en/about-claude/models/overview` and `platform.claude.com/docs/en/about-claude/pricing`, re-verified July 1, 2026.

---

## 🆕 Platform Feature: Claude Tag *(Teams Product — June 23, 2026)*

> **June 23, 2026:** Anthropic launched **Claude Tag** (`@Claude`) — a new way for teams to mention and interact with Claude directly within shared workspaces. This is a **product/teams feature**, not a new API model. Billed at standard API token rates using the underlying Claude model.

## 🆕 Platform Feature: Claude Security (Enterprise — Public Beta)

> **May 2026:** Anthropic launched **Claude Security** in public beta for Claude Enterprise customers, purpose-built for security operations workflows. Billed at standard API token rates using the underlying model.

## 🤝 Deeper US Government Collaboration (announced June 30, 2026)

> As part of the resolution that restored Fable 5 and Mythos 5, Anthropic committed to: (1) expanded pre-release government access and evaluation for models that materially advance the capability frontier; (2) rapid information sharing on safeguards and jailbreaks; (3) dedicated resources for joint AI-security research with the government; and (4) work toward a common, voluntary industry security/evaluation standard. Anthropic is also partnering with Amazon, Microsoft, Google, and other Glasswing partners on a **shared jailbreak-severity scoring framework** (capability gain, breadth, ease of weaponization, discoverability).

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new projects. **LEGACY** = still API-accessible but in the provider's legacy section. **DEPRECATED** = still accessible, published retirement date. **RETIRED** = API calls return errors ❌.

---

### ⚠️ LEGACY — Claude Mythos Preview *(Superseded by Mythos 5)*

| Field | Value |
|---|---|
| **Status** | ⚠️ LEGACY — Superseded by Claude Mythos 5 (June 9, 2026) within Project Glasswing |
| **Last-known Pricing** | $25.00 / MTok input · $125.00 / MTok output |
| **Migration** | → **Claude Mythos 5** ($10/$50 — same capability tier, lower price) |

---

### ⚠️ LEGACY — Claude Opus 4.7 *(Fast Mode deprecated — removal July 24, 2026)*

> Fast Mode for Claude Opus 4.7 is officially **deprecated** and will be **removed on July 24, 2026**. Until removal, Fast Mode remains billable at $30/$150 per MTok (6×).

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-7` |
| **Status** | ⚠️ LEGACY — Fast Mode deprecated, removal July 24, 2026 |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode (input/output)** | $30.00 / $150.00 per MTok *(⚠️ DEPRECATED, removal July 24, 2026)* |
| **Context window** | 1,000,000 tokens |
| **Migration** | → **Claude Opus 4.8** (same price, cheaper Fast Mode at 2× vs 6×) |

---

### ⚠️ LEGACY — Claude Opus 4.6 *(Fast Mode REMOVED June 29, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-6` |
| **Status** | ⚠️ LEGACY — Fast Mode removed June 29, 2026 |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode** | ❌ REMOVED June 29, 2026 — billed at standard rates |
| **Context window** | 1,000,000 tokens |
| **Migration** | → **Claude Opus 4.8** |

---

### ⚠️ LEGACY — Claude Sonnet 4.5

| Field | Value |
|---|---|
| **Model ID** | `claude-sonnet-4-5` |
| **Status** | ⚠️ LEGACY — 1M context beta RETIRED April 30, 2026; max context now 200K |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Migration** | → **Claude Sonnet 5** (intro $2/$10 through Aug 31) or **Claude Sonnet 4.6** |

---

### ⚠️ LEGACY — Claude Opus 4.5

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-5` |
| **Status** | ⚠️ LEGACY |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Context window** | 200,000 tokens |
| **Migration** | → **Claude Opus 4.8** (1M context, 128k output) |

---

### ⚠️ LEGACY — Claude Opus 4.1

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-1` |
| **Status** | ⚠️ LEGACY (deprecated) |
| **Input price** | $15.00 / MTok |
| **Output price** | $75.00 / MTok |
| **Migration** | → **Claude Opus 4.8** ($5/$25) — 67% cheaper |

---

### ⚠️ RETIRED — Claude Sonnet 4 *(Retired June 15, 2026 ❌ — except Bedrock/Google Cloud)*

| Field | Value |
|---|---|
| **Model ID** | `claude-sonnet-4-20250514` |
| **Status** | ⚠️ RETIRED — API calls return errors ❌ on Claude API |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Migration** | → **Claude Sonnet 5** or **Claude Sonnet 4.6** |

---

### ⚠️ RETIRED — Claude Opus 4 *(Retired June 15, 2026 ❌ — except Google Cloud)*

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-20250514` |
| **Status** | ⚠️ RETIRED — API calls return errors ❌ on Claude API |
| **Input price** | $15.00 / MTok |
| **Output price** | $75.00 / MTok |
| **Migration** | → **Claude Opus 4.8** ($5/$25) — 67% cheaper |

---

### ⚠️ LEGACY — Claude Haiku 3.5 *(RETIRED February 19, 2026 on Claude API)*

| Field | Value |
|---|---|
| **Model ID** | `claude-3-5-haiku-20241022` |
| **Status** | ⚠️ LEGACY — RETIRED Feb 19, 2026 ❌ (Claude API); still on Bedrock/Vertex AI |
| **Input price** | $0.80 / MTok |
| **Output price** | $4.00 / MTok |
| **Migration** | → **Claude Haiku 4.5** ($1/$5) |

---

### ⚠️ LEGACY — Claude Haiku 3 *(RETIRED February 19, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `claude-3-haiku-20240307` |
| **Status** | ⚠️ LEGACY — RETIRED Feb 19, 2026 ❌ |
| **Migration** | → **Claude Haiku 4.5** ($1/$5) |

---

### ⚠️ LEGACY — Claude Sonnet 3.7 *(RETIRED October 28, 2025)*

| Field | Value |
|---|---|
| **Model ID** | `claude-3-7-sonnet-20250219` |
| **Status** | ⚠️ LEGACY — RETIRED Oct 28, 2025 ❌ |
| **Migration** | → **Claude Sonnet 5** or **Claude Sonnet 4.6** |

---

### ⚠️ LEGACY — Claude 3 Series

| Model | Status | Migration |
|---|---|---|
| Claude 3 Opus | ⚠️ DEPRECATED Jan 2026 — available by request | → Claude Opus 4.8 |
| Claude 3.5 Sonnet (v1 & v2) | ⚠️ RETIRED January 5, 2026 | → Claude Sonnet 5 or Sonnet 4.6 |
| Claude 3 Sonnet | ⚠️ RETIRED | → Claude Sonnet 5 or Sonnet 4.6 |
| Claude 3 Haiku | ⚠️ RETIRED February 19, 2026 ❌ | → Claude Haiku 4.5 |

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
| **🔓 Fable 5 restored** | $10/$50 — 2× Opus 4.8. Safety-flagged queries auto-route to Opus 4.8 and bill at Opus 4.8 rates |
| **🆕 Sonnet 5 introductory pricing** | $2/$10 per MTok through Aug 31, 2026 — lock in savings before the Sept 1 jump to $3/$15 |
| **Opus 4.8 vs Opus 4.7 Fast Mode** | Opus 4.8 Fast Mode is $10/$50 (2× standard); Opus 4.7 Fast Mode was $30/$150 (6×) and is deprecated (removal July 24, 2026) |
| **⚠️ Opus 4.6 Fast Mode removed** | As of June 29, 2026, billed at standard $5/$25 |
| **US-only inference (data residency)** | 1.1× pricing on Opus 4.6+, Sonnet 4.6+, Sonnet 5, and Fable 5/Mythos 5 |
| **Thinking modes** | Adaptive: Fable 5, Mythos 5, Opus 4.8, Sonnet 5, Sonnet 4.6. Extended: Sonnet 4.6, Haiku 4.5 (**not** on Sonnet 5/Fable 5/Mythos 5) |
| **Tokenizer note** | Fable 5, Mythos 5, Opus 4.7+, and Sonnet 5 use a newer tokenizer producing ~30% more tokens for the same text vs. Sonnet 4.6-and-earlier |
| **⚠️ Sonnet 4 + Opus 4 RETIRED** | Retired June 15, 2026 ❌ on Claude API — Sonnet 4 → Sonnet 5/4.6, Opus 4 → Opus 4.8 |

---

*Sources last verified: July 1, 2026 against `platform.claude.com/docs/en/about-claude/pricing`, `platform.claude.com/docs/en/about-claude/models/overview`, `anthropic.com/news/redeploying-fable-5`, and `anthropic.com/news/fable-mythos-access`. 🔓 **Major update:** Fable 5 and Mythos 5 export controls lifted June 30, 2026; Fable 5 restored globally July 1, 2026 with a new >99%-effective safety classifier; Mythos 5 restored for approved orgs June 26, 2026. Opus 4.8 $5/$25, Sonnet 5 $2/$10→$3/$15, Sonnet 4.6 $3/$15, Haiku 4.5 $1/$5 all re-confirmed unchanged against the official pricing table.*
