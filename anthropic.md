# 🟠 Anthropic — Claude Model Cards

> **Last updated:** 2026-07-27
> **Source:** https://www.anthropic.com/pricing · https://platform.claude.com/docs/en/about-claude/models/overview · https://platform.claude.com/docs/en/about-claude/pricing · https://www.anthropic.com/news/claude-opus-5
> **Scraped / verified:** 2026-07-27 — ✅ **Re-verified against the live `platform.claude.com/docs/en/about-claude/pricing` page and independent reporting on the July 24, 2026 Opus 5 launch.** 🆕 **Claude Opus 5 launched July 24, 2026** at the same $5.00/$25.00 per MTok rate as the Opus 4.8 model it replaces, becoming the new default on Claude Max and the strongest model on Claude Pro. ✅ **Fable 5's subscription-tier cliff was permanently resolved on July 20, 2026:** Max and Team Premium plans keep Fable 5 included at 50% of weekly usage limits going forward; Pro and Team Standard plans moved to metered usage credits ($10/$50 per MTok, same as the API rate) with a one-time $100 credit. All other active price points (Fable 5, Mythos 5, Sonnet 5, Sonnet 4.6, Haiku 4.5) re-confirmed unchanged.

All prices are **USD per million tokens (MTok)**. Batch API gives a flat **50% discount** on all models. Prompt caching gives up to **90% off** on repeated input context.

