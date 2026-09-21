# 🟠 Anthropic — Claude Model Cards

> **Last updated:** 2026-09-21
> **Source:** https://www.anthropic.com/pricing · https://claude.com/pricing · https://platform.claude.com/docs/en/about-claude/models/overview · https://platform.claude.com/docs/en/about-claude/pricing · https://www.anthropic.com/claude-fable-and-mythos-5-1 · https://www.anthropic.com/news
> **Scraped / verified:** 2026-09-21 — ✅ **Re-verified against the live `platform.claude.com/docs/en/about-claude/pricing` and `claude.com/pricing` pages.** Every active model price (Fable 5.1 $10/$50 w/ $0.25 cache-read, Mythos 5.1, Fable 5, Mythos 5, Opus 5 $5/$25, Opus 4.8, Sonnet 5 $2/$10 permanent, Sonnet 4.6, Haiku 4.5) and the full legacy table (down to Opus 4.1, Opus 4, Sonnet 4, Haiku 3.5) are **byte-for-byte unchanged** since the September 14 refresh. Checked `anthropic.com/news` through September 21, 2026 — three new **non-pricing** items found: the Life Sciences Verification Program (LSVP) opened in beta (Sept 17), an embedded-evaluation partnership with Accenture worth $1B+ over five years (Sept 18), and a Claude R&D Automation Index research disclosure (Sept 17), plus a Cowork/chat product merge (Sept 16). No new model releases, retirements, or price changes found this cycle.

All prices are **USD per million tokens (MTok)**. Batch API gives a flat **50% discount** on all models. Prompt caching gives up to **90% off** on repeated input context (up to **97.5% off** on Fable 5.1 / Mythos 5.1 cache reads — see below).