> 🆕 **July 24, 2026 — Claude Opus 5 launched.** Anthropic's new premium daily-driver model, replacing Claude Opus 4.8 at **identical pricing** ($5.00/$25.00 per MTok). Anthropic positions Opus 5 as approaching Fable 5-level intelligence at half Fable 5's price, and it becomes the default model on Claude Max and the strongest model available on Claude Pro. Model ID: `claude-opus-5`. On Anthropic's internal Frontier-Bench v0.1, Opus 5 scored 43.3% vs. 33.7% for Fable 5, 21.1% for Opus 4.8, and 34.4% for GPT-5.6 Sol. Anthropic says Opus 5's cyber safety classifiers intervene roughly 85% less often than Fable 5's, and the model carries no mandatory data-retention requirement (unlike Fable 5's 30-day retention). Fast Mode runs ~2.5× the standard speed at 2× the base price. See [Anthropic's announcement](https://www.anthropic.com/news/claude-opus-5).
>
> ✅ **July 20, 2026 — Fable 5 subscription-tier access permanently resolved.** After being extended three times (July 7 → July 12 → July 19), the promotional "included" window for Fable 5 on subscription plans ended and Anthropic announced a permanent split: **Max and Team Premium** plans keep Fable 5 included at **50% of weekly usage limits** indefinitely (no usage-credit draw). **Pro and Team Standard** plans lost bundled access and now run Fable 5 on **metered usage credits at the standard API rate** ($10/$50 per MTok), softened by a one-time **$100 credit** granted to eligible seats when the change took effect. The underlying API rate for Fable 5 is unchanged at $10/$50 per MTok regardless of billing mechanism.

> 📝 **July 14, 2026 update — Fable 5 usage-credit cliff extended again (twice now).** The July 1 restoration of Claude Fable 5 originally included it in Pro/Max/Team/select-Enterprise subscription plans for up to 50% of weekly usage limits **through July 7, 2026**, after which it was to move to metered usage-credit billing. That cutoff has since been **extended twice** — first to **July 12**, then to **July 19, 2026** — per third-party trackers monitoring Anthropic's usage dashboard messaging. Anthropic has not published a formal blog post about the extensions; the confirmed API rate for Fable 5 remains unchanged at **$10/$50 per MTok** regardless of which billing mode (subscription-included vs. metered credits) is in effect. *(Superseded by the July 20 permanent resolution above.)*
>
> 🌐 **July 13, 2026 — Anthropic begins localizing Claude.ai consumer pricing for India**, its second-largest market after the US (5.8% of global Claude usage). Claude Pro is listed at ₹2,000/mo (~$21, annual billing) vs. $17/mo in the US; Claude Max starts at ₹11,999/mo (~$125) vs. $100/mo in the US; Team starts at ₹2,399/seat/mo (~$25) vs. $20/mo in the US. **This is consumer subscription pricing only — it does not affect Claude API/developer pricing**, which remains USD-denominated globally. UPI payment support is not yet available; users still pay via card or app-store billing.

> 🔓 **July 1, 2026 — Fable 5 and Mythos 5 RESTORED after US government lifts export controls.** On June 12, 2026, the US government issued an export control directive suspending all access to Fable 5 and Mythos 5 (citing a reported non-universal jailbreak). On **June 30, 2026**, the Trump administration lifted those export controls after Anthropic worked with the government (including CAISI/NIST) to deploy an improved safety classifier that blocks the reported bypass technique in **over 99%** of cases. **Fable 5 became available globally starting July 1, 2026** across the Claude Platform, Claude.ai, Claude Code, and Claude Cowork; AWS Bedrock, Google Cloud, and Microsoft Foundry access continues to be re-enabled. **Mythos 5** was restored earlier, on June 26, 2026, for an approved set of US organizations under Project Glasswing, with broader international/domestic expansion ongoing. See [Anthropic's full statement](https://www.anthropic.com/news/redeploying-fable-5).
>
> - **Subscription access:** For Pro, Max, Team, and select Enterprise plans, Fable 5 is included for a limited share of weekly usage limits — see the July 14 update above for the latest (twice-extended) cutoff date — after which it moves to a **usage-credits** model (no longer bundled free).
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
| **Subscription access** | **Resolved July 20, 2026:** Max/Team Premium — included permanently at 50% of weekly usage limits. Pro/Team Standard — usage credits at API rates ($10/$50), softened by a one-time $100 credit |
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

### 🆕 Claude Opus 5 *(New Premium Daily Driver — Released July 24, 2026)*

> **July 24, 2026 — Claude Opus 5** replaces Claude Opus 4.8 as Anthropic's premium, everyday model — at **identical pricing**. Anthropic frames it as approaching Fable 5-level intelligence for daily professional work at half Fable 5's price, while reserving Fable 5 for the longest, most autonomous multi-day tasks. Opus 5 is now the default model on Claude Max and the strongest model available on Claude Pro. Knowledge cutoff is May 2026 (vs. January 2026 for Fable 5 and Opus 4.8).

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-5` |
| **Released** | July 24, 2026 |
| **Status** | ✅ Active — **New default on Claude Max; strongest model on Claude Pro** |
| **Input price** | $5.00 / MTok *(unchanged from Opus 4.8)* |
| **Output price** | $25.00 / MTok *(unchanged from Opus 4.8)* |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok *(90% off standard input, consistent with Opus 4.8)* |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Fast Mode** | ~2.5× standard speed at 2× base price ($10.00/$50.00 per MTok) |
| **Batch** | 50% off standard rates |
| **Context window** | 1,000,000 tokens |
| **Tool-use system prompt (`auto`/`none` — `any`/`tool`)** | 286 tokens — 406 tokens *(cheapest tool-use overhead of any active model)* |
| **Data retention** | No mandatory data-retention requirement for general access (unlike Fable 5's 30-day retention) |
| **Safety** | Cyber safety classifiers intervene ~85% less often than Fable 5's; flagged requests auto-route to another model by default (on by default in Claude.ai, Claude Code, Claude Cowork; available as an API option) rather than being refused outright |
| **Availability** | Claude API (`claude-opus-5`) · Claude.ai (Max default, strongest on Pro) · Claude Code · Amazon Bedrock · Claude Platform on AWS · Google Cloud · Microsoft Foundry |
| **Notable** | Anthropic reports Opus 5 beats Fable 5 on several benchmarks (Frontier-Bench v0.1: 43.3% vs. 33.7%; ARC-AGI 3: 30.2% vs. much lower prior scores; GDPVal-AA v2 highest of any model tested) while trailing Fable 5 on long-horizon coherence and CursorBench 3.2 by a narrow margin, and trailing Mythos 5 on offensive cybersecurity/biology research. Anthropic's internal behavioral audit reports Opus 5 as its most-aligned model to date. Beta features: mid-conversation tool swapping without invalidating the prompt cache, and automatic safety-fallback routing. |

---

### Claude Opus 4.8 *(🔄 Replaced by Opus 5 — still active)*

> 🔄 **REPLACED (July 24, 2026):** Claude Opus 5 has replaced Opus 4.8 as Anthropic's recommended premium/default model, at the identical $5/$25 price point. Opus 4.8 remains fully API-accessible and is not deprecated — it also continues to serve as the automatic safety-fallback target when Fable 5's classifiers flag a request.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-8` |
| **AWS Bedrock ID** | `anthropic.claude-opus-4-83` (Messages-API Bedrock endpoint only) |
| **Vertex AI ID** | `claude-opus-4-8` |
| **Released** | May 2026 |
| **Status** | ✅ Active — 🔄 Replaced by Opus 5 as default (July 24, 2026); still the safety-fallback target for Fable 5 |
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
| **Notable** | 1M context at standard pricing; Fast Mode at 2× base rate; still the safety-fallback target for Fable 5 cybersecurity/biology queries; **superseded by Opus 5** for new projects |

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
| **Tool-use system prompt (`auto`/`none` — `any`/`tool`)** | 354 tokens — 474 tokens |
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
| **Status** | ✅ Active — 🔄 Replaced by Sonnet 5 as default (June 30, 2026) |
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
| Claude Fable 5 | ❌ No | ✅ Yes (always on) | 🔓 Restored July 1, 2026. Cyber/bio queries auto-route to Opus 4.8. |
| Claude Mythos 5 | ❌ No | ✅ Yes (always on) | 🔒 Restricted to Project Glasswing (restored June 26, 2026). |
| Claude Opus 5 | ❌ No | ✅ Yes | 🆕 New default on Max/strongest on Pro (July 24, 2026) |
| Claude Opus 4.8 | ❌ No | ✅ Yes | 🔄 Replaced by Opus 5 as default; still active, Fast Mode at 2× pricing |
| Claude Sonnet 5 | ❌ No | ✅ Yes | Narrows gap with Opus-tier models; effort defaults to `high` |
| Claude Sonnet 4.6 | ✅ Yes | ✅ Yes | Replaced by Sonnet 5 as default; still active |
| Claude Haiku 4.5 | ✅ Yes | ❌ No | Fastest; extended thinking for budget reasoning |

> Source: `platform.claude.com/docs/en/about-claude/models/overview` and `platform.claude.com/docs/en/about-claude/pricing`, re-verified July 27, 2026.

---

## 🔧 Tools & Agents Pricing *(🆕 newly documented section — July 20, 2026)*

> Confirmed directly against the live `platform.claude.com/docs/en/about-claude/pricing` page. These charges are additive to standard per-model token pricing.

### Server-side tools

| Tool | Pricing |
|---|---|
| **Web search** | $10 per 1,000 searches, plus standard token costs for search-generated content. Each search counts as one use regardless of result count; failed searches are not billed. |
| **Web fetch** | No additional charge — standard token costs only for fetched content that enters context. Use `max_content_tokens` to cap consumption (avg 10kB page ≈ 2,500 tokens; 100kB doc ≈ 25,000 tokens; 500kB PDF ≈ 125,000 tokens). |
| **Code execution** | **Free when used alongside `web_search_20260209`+ or `web_fetch_20260209`+.** Otherwise billed by execution time (5-min minimum): **1,550 free container-hours/month per org**, then **$0.05/hour per container**. Files attached to a request bill execution time even if the tool isn't invoked. |
| **Bash tool** | Adds 325 input tokens (Opus 4.7/4.8/5) or 244 tokens (Opus 4.6, Sonnet 4.6 and earlier) on top of the standard tool-use system prompt. |
| **Text editor tool** | Adds 700 input tokens (Claude 4.x `text_editor_20250429`) on top of standard tool-use overhead. |
| **Computer use tool** | Adds 466–499 system-prompt tokens plus 735 tokens per tool definition (Claude 4.x); screenshots billed at standard vision-token rates. |

### Tool-use system-prompt overhead (per request, when ≥1 tool is defined)

| Model | `auto`/`none` | `any`/`tool` |
|---|---|---|
| Claude Opus 5 | 286 tokens | 406 tokens |
| Claude Opus 4.8 | 290 tokens | 410 tokens |
| Claude Opus 4.7 | 675 tokens | 804 tokens |
| Claude Opus 4.6 | 497 tokens | 589 tokens |
| Claude Opus 4.5 | 496 tokens | 588 tokens |
| Claude Sonnet 5 | 354 tokens | 474 tokens |
| Claude Sonnet 4.6 | 497 tokens | 589 tokens |
| Claude Sonnet 4.5 | 496 tokens | 588 tokens |
| Claude Haiku 4.5 | 496 tokens | 588 tokens |
| Claude Haiku 3.5 (legacy) | 264 tokens | 355 tokens |

> 🆕 **Claude Opus 5 now has the cheapest tool-use overhead of any active model** (286/406 tokens) — even lower than Opus 4.8's 290/410, confirmed on the live pricing page's tool-use pricing table.
> These tokens are billed as ordinary input tokens at the model's standard rate — they are not a separate line item.

### Claude Managed Agents *(billed on tokens + session runtime)*

| SKU | Rate | Notes |
|---|---|---|
| **Session runtime** | $0.08 per session-hour | Metered to the millisecond, accrues only while session status is `running` (not `idle`/`rescheduling`/`terminated`) |
| **Tokens** | Standard per-model rates | Prompt caching multipliers apply identically; web search inside a session still costs $10/1,000 searches |
| **Not applicable** | Batch API discount, Fast Mode premium, data residency multiplier, cloud-platform (Bedrock/Vertex) pricing | Managed Agents sessions are stateful/interactive — none of these modifiers apply |

**Worked example** (1-hour Opus 5 session, 50K input / 15K output tokens, no caching): $0.25 (input) + $0.375 (output) + $0.08 (runtime) = **$0.705**. With 40K of the 50K input tokens served from cache: **$0.525**.

---

## 🆕 Platform Feature: Claude Tag *(Teams Product — June 23, 2026)*

> **June 23, 2026:** Anthropic launched **Claude Tag** (`@Claude`) — a new way for teams to mention and interact with Claude directly within shared workspaces. This is a **product/teams feature**, not a new API model. Billed at standard API token rates using the underlying Claude model.

## 🆕 Platform Feature: Claude Security (Enterprise — Public Beta)

> **May 2026:** Anthropic launched **Claude Security** in public beta for Claude Enterprise customers, purpose-built for security operations workflows. Billed at standard API token rates using the underlying model.

## 🌐 Consumer Pricing Localization (India — July 13, 2026)

> Anthropic began rolling out **rupee-denominated pricing** for Claude.ai consumer plans in India, its second-largest market after the US. Claude Pro: ₹2,000/mo (~$21, annual billing) vs. $17/mo in the US. Claude Max: ₹11,999/mo (~$125) vs. $100/mo in the US. Team: ₹2,399/seat/mo (~$25) vs. $20/mo in the US. **This affects consumer subscriptions only — Claude API/developer pricing is unaffected and remains USD-denominated globally.** UPI payment support is not yet enabled (card/app-store billing only).

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

### ⚠️ LEGACY — Claude Opus 4.7 *(Fast Mode ❌ REMOVED July 24, 2026)*

> ✅ **Confirmed removed on schedule.** Fast Mode for Claude Opus 4.7 was deprecated with a published removal date of July 24, 2026 (the same day Claude Opus 5 launched); the live `platform.claude.com/docs/en/about-claude/pricing` page now explicitly states that requests with `speed: "fast"` against Opus 4.7 **return an error**. This is now a confirmed removal, not a scheduled one.

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-7` |
| **Status** | ⚠️ LEGACY — Fast Mode ❌ REMOVED July 24, 2026 (confirmed on live pricing page) |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode (input/output)** | ❌ REMOVED — `speed: "fast"` requests now return an error (was $30.00/$150.00 per MTok, 6×, prior to removal) |
| **Context window** | 1,000,000 tokens |
| **Migration** | → **Claude Opus 5** or **Opus 4.8** (both support Fast Mode at 2× standard pricing, $10/$50) |

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
| **Migration** | → **Claude Opus 5** or **Opus 4.8** |

---

### ⚠️ LEGACY — Claude Sonnet 4.5

| Field | Value |
|---|---|
| **Model ID** | `claude-sonnet-4-5` |
| **Status** | ⚠️ LEGACY — 1M context beta RETIRED April 30, 2026; max context now 200K. Still listed on the live model-pricing table (not yet a deprecated/retired model per Anthropic's docs) |
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
| **Migration** | → **Claude Opus 5** or **Opus 4.8** (1M context, 128k output) |

---

### ⚠️ LEGACY — Claude Opus 4.1

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-1` |
| **Status** | ⚠️ LEGACY (deprecated, per live pricing page) |
| **Input price** | $15.00 / MTok |
| **Output price** | $75.00 / MTok |
| **Migration** | → **Claude Opus 5** or **Opus 4.8** ($5/$25) — 67% cheaper |

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
| **Migration** | → **Claude Opus 5** or **Opus 4.8** ($5/$25) — 67% cheaper |

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
| Claude 3 Opus | ⚠️ DEPRECATED Jan 2026 — available by request | → Claude Opus 5 or 4.8 |
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
| **🆕 Opus 5 replaces Opus 4.8** | Same $5/$25 price, more capability — near-Fable-5 performance on many benchmarks at half Fable 5's price. Default reason to migrate off Opus 4.8 for new projects |
| **🆕 Opus 5 has the cheapest tool-use overhead** | 286/406 tokens (auto/none — any/tool) vs. 290/410 for Opus 4.8 — a small but real savings for tool-heavy agents at scale |
| **🔓 Fable 5 restored** | $10/$50 — 2× Opus 5/Opus 4.8. Safety-flagged queries auto-route to Opus 4.8/Opus 5 and bill at that model's rates |
| **🆕 Sonnet 5 introductory pricing** | $2/$10 per MTok through Aug 31, 2026 — lock in savings before the Sept 1 jump to $3/$15 |
| **Opus 5 / Opus 4.8 Fast Mode** | Both run Fast Mode at $10/$50 (2× standard); Opus 4.7 Fast Mode was $30/$150 (6×) and is now confirmed **removed** as of July 24, 2026 |
| **⚠️ Opus 4.6 Fast Mode removed** | As of June 29, 2026, billed at standard $5/$25 |
| **⚠️ Opus 4.7 Fast Mode removed** | As of July 24, 2026 (confirmed on live pricing page — `speed: "fast"` requests now error), billed at standard $5/$25 |
| **US-only inference (data residency)** | 1.1× pricing on Opus 4.6+, Sonnet 4.6+, Sonnet 5, and Fable 5/Mythos 5 |
| **Thinking modes** | Adaptive: Fable 5, Mythos 5, Opus 5, Opus 4.8, Sonnet 5, Sonnet 4.6. Extended: Sonnet 4.6, Haiku 4.5 (**not** on Sonnet 5/Opus 5/Fable 5/Mythos 5) |
| **Tokenizer note** | Fable 5, Mythos 5, Opus 4.7+, and Sonnet 5 use a newer tokenizer producing ~30% more tokens for the same text vs. Sonnet 4.6-and-earlier |
| **⚠️ Sonnet 4 + Opus 4 RETIRED** | Retired June 15, 2026 ❌ on Claude API — Sonnet 4 → Sonnet 5/4.6, Opus 4 → Opus 5/4.8 |
| **✅ Fable 5 subscription cliff resolved** | Permanently split July 20, 2026: Max/Team Premium keep 50%-of-limits included access; Pro/Team Standard moved to metered usage credits at the $10/$50 API rate (one-time $100 credit granted) |
| **🌐 India consumer pricing** | Now localized in INR (Pro ₹2,000/mo, Max ₹11,999/mo, Team ₹2,399/seat/mo) — API/developer pricing unaffected |
| **🆕 Code execution + web search/fetch combo** | Free code execution when paired with `web_search_20260209`+/`web_fetch_20260209`+ — otherwise $0.05/hr per container after 1,550 free org-hours/month |
| **🆕 Claude Managed Agents** | $0.08/session-hour runtime (billed only while `running`) + standard token rates — no Batch/Fast Mode/data-residency modifiers apply |
| **Tool-use overhead varies by model** | Opus 5's tool-use system prompt (286–406 tokens) is now the cheapest of any active model, edging out Opus 4.8 (290–410 tokens) and far cheaper than Opus 4.7's former 675–804 tokens — a meaningful cost delta for tool-heavy agents at scale |

---

*Sources last verified: August 3, 2026 against `platform.claude.com/docs/en/about-claude/pricing`, `anthropic.com/news`, and `anthropic.com/news/claude-opus-5`. All active model prices (Fable 5, Mythos 5, Opus 5, Opus 4.8, Opus 4.7 (deprecated), Opus 4.6, Opus 4.5, Sonnet 5, Sonnet 4.6, Sonnet 4.5, Haiku 4.5, Haiku 3.5 (retired)) re-confirmed unchanged directly against the live model-pricing table. **Key confirmation this cycle:** Claude Opus 4.7's Fast Mode, previously flagged as "deprecated, scheduled removal July 24, 2026," is now **confirmed removed** — the live pricing page states Fast Mode requests against Opus 4.7 return an error. Also newly captured: Claude Opus 5's tool-use system-prompt overhead (286/406 tokens, `auto`/`none` vs. `any`/`tool`), now the cheapest of any active model, from the live pricing page's tool-use pricing table. Checked `anthropic.com/news` through July 30, 2026 (most recent entry found) — no new model releases since Claude Opus 5 (July 24, 2026). Fast mode remains available only on Opus 5 and Opus 4.8, both at $10/$50 per MTok. No other pricing changes detected.*