> 🆕 **September 1, 2026 — Claude Fable 5.1 and Claude Mythos 5.1 launched.** Anthropic's new most-advanced models for coding and knowledge work, described as offering "an early glimpse of how AI models will contribute to scientific progress." Fable 5.1 and Mythos 5.1 are **the same underlying model** with different safeguard levels (Fable 5.1 = generally available; Mythos 5.1 = trusted-access only, for vetted cybersecurity/life-sciences work). Headline price is unchanged at $10/$50 per MTok, but **cache-read (cache-hit) pricing drops 75%**, from $1.00/MTok (0.1× multiplier) to **$0.25/MTok (0.025× multiplier)** — Anthropic estimates this cuts typical workload costs by **~25%** and highly agentic/cache-heavy workload costs by **up to ~45%**. See the dedicated section below. Model ID: `claude-fable-5-1`. See [Anthropic's announcement](https://www.anthropic.com/claude-fable-and-mythos-5-1).
>
> ✅ **September 1, 2026 — Claude Sonnet 5's introductory pricing is now PERMANENT.** The $2/$10 per MTok (input/output) rate announced at Sonnet 5's June 30, 2026 launch as introductory pricing through August 31, 2026 **is now the standard, permanent price**. The previously scheduled increase to $3/$15 per MTok on September 1, 2026 **will not occur**. This is a pricing win for existing Sonnet 5 users — no action needed.
>
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

> 🆕 **June 30, 2026 — Claude Sonnet 5 launched.** Anthropic's most agentic Sonnet-tier model yet, replacing Claude Sonnet 4.6 as the default model for Free and Pro plans (also available on Max, Team, Enterprise, Claude Code, and the Claude Platform). Narrows the performance gap with Opus 4.8 on agentic coding, tool use, and knowledge work while remaining priced at the Sonnet tier. Model ID: `claude-sonnet-5`. See [announcement](https://www.anthropic.com/news/claude-sonnet-5). *(Introductory $2/$10 pricing made permanent September 1, 2026 — see above.)*
>
> 🆕 **June 23, 2026 — Claude Tag launched.** @Claude is a new Teams/workspace product integration that allows teams to mention and interact with Claude directly in platforms. This is a **product feature**, not a new API model — billed at standard API token rates using the underlying model. See [announcement](https://www.anthropic.com/news/introducing-claude-tag).
>
> ✅ **Claude Sonnet 4 + Opus 4 RETIRED on June 15, 2026. ❌** API calls to `claude-sonnet-4-20250514` and `claude-opus-4-20250514` now return errors (except via Amazon Bedrock and Google Cloud, where they remain available per Anthropic's model deprecation policy). Migration: Sonnet 4 → Sonnet 5 or Sonnet 4.6 (same price, 1M context); Opus 4 → Opus 4.8 ($5/$25, 67% cheaper).

---

## ✅ Active / Recommended Models

### 🆕 Claude Fable 5.1 *(Released September 1, 2026 — Most Advanced Model for Coding & Knowledge Work)*

> **September 1, 2026 — Claude Fable 5.1** replaces Claude Fable 5 as Anthropic's most advanced model for coding and knowledge work. Fable 5.1 and Mythos 5.1 are the **same underlying model**, differing only in safeguard configuration. Early-access partners (Jane Street, Cognition/Devin, Millennium, MongoDB, Datadog, SpaceXAI, and others) report it matches or beats Fable 5 and Opus 5 on coding/agentic benchmarks while using roughly half the tokens. Anthropic's own comparison table shows Fable 5.1 scoring 55.8% on Terminal-Bench 4.0 (60.9% as Mythos 5.1) vs. 42.0% for Fable 5 and 52.3% for Opus 5, and 31.4% on AutomationBench vs. 17.1% for Fable 5.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-fable-5-1` |
| **Released** | September 1, 2026 |
| **Status** | ✅ Active — **Most advanced model for coding & knowledge work; replaces Fable 5 as flagship** |
| **Input price** | $10.00 / MTok *(unchanged from Fable 5)* |
| **Output price** | $50.00 / MTok *(unchanged from Fable 5)* |
| **Cache write (5 min)** | $12.50 / MTok |
| **Cache write (1 hr)** | $20.00 / MTok |
| **Cache read (cache hit)** | 📉 **$0.25 / MTok** *(0.025× multiplier — 75% cheaper than Fable 5's $1.00/MTok 0.1× rate)* |
| **Batch input** | $5.00 / MTok *(50% off)* |
| **Batch output** | $25.00 / MTok *(50% off)* |
| **US-only inference** | 1.1× pricing |
| **Context window** | 1,000,000 tokens (standard pricing — no long-context surcharge) |
| **Max output** | 128,000 tokens |
| **Thinking mode** | Adaptive only; defaults to **High effort in Claude Code**, **Medium in Claude Cowork/Claude.ai** |
| **Tokenizer** | Newer tokenizer (shared with Fable 5/Opus 4.7+) — ~30% more tokens for the same text vs. Sonnet 4.6-and-earlier |
| **Availability** | Claude API (`claude-fable-5-1`) · Claude.ai · Claude Code · Claude Cowork · Amazon Web Services · Google Cloud · Microsoft Azure |
| **Data retention** | Enterprise Frontier Safeguards (EFS) — customer-controlled cloud storage, rolling out in phases starting **fall 2026** — will offer zero-data-retention-equivalent privacy. Until EFS ships, eligible customers can use Fable 5.1 (and Fable 5) with **zero data retention** today |
| **Safety** | Cyber safeguards fire ~60% fewer false positives than Fable 5's; Fable 5.1 can now be used to **discover** software vulnerabilities (not develop exploits — those still route to Opus models). Biology safeguards fire 85% less often on benign elementary-biology/medical queries (shared improvement with Fable 5) |
| **Anti-distillation** | New API accounts created from Sept 1, 2026 onward can no longer manually edit Claude's prior-turn context while preserving the prior thinking transcript — closes a documented distillation technique |
| **Watermarking** | Outputs include an invisible statistical watermark (EU AI Act Code of Practice on Transparency of AI-Generated Content compliance) — no effect on output quality; a detection API is in private preview |
| **Notable** | Estimated **~25% cheaper for typical workloads** and **up to ~45% cheaper for highly agentic workloads** vs. Fable 5, purely from the cache-read price cut; Cognition (Devin) reports moving all Opus 5 traffic to Fable 5.1 at launch due to the new cache economics |

---

### 🔒 Claude Mythos 5.1 *(Trusted Access — Released September 1, 2026)*

> **September 1, 2026 —** Identical underlying model to Fable 5.1, with more permissive cybersecurity and life-sciences safeguards for vetted individuals/organizations. Anthropic reports Mythos 5.1 designed high-affinity protein binders 10× stronger than the best entries in Adaptyv Bio's public protein-design competitions, and used custom GPU kernels to speed up seven open-source genomics/protein models by up to 2.5×, cutting estimated GPU costs 30–60% on genome-wide analyses.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-mythos-5-1` |
| **Released** | September 1, 2026 |
| **Status** | 🔒 Trusted access only — replaces Mythos 5 |
| **Pricing** | $10.00 / MTok input · $50.00 / MTok output (identical to Fable 5.1, including the $0.25/MTok cache-read rate) |
| **Context window** | 1,000,000 tokens · Max output: 128,000 tokens |
| **Access** | **Cyber Verification Program (CVP)** — [apply here](https://portal.anthropic.com/programs/cvp) — for defensive cybersecurity work; **Life Sciences Verification Program (LSVP)** — developed with the US government — for professional biology/life-sciences R&D. Now in beta and open to broader applications (see Sept 17, 2026 update below); expanding internationally |
| **Notable** | Strongest cyber capabilities of any Anthropic model released to date (with cyber safeguards off for evaluation), but still falls in the lower risk category of Anthropic's Frontier Compliance Framework; no critical-severity jailbreak found after external red-teaming (Gray Swan + two other firms). Now also powers **Claude Security** (codebase vulnerability scanning product) |

---

### Claude Fable 5 *(🔄 Replaced by Fable 5.1 — still active)*

> 🔄 **REPLACED (September 1, 2026):** Claude Fable 5.1 has replaced Fable 5 as Anthropic's most advanced model. Fable 5 remains fully API-accessible at unchanged pricing and is not deprecated.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-fable-5` |
| **AWS Bedrock ID** | `anthropic.claude-fable-5` |
| **Vertex AI ID** | `claude-fable-5` |
| **Released** | June 9, 2026 · Suspended June 12–30, 2026 · Restored July 1, 2026 |
| **Status** | ✅ Active — 🔄 Replaced by Fable 5.1 as flagship (September 1, 2026) |
| **Input price** | $10.00 / MTok |
| **Output price** | $50.00 / MTok |
| **Cache write (5 min)** | $12.50 / MTok |
| **Cache write (1 hr)** | $20.00 / MTok |
| **Cache read** | $1.00 / MTok *(still the older 0.1× rate — not discounted to Fable 5.1's $0.25/MTok)* |
| **Batch input** | $5.00 / MTok *(50% off)* |
| **Batch output** | $25.00 / MTok *(50% off)* |
| **Context window** | 1,000,000 tokens |
| **Max output** | 128,000 tokens |
| **Availability** | Claude API · Claude.ai · Claude Code · Claude Cowork · Claude Platform on AWS · Amazon Bedrock · Google Vertex AI · Microsoft Foundry |
| **Notable** | Same headline price as Fable 5.1 but without the cheaper cache-read rate — **Fable 5.1 is a strict cost/performance upgrade** for cache-heavy workloads |

---

### 🔒 Claude Mythos 5 *(🔄 Replaced by Mythos 5.1 — still active for approved orgs)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-mythos-5` |
| **Status** | 🔒 Restricted — 🔄 Replaced by Mythos 5.1 (September 1, 2026); still active for previously approved Project Glasswing organizations |
| **Pricing** | $10.00 / MTok input · $50.00 / MTok output (cache read at older $1.00/MTok rate) |
| **Context window** | 1,000,000 tokens · Max output: 128,000 tokens |
| **Access** | [Project Glasswing](https://anthropic.com/glasswing) — contact Anthropic, AWS, or Google Cloud account team |

---

### Claude Opus 5 *(Premium Daily Driver — Released July 24, 2026)*

> **July 24, 2026 — Claude Opus 5** replaces Claude Opus 4.8 as Anthropic's premium, everyday model — at **identical pricing**. Anthropic frames it as approaching Fable-level intelligence for daily professional work at a fraction of Fable's price, while reserving Fable 5.1 for the longest, most autonomous multi-day tasks. Opus 5 is the default model on Claude Max and the strongest model available on Claude Pro. Knowledge cutoff is May 2026.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-5` |
| **Released** | July 24, 2026 |
| **Status** | ✅ Active — **Default on Claude Max; strongest model on Claude Pro** |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok *(standard 0.1× multiplier — not discounted like Fable 5.1)* |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Fast Mode** | ~2.5× standard speed at 2× base price ($10.00/$50.00 per MTok) |
| **Context window** | 1,000,000 tokens |
| **Tool-use system prompt (`auto`/`none` — `any`/`tool`)** | 286 tokens — 406 tokens *(cheapest tool-use overhead of any active model)* |
| **Availability** | Claude API (`claude-opus-5`) · Claude.ai (Max default, strongest on Pro) · Claude Code · Amazon Bedrock · Claude Platform on AWS · Google Cloud · Microsoft Foundry |
| **Notable** | Anthropic's internal comparison table (published with the Fable 5.1 launch) shows Opus 5 scoring 29.0–30.0% on Terminal-Bench-Science 0.1 and 52.3% on Terminal-Bench 4.0 — behind Fable 5.1 (52.6% / 55.8%) but ahead of Fable 5 and GPT-5.6 Sol on most benchmarks shown |

---

### Claude Opus 4.8 *(🔄 Replaced by Opus 5 — still active)*

> 🔄 **REPLACED (July 24, 2026):** Claude Opus 5 has replaced Opus 4.8 as Anthropic's recommended premium/default model, at the identical $5/$25 price point. Opus 4.8 remains fully API-accessible and is not deprecated — it also continues to serve as the automatic safety-fallback target when Fable 5.1's classifiers flag a request.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-8` |
| **AWS Bedrock ID** | `anthropic.claude-opus-4-83` (Messages-API Bedrock endpoint only) |
| **Vertex AI ID** | `claude-opus-4-8` |
| **Released** | May 2026 |
| **Status** | ✅ Active — 🔄 Replaced by Opus 5 as default (July 24, 2026); still the safety-fallback target for Fable 5.1 |
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
| **Notable** | 1M context at standard pricing; Fast Mode at 2× base rate; still the safety-fallback target for Fable 5.1 cybersecurity/biology queries; **superseded by Opus 5** for new projects |

---

### Claude Sonnet 5 *(Default Sonnet-Tier Model — Released June 30, 2026; permanent pricing confirmed Sept 1, 2026)*

> **June 30, 2026 — Claude Sonnet 5** is Anthropic's most agentic Sonnet-class model yet, replacing **Claude Sonnet 4.6** as the default model for Claude Free and Pro plans. ✅ **September 1, 2026:** The $2/$10 per MTok launch price is now **permanent** — the previously announced increase to $3/$15 will not occur.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-5` |
| **AWS Bedrock ID** | `anthropic.claude-sonnet-5` |
| **Vertex AI ID** | `claude-sonnet-5` |
| **Released** | June 30, 2026 |
| **Status** | ✅ Active — **Default Sonnet-Tier Model; $2/$10 pricing now permanent (Sept 1, 2026)** |
| **Input price** | **$2.00 / MTok** *(permanent, not introductory)* |
| **Output price** | **$10.00 / MTok** *(permanent, not introductory)* |
| **Cache write (5 min)** | $2.50 / MTok |
| **Cache write (1 hr)** | $4.00 / MTok |
| **Cache read** | $0.20 / MTok |
| **Batch input** | $1.00 / MTok |
| **Batch output** | $5.00 / MTok |
| **Context window** | 1,000,000 tokens (at standard pricing — no surcharge) |
| **Max output** | 128,000 tokens (sync) / 300,000 tokens (Batch API with beta header) |
| **Extended thinking** | ❌ No |
| **Adaptive thinking** | ✅ Yes (effort defaults to `high` on Claude API and Claude Code) |
| **Tool-use system prompt (`auto`/`none` — `any`/`tool`)** | 354 tokens — 474 tokens |
| **Tokenizer** | Newer tokenizer (same generation as Opus 4.7+/Fable 5.1) — produces ~30% more tokens than Sonnet 4.6 for the same text |
| **Availability** | Claude API · Claude.ai (Free/Pro/Max/Team/Enterprise) · Claude Code · Claude Platform on AWS · Amazon Bedrock · Google Cloud · Microsoft Foundry |
| **Notable** | Default model for Free/Pro plans; strict improvement over Sonnet 4.6 on agentic benchmarks; the cheapest Anthropic model with 1M context at standard pricing; **first Sonnet-tier model with real-time cybersecurity safeguards** — prohibited/high-risk cyber requests are refused with `stop_reason: "refusal"` (returned as HTTP 200, not an error) |

> ✅ **September 1, 2026 — pricing confirmed permanent at $2/$10 per MTok.** The scheduled Sept 1 increase to $3/$15 was cancelled.
> 🔄 **Replaces Claude Sonnet 4.6** as Anthropic's recommended default mid-tier model.

---

### Claude Sonnet 4.6 *(🔄 Replaced by Sonnet 5 as default — still active)*

> 🔄 **REPLACED (June 30, 2026):** Claude Sonnet 5 has replaced Sonnet 4.6 as Anthropic's default Sonnet-tier / recommended model. Sonnet 4.6 remains fully API-accessible at unchanged pricing and is not deprecated. Note that Sonnet 5 is now **cheaper** than Sonnet 4.6 ($2/$10 vs. $3/$15), making Sonnet 4.6 primarily a legacy-compatibility option.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4-6` |
| **Released** | February 17, 2026 |
| **Status** | ✅ Active — 🔄 Replaced by Sonnet 5 as default (June 30, 2026); now the more expensive of the two |
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
| **Notable** | Still a solid balance of intelligence, cost, and speed; retains Extended Thinking, which Sonnet 5 lacks; **superseded by Sonnet 5** for new projects, which is now both cheaper and more capable for most use cases |

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
| Claude Fable 5.1 | ❌ No | ✅ Yes | 🆕 Released Sept 1, 2026. Defaults: High effort (Claude Code), Medium (Cowork/Claude.ai). Cyber/bio queries auto-route to Opus models. |
| Claude Mythos 5.1 | ❌ No | ✅ Yes | 🔒 Trusted access only (CVP / LSVP). |
| Claude Fable 5 | ❌ No | ✅ Yes (always on) | 🔄 Replaced by Fable 5.1; still active. |
| Claude Mythos 5 | ❌ No | ✅ Yes (always on) | 🔄 Replaced by Mythos 5.1; still active for approved orgs. |
| Claude Opus 5 | ❌ No | ✅ Yes | Default on Max/strongest on Pro. |
| Claude Opus 4.8 | ❌ No | ✅ Yes | 🔄 Replaced by Opus 5 as default; still active, Fast Mode at 2× pricing |
| Claude Sonnet 5 | ❌ No | ✅ Yes | $2/$10 pricing now permanent (Sept 1, 2026); effort defaults to `high` |
| Claude Sonnet 4.6 | ✅ Yes | ✅ Yes | Replaced by Sonnet 5 as default; still active; only Sonnet-tier model with Extended Thinking |
| Claude Haiku 4.5 | ✅ Yes | ❌ No | Fastest; extended thinking for budget reasoning |

> Source: `platform.claude.com/docs/en/about-claude/models/overview` and `platform.claude.com/docs/en/about-claude/pricing`, re-verified September 21, 2026 — unchanged.

---

## 🔧 Tools & Agents Pricing

> Confirmed directly against the live `platform.claude.com/docs/en/about-claude/pricing` page. These charges are additive to standard per-model token pricing.

### Server-side tools

| Tool | Pricing |
|---|---|
| **Web search** | $10 per 1,000 searches, plus standard token costs for search-generated content. Each search counts as one use regardless of result count; failed searches are not billed. |
| **Web fetch** | No additional charge — standard token costs only for fetched content that enters context. Use `max_content_tokens` to cap consumption (avg 10kB page ≈ 2,500 tokens; 100kB doc ≈ 25,000 tokens; 500kB PDF ≈ 125,000 tokens). |
| **Code execution** | **Free when used alongside `web_search_20260209`+ or `web_fetch_20260209`+.** Otherwise billed by execution time (5-min minimum): **1,550 free container-hours/month per org** (equivalently ~50 free hours/day per `claude.com/pricing`), then **$0.05/hour per container**. Files attached to a request bill execution time even if the tool isn't invoked. |
| **Bash tool** | Adds 325 input tokens (Opus 4.7/4.8/5) or 244 tokens (Opus 4.6, Sonnet 4.6 and earlier) on top of the standard tool-use system prompt. |
| **Text editor tool** | Adds 700 input tokens (Claude 4.x `text_editor_20250429`) on top of standard tool-use overhead. |
| **Computer use tool** | New `computer_toolset_20260801`: ~4,500 input tokens overhead (~4,520 on Fable 5/5.1, Mythos 5/5.1, Opus 5, Opus 4.8; ~4,590 on Sonnet 5), covering member tool definitions + tool-use system prompt. Disabling `zoom` removes ~410 tokens. Earlier tool versions (`computer_20251124`/`computer_20250124`): 466–499 system-prompt tokens + ~735 tokens per tool definition. Screenshots billed at standard vision-token rates. |
| **Browser use tool** | `browser_toolset_20260801`: ~6,600 input tokens overhead (~6,610 on Fable 5/5.1, Mythos 5/5.1, Opus 5, Opus 4.8; ~6,670 on Sonnet 5). Enabling all four optional members adds ~880 tokens. Text tool results (accessibility trees, page text, console/network entries) billed as ordinary input tokens. |

### Tool-use system-prompt overhead (per request, when ≥1 tool is defined)

| Model | `auto`/`none` | `any`/`tool` |
|---|---|---|
| Claude Opus 5 | 286 tokens | 406 tokens |
| Claude Opus 4.8 | 290 tokens | 410 tokens |
| Claude Opus 4.7 | 675 tokens | 804 tokens |
| Claude Opus 4.6 | 497 tokens | 589 tokens |
| Claude Opus 4.5 | 496 tokens | 588 tokens |
| Claude Opus 4.1 (retired, except Bedrock/Google Cloud) | 313 tokens | 315 tokens |
| Claude Opus 4 (retired, except Google Cloud) | 313 tokens | 315 tokens |
| Claude Sonnet 5 | 354 tokens | 474 tokens |
| Claude Sonnet 4.6 | 497 tokens | 589 tokens |
| Claude Sonnet 4.5 | 496 tokens | 588 tokens |
| Claude Sonnet 4 (retired, except Bedrock/Google Cloud) | 313 tokens | 315 tokens |
| Claude Haiku 4.5 | 496 tokens | 588 tokens |
| Claude Haiku 3.5 (retired, except Bedrock/Google Cloud) | 264 tokens | 355 tokens |

> Claude Opus 5 has the cheapest tool-use overhead of any active model (286/406 tokens). These tokens are billed as ordinary input tokens at the model's standard rate — they are not a separate line item. Fable 5.1 and Mythos 5.1 do not yet have a separately published tool-use overhead row on the live pricing page as of this refresh; they are expected to inherit Fable 5's figures.

### Claude Managed Agents *(billed on tokens + session runtime)*

| SKU | Rate | Notes |
|---|---|---|
| **Session runtime** | $0.08 per session-hour | Metered to the millisecond, accrues only while session status is `running` (not `idle`/`rescheduling`/`terminated`) |
| **Tokens** | Standard per-model rates | Prompt caching multipliers apply identically; web search inside a session still costs $10/1,000 searches |
| **Not applicable** | Batch API discount, Fast Mode premium (unless `model.speed: "fast"`), cloud-platform (Bedrock/Vertex) pricing | Managed Agents sessions are stateful/interactive — Batch mode and partner-cloud pricing don't apply |

**Worked example** (1-hour Opus 5 session, 50K input / 15K output tokens, no caching): $0.25 (input) + $0.375 (output) + $0.08 (runtime) = **$0.705**. With 40K of the 50K input tokens served from cache: **$0.525**.

---

## 🆕 Enterprise Frontier Safeguards (EFS) — announced September 1, 2026

> A new privacy model for enterprise customers: data is stored on **customer-controlled cloud infrastructure** (AWS, Google Cloud, or Microsoft Azure) rather than Anthropic's systems, with any human review defaulting to the customer rather than Anthropic — delivering zero-data-retention-equivalent privacy while retaining state-of-the-art misuse detection. Developed with 100+ enterprise customers across financial services, healthcare, manufacturing, telecom, law, retail, and the public sector. Rolling out in phases starting **fall 2026** across Claude Code, Claude Enterprise, the Claude Platform, Amazon Bedrock, Claude Platform on AWS, Google's Agent Platform, and Microsoft Foundry. This is a **data-governance feature, not a separate priced model** — eligible customers can use Fable 5.1 (and Fable 5) with zero data retention today, ahead of full EFS availability.

## 🆕 Life Sciences Verification Program (LSVP) — beta opened September 17, 2026

> **September 17, 2026:** Anthropic opened the **Life Sciences Verification Program (LSVP)** in beta, giving verified life science professionals and organizations access to **Mythos, Opus, and Sonnet models with a refined, more permissive set of safeguards for biology-related work**. Dozens of organizations were already onboarded via an early-access program; applications are now open to the broader life-science community. This is an **access/safeguard program, not a separate priced model or a pricing change** — approved users are billed at the standard rate for whichever underlying Claude model they use. See [Anthropic's announcement](https://www.anthropic.com/news/life-sciences-verification-program).

## 🆕 Embedded Evaluation Partnership with Accenture — announced September 18, 2026

> **September 18, 2026:** Anthropic and Accenture (via its Faculty AI division) announced a partnership pioneering **"embedded evaluation"** — independent evaluators operating inside Anthropic with employee-level access to observe training decisions and deployment governance in real time. Each party expects to invest **at least $1 billion over five years**. This is a **safety-governance and enterprise-credibility initiative, not a pricing change** — no new models or price changes accompanied this announcement.

## 🆕 Platform Feature: Claude Tag *(Teams Product — June 23, 2026)*

> **June 23, 2026:** Anthropic launched **Claude Tag** (`@Claude`) — a new way for teams to mention and interact with Claude directly within shared workspaces. This is a **product/teams feature**, not a new API model. Billed at standard API token rates using the underlying Claude model.

## 🆕 Platform Feature: Claude Security (Enterprise — Public Beta)

> **May 2026:** Anthropic launched **Claude Security** in public beta for Claude Enterprise customers, purpose-built for security operations workflows. Billed at standard API token rates using the underlying model. As of September 1, 2026, Claude Security is powered by **Claude Mythos 5.1**.

## 🌐 Consumer Pricing Localization (India — July 13, 2026)

> Anthropic began rolling out **rupee-denominated pricing** for Claude.ai consumer plans in India, its second-largest market after the US. Claude Pro: ₹2,000/mo (~$21, annual billing) vs. $17/mo in the US. Claude Max: ₹11,999/mo (~$125) vs. $100/mo in the US. Team: ₹2,399/seat/mo (~$25) vs. $20/mo in the US. **This affects consumer subscriptions only — Claude API/developer pricing is unaffected and remains USD-denominated globally.** UPI payment support is not yet enabled (card/app-store billing only).

## 🤝 Deeper US Government Collaboration (announced June 30, 2026)

> As part of the resolution that restored Fable 5 and Mythos 5, Anthropic committed to: (1) expanded pre-release government access and evaluation for models that materially advance the capability frontier; (2) rapid information sharing on safeguards and jailbreaks; (3) dedicated resources for joint AI-security research with the government; and (4) work toward a common, voluntary industry security/evaluation standard. The Life Sciences Verification Program for Mythos 5.1 was also developed in partnership with the US government (see LSVP beta launch above).

## 🆕 Threat Intelligence Report *(September 10, 2026 — non-pricing)*

> Anthropic published "Detecting and countering misuse of AI: September 2026," sharing case studies from Threat Intelligence team operations disrupting attempted malicious use of Claude over the prior eight months, and describing how misuse patterns have evolved since 2025's reports. This is a **safety/policy publication with no pricing or model-lineup impact** — no new models, retirements, or price changes were announced alongside it.

## 🆕 Claude/Chat and Cowork Merge *(Product change — announced September 16, 2026)*

> **September 16, 2026:** Anthropic announced that Cowork and regular Claude chat are merging into a single unified Claude experience, rolling out to Pro and Max plans first, with Team and Free to follow. This is a **product/UX consolidation, not a pricing change** — billed at the standard rate of whichever underlying model is selected.

## 🆕 R&D Automation Index *(Research disclosure — September 17, 2026, non-pricing)*

> Anthropic published a prototype "R&D Automation Index," reporting that Claude now **leads 26% of Anthropic's own AI research and development work** as of August 2026 (up from under 1% in February 2026), with more than 90% of R&D work happening at the "collaborates" level or above and none fully autonomous. This is a **research/transparency disclosure with no pricing or model-lineup impact**.

---

## 📰 September 21, 2026 Refresh — No Pricing Changes; New Non-Pricing Announcements

> ✅ Independently re-checked the live `platform.claude.com/docs/en/about-claude/pricing` and `claude.com/pricing` pages. **Every active and legacy model price remains byte-for-byte unchanged** since the September 14 refresh — Fable 5.1, Mythos 5.1, Fable 5, Mythos 5, Opus 5, Opus 4.8, Sonnet 5 ($2/$10 permanent), Sonnet 4.6, Haiku 4.5, and the full legacy/retired table all confirmed identical. Checked `anthropic.com/news` through September 21, 2026 and found three new non-pricing items (all documented above):
> - **Sep 18, 2026** — Embedded evaluation partnership with Accenture ($1B+ commitment; governance, not pricing).
> - **Sep 17, 2026** — Life Sciences Verification Program (LSVP) opened in beta (access/safeguard program for Mythos/Opus/Sonnet, not a new priced model).
> - **Sep 17, 2026** — R&D Automation Index research disclosure (26% of Anthropic's own R&D now "led" by Claude; no pricing impact).
> - **Sep 16, 2026** — Cowork and chat merging into one unified Claude experience (product/UX change, no pricing impact).
>
> **No new Claude model releases, retirements, or price changes found this cycle.**

---

## 📰 September 14, 2026 Refresh — No Pricing Changes; Confirmed Unchanged

> ✅ Independently re-fetched the live `platform.claude.com/docs/en/about-claude/pricing` and `claude.com/pricing` pages in full. **Every active model price** (Fable 5.1, Mythos 5.1, Fable 5, Mythos 5, Opus 5, Opus 4.8, Sonnet 5, Sonnet 4.6, Haiku 4.5) and the **entire legacy/retired table** (down to Opus 4.1, Opus 4, Sonnet 4, Haiku 3.5) matched byte-for-byte against the September 7 refresh — no price changes, no new model releases, no retirements this cycle. Checked `anthropic.com/news` through September 10, 2026:
> - **Sep 10, 2026** — "Detecting and countering misuse of AI: September 2026" (Threat Intelligence report; no pricing impact — see dedicated section above).
> - **Sep 1, 2026** — Fable 5.1/Mythos 5.1 launch; "Developing Enterprise Frontier Safeguards with our customers" (already documented in the September 7 refresh).
>
> **No new Claude model releases, retirements, or price changes found this cycle.**

---

## 📰 September 7, 2026 Refresh — Fable 5.1 / Mythos 5.1 Launch, Sonnet 5 Pricing Confirmed Permanent

> ✅ Independently re-fetched the live `platform.claude.com/docs/en/about-claude/pricing` page in full. **Major update this cycle:** Claude Fable 5.1 and Claude Mythos 5.1 launched September 1, 2026, replacing Fable 5 / Mythos 5 as Anthropic's most advanced models (same $10/$50 base price, but cache-read pricing cut 75% to $0.25/MTok — an estimated 25–45% reduction in typical/agentic workload cost). Claude Sonnet 5's introductory $2/$10 pricing was also confirmed **permanent** — the scheduled Sept 1 increase to $3/$15 will not happen. New tool pricing documented: `computer_toolset_20260801` (~4,500 tokens) and a brand-new **Browser use tool** (`browser_toolset_20260801`, ~6,600 tokens). Checked `anthropic.com/news` through September 1, 2026:
> - **Sep 1, 2026** — Fable 5.1/Mythos 5.1 launch; "Developing Enterprise Frontier Safeguards with our customers" (EFS data-governance program).
> - **Aug 31, 2026** — "Improving our alignment and security efforts" (safety research post; no pricing impact).
> - **Aug 27, 2026** — "Previewing the Model Hardware Standard" (research preview allowing Claude to safely operate lab equipment; not a priced product) and "Expanding our support for scientists" (AI for Science program credits; not a pricing change).
> - **Aug 25, 2026** — "Funding better evaluations of AI's impact on wellbeing" (research grants; no pricing impact).
> - **Aug 14, 2026** — "How Claude's text watermark works" (EU AI Act compliance explainer; no pricing impact).
> - **Aug 7, 2026** — "Improving Fable 5's biology safeguards" (safety classifier update; no pricing impact).
> - **Aug 4, 2026** — Mariano-Florentino (Tino) Cuéllar announced as incoming Chief Global Affairs Officer (governance news; no pricing impact).
>
> **No other new Claude model releases, retirements, or price changes found this cycle** beyond Fable 5.1/Mythos 5.1 and the Sonnet 5 pricing confirmation.

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new projects. **LEGACY** = still API-accessible but in the provider's legacy section. **DEPRECATED** = still accessible, published retirement date. **RETIRED** = API calls return errors ❌. **🔄 REPLACED** = superseded by a newer flagship but still fully active/priced.

---

### 🔄 REPLACED — Claude Fable 5 *(Superseded by Fable 5.1, Sept 1, 2026 — still active)*

| Field | Value |
|---|---|
| **Status** | 🔄 REPLACED by Claude Fable 5.1 — still fully active and priced identically apart from cache-read rate |
| **Pricing** | $10.00 / MTok input · $50.00 / MTok output · $1.00/MTok cache read (not discounted) |
| **Migration** | → **Claude Fable 5.1** (`claude-fable-5-1`) — same headline price, ~25–45% cheaper in practice via discounted cache reads |

---

### 🔄 REPLACED — Claude Mythos 5 *(Superseded by Mythos 5.1, Sept 1, 2026 — still active for approved orgs)*

| Field | Value |
|---|---|
| **Status** | 🔄 REPLACED by Claude Mythos 5.1 — still active for previously approved Project Glasswing organizations |
| **Pricing** | $10.00 / MTok input · $50.00 / MTok output |
| **Migration** | → **Claude Mythos 5.1** (`claude-mythos-5-1`) via CVP / LSVP |

---

### ⚠️ LEGACY — Claude Mythos Preview *(Superseded by Mythos 5)*

| Field | Value |
|---|---|
| **Status** | ⚠️ LEGACY — Superseded by Claude Mythos 5 (June 9, 2026), itself now replaced by Mythos 5.1; still marked deprecated with no published retirement date |
| **Last-known Pricing** | $25.00 / MTok input · $125.00 / MTok output |
| **Migration** | → **Claude Mythos 5.1** |

---

### ⚠️ LEGACY — Claude Opus 4.7 *(Fast Mode ❌ REMOVED July 24, 2026)*

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
| **Status** | ⚠️ LEGACY — 1M context beta RETIRED April 30, 2026; max context now 200K. Still listed on the live model-pricing table |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Migration** | → **Claude Sonnet 5** ($2/$10, now permanent) or **Claude Sonnet 4.6** |

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

### ⚠️ LEGACY — Claude Opus 4.1 *(retired, except Bedrock/Google Cloud — RETIRED Aug 5, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-1` |
| **Status** | ⚠️ LEGACY — retired on the Claude API (August 5, 2026) except via Bedrock and Google Cloud, per live pricing page |
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
| Claude 3 Opus | ⚠️ RETIRED January 2026 | → Claude Opus 5 or 4.8 |
| Claude 3.5 Sonnet (v1 & v2) | ⚠️ RETIRED February 2026 | → Claude Sonnet 5 or Sonnet 4.6 |
| Claude 3 Sonnet | ⚠️ RETIRED | → Claude Sonnet 5 or Sonnet 4.6 |
| Claude 3 Haiku | ⚠️ RETIRED April 2026 | → Claude Haiku 4.5 |

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
| **🆕 Fable 5.1 cache-read discount** | Cache hits now $0.25/MTok (0.025×) vs. Fable 5's $1.00/MTok (0.1×) — ~25% cheaper for typical workloads, up to ~45% for cache-heavy agentic workloads. The single biggest lever for teams currently on Fable 5 |
| **Prompt caching — cache read (other models)** | 90% off repeated input tokens (0.1× multiplier) |
| **Prompt caching — cache write (5-min TTL)** | 1.25× standard input (break-even after 2 reads) |
| **Prompt caching — cache write (1-hr TTL)** | 2× standard input (break-even after 8 reads) |
| **✅ Sonnet 5 pricing now permanent** | $2/$10 per MTok confirmed permanent Sept 1, 2026 — the scheduled $3/$15 increase was cancelled. Sonnet 5 is now cheaper *and* more capable than Sonnet 4.6 ($3/$15) |
| **Opus 5 replaces Opus 4.8** | Same $5/$25 price, more capability. Default reason to migrate off Opus 4.8 for new projects |
| **Opus 5 has the cheapest tool-use overhead** | 286/406 tokens (auto/none — any/tool) vs. 290/410 for Opus 4.8 |
| **Fable 5.1 / Mythos 5.1** | $10/$50 base — 2× Opus 5/Opus 4.8, but now cheaper in practice than Fable 5 due to cache-read pricing. Safety-flagged queries auto-route to Opus 4.8/Opus 5 and bill at that model's rates |
| **Opus 5 / Opus 4.8 Fast Mode** | Both run Fast Mode at $10/$50 (2× standard); Opus 4.7/4.6 Fast Mode removed |
| **US-only inference (data residency)** | 1.1× pricing on Opus 4.6+, Sonnet 4.6+, Sonnet 5, and Fable 5.1/Mythos 5.1 |
| **Thinking modes** | Adaptive: Fable 5.1, Mythos 5.1, Opus 5, Opus 4.8, Sonnet 5, Sonnet 4.6. Extended: Sonnet 4.6, Haiku 4.5 (**not** on Sonnet 5/Opus 5/Fable 5.1/Mythos 5.1) |
| **Tokenizer note** | Fable 5/5.1, Mythos 5/5.1, Opus 4.7+, and Sonnet 5 use a newer tokenizer producing ~30% more tokens for the same text vs. Sonnet 4.6-and-earlier |
| **⚠️ Sonnet 4 + Opus 4 RETIRED** | Retired June 15, 2026 ❌ on Claude API — Sonnet 4 → Sonnet 5/4.6, Opus 4 → Opus 5/4.8 |
| **⚠️ Opus 4.1 RETIRED** | Retired August 5, 2026 on the Claude API (still on Bedrock/Google Cloud) — migrate to Opus 5 or 4.8 |
| **🆕 Enterprise Frontier Safeguards (EFS)** | Rolling out in phases starting fall 2026 — zero-data-retention-equivalent privacy on customer-controlled cloud infrastructure. Eligible customers can use Fable 5.1/Fable 5 with ZDR now, ahead of full EFS availability |
| **🆕 Life Sciences Verification Program (LSVP)** | Opened in beta Sept 17, 2026 — gives verified life-science teams more permissive safeguards on Mythos/Opus/Sonnet; billed at standard rates, not a separate SKU |
| **Code execution + web search/fetch combo** | Free code execution when paired with `web_search_20260209`+/`web_fetch_20260209`+ — otherwise $0.05/hr per container after 1,550 free org-hours/month (~50/day) |
| **Browser use tool** | `browser_toolset_20260801` — ~6,600 tokens overhead — priced as ordinary tool-use tokens, no separate line item |
| **Claude Managed Agents** | $0.08/session-hour runtime (billed only while `running`) + standard token rates — no Batch discount or partner-cloud pricing applies |

---

*Sources last verified: September 21, 2026 against `platform.claude.com/docs/en/about-claude/pricing`, `claude.com/pricing`, and `anthropic.com/news` (through September 21, 2026). **This cycle:** independently re-verified every active and legacy model price — all confirmed byte-for-byte unchanged since the September 14 refresh. Three new non-pricing items were found: the Life Sciences Verification Program (LSVP) opened in beta (Sept 17), an embedded-evaluation partnership with Accenture worth $1B+ over five years (Sept 18), a Claude R&D Automation Index research disclosure (Sept 17), and the Cowork/chat product merge (Sept 16). No new model releases, retirements, or price changes this cycle.*
