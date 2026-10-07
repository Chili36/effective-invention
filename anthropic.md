# 🟠 Anthropic — Claude Model Cards

> **Last updated:** 2026-10-07
> **Source:** https://www.anthropic.com/pricing · https://claude.com/pricing · https://platform.claude.com/docs/en/about-claude/models/overview · https://platform.claude.com/docs/en/about-claude/pricing · https://platform.claude.com/docs/en/models/haiku-5-5/overview · https://www.anthropic.com/claude-haiku-5-5 · https://www.anthropic.com/news/claude-sonnet-5-5 · https://www.anthropic.com/claude-opus-5-5 · https://www.anthropic.com/claude-fable-and-mythos-5-1 · https://www.anthropic.com/news · https://endoflife.date/claude
> **Scraped / verified:** 2026-10-07 — ✅ Re-fetched `platform.claude.com/docs/en/about-claude/pricing`, the new `platform.claude.com/docs/en/models/haiku-5-5/overview` model page, and `anthropic.com/news` directly. 🆕 **October 7, 2026 — Claude Haiku 5.5 launched**, Anthropic's "fastest, cheapest, and most capable small model yet," built for high-volume, latency-sensitive work (classification, extraction, routing, subagents). It carries Anthropic's first **tiered small-model pricing**: $0.10/$0.50 per MTok for prompts up to 100,000 tokens, rising to $0.50/$2.50 per MTok beyond that — a genuine **1,000,000-token context window** (4× Haiku 4.5's 200K) with 128K max output. Claude Haiku 4.5 is now 🔄 **REPLACED** (still fully active, no retirement date published yet). 🆕 **October 6, 2026 — Anthropic expanded the Cyber Verification Program**, opening reduced-blocking cybersecurity access to ~150 more vetted security organizations (non-pricing). ✅ **Re-confirmed:** Claude Sonnet 5.5 remains Anthropic's primary Sonnet-tier model at unchanged pricing ($2/$10 per MTok), and Claude Sonnet 4.5's tentative **November 30, 2026** retirement on the Claude API is unchanged. All other active and legacy model prices re-confirmed unchanged against the official pricing table.

All prices are **USD per million tokens (MTok)**. Batch API gives a flat **50% discount** on all models. Prompt caching gives up to **90% off** on repeated input context (up to **99% off** on Claude Haiku 5.5 cache reads for prompts ≤100K tokens, **97.5% off** on Fable 5.1 / Mythos 5.1 cache reads, and **95% off** on Opus 5.5 cache reads — see below). Claude Sonnet 5.5 uses the standard 0.1× cache-read multiplier ($0.20/MTok), not the deeper Fable/Opus 5.5/Haiku 5.5 discounts.

> 🆕 **October 7, 2026 — Claude Haiku 5.5 launched.** Anthropic's fourth and final member of the "Claude 5.5" family (`claude-haiku-5-5`), released on the Claude API, Amazon Bedrock, Google Cloud, Microsoft Foundry, and Claude Platform on AWS. Built for high-volume, latency-sensitive tasks — classification, routing, extraction, and subagent work. It supports adaptive thinking (default effort `medium`), a full 1,000,000-token context window, and up to 128K output tokens (300K on the Batch API with the `output-300k-2026-03-24` beta header). It uses the same newer tokenizer as Claude 4.7-and-later models, so identical text counts as ~30% more tokens than on Haiku 4.5. Thinking blocks are account-bound, like Sonnet 5.5/Opus 5.5. Reliable knowledge cutoff: June 2026. Retirement floor: not sooner than October 7, 2027.
>
> 🆕 **September 28, 2026 — Claude Sonnet 5.5 launched.** The second model in Anthropic's "Claude 5.5" family, released `claude-sonnet-5-5` on the Claude API, Amazon Bedrock, Google Cloud, and Microsoft Foundry. Anthropic describes it as "a faster, lower-cost complement to Claude Opus 5.5," strongest at well-scoped everyday tasks, bug fixes, and polished documents/slides/spreadsheets, with "a sharp eye for design." It is the first Sonnet-tier model to carry real-time cybersecurity safeguards, with Anthropic describing its cyber capability as comparable to Claude Opus 5.
>
> - **Pricing:** Unchanged from Sonnet 5 — $2.00 input / $10.00 output per MTok · Cache write (5 min): $2.50/MTok · Cache write (1 hr): $4.00/MTok · Cache read (hit): $0.20/MTok (standard 0.1× multiplier). Batch: $1.00 input / $5.00 output (50% off).
> - **Specs:** 1,000,000-token context window · 128,000 max output tokens · adaptive thinking on by default · tool-use system prompt overhead (`auto`/`none`): 286 tokens — down from Sonnet 5's 354 tokens, matching Opus 5.5.
> - **Performance:** Anthropic says it runs 30%+ faster than Sonnet 5 and costs up to 30% less for most work (via fewer tokens per task, not a price cut) — and that it is the first Sonnet model to beat Pokémon Red from screenshots alone, which Anthropic cites as evidence of long-horizon agentic and image-understanding gains. Anthropic's own benchmarks show Sonnet 5.5 on Terminal-Bench 4.0 at **70.6%**, ahead of both Sonnet 5 (10.3%) and Opus 5.5 (66.4%); on GDPval-AA it scores 1844 vs. Opus 5.5's 1846 — Anthropic says Opus 5.5 remains clearly stronger on complex, open-ended work.
> - **Safety / migration notes:** Thinking blocks Sonnet 5.5 produces now work only in the account that produced them (or a linked account) — an anti-distillation measure Anthropic says is meant "to curb distillation attacks via account-switching." Migrating from Sonnet 5 is not a drop-in swap: forced tool choice (`tool_choice: any`/`tool`) behavior and effort-level calibration both change.
> - **Availability:** Claude API (`claude-sonnet-5-5`), Claude.ai, Claude Code, Claude Cowork, Amazon Bedrock, Google Cloud, Microsoft Foundry.
> - **Notable:** Claude Sonnet 5 is now the 🔄 **replaced** (but still active) prior-generation Sonnet. Claude Haiku 5.5 remains the only unreleased member of the Claude 5.5 family, still "in the coming weeks" per Anthropic with no ID, price, or context window published.
>
> 🆕 **September 30, 2026 — Claude Sonnet 4.5 deprecated; retires November 30, 2026.** Anthropic notified developers that `claude-sonnet-4-5-20250929` is deprecated on the Claude API, with a tentative retirement date of **November 30, 2026** (61 days' notice, one day above Anthropic's own 60-day minimum-notice floor) and `claude-sonnet-5-5` as the recommended replacement. The dates apply to Anthropic-operated platforms only — Amazon Bedrock and Google Cloud set their own retirement schedules for Sonnet 4.5.
>
> 🆕 **September 22, 2026 — Claude Opus 5.5 launched.** The first model in Anthropic's new "Claude 5.5" family. Anthropic says it performs at the level of Claude Fable 5.1 on most work and costs 40% less to run than Opus 5 on typical workloads, thanks to lower per-token pricing plus using fewer tokens per task. It scored the best of any Claude model to date on Anthropic's automated behavioral audit (its primary alignment suite) and was evaluated pre-release by METR and Frontier Design.
>
> - **Pricing:** $4.00 input / $20.00 output per MTok (20% cheaper than Opus 5's $5/$25) · Cache write (5 min): $5.00/MTok · Cache write (1 hr): $8.00/MTok · **Cache read (hit): $0.20/MTok — a 0.05× multiplier, 60% cheaper than Opus 5's $0.50/MTok (0.1×)**. Batch: $2.00 input / $10.00 output. Fast Mode: $8.00 input / $40.00 output (up to 2.5× speed).
> - **Specs:** 1,000,000-token context window · 128,000 max output tokens · reliable knowledge cutoff June 2026 · thinking is **adaptive only and can no longer be disabled** (unlike Opus 5) · default reasoning effort `medium` · tool-use system prompt overhead (`auto`/`none`): 286 tokens, identical to Opus 5.
> - **Safety:** First Opus model to launch with Fable-5.1-class safeguards on cybersecurity, biology, and anti-distillation (preserved thinking) — most cybersecurity tasks re-route to Claude Opus 4.8; advanced biology work requires the Life Sciences Verification Program. Available with zero data retention, like previous Opus models.
> - **Benchmarks (Anthropic's own):** Terminal-Bench 4.0 66.4% (vs. Fable 5.1's 55.8%, Opus 5's 52.3%, GPT-6 Astra's 57.9%); beats GPT-6 Astra on FrontierCode at ~20% of the cost per task; matches GPT-6 Astra on Terminal-Bench 4.0 at ~40% of the cost.
> - **Availability:** Claude API/Platform (`claude-opus-5-5`), Claude.ai, Claude Code, Claude Cowork, Amazon Web Services, Google Cloud, Microsoft Azure.
>
> 🆕 **September 1, 2026 — Claude Fable 5.1 and Claude Mythos 5.1 launched.** Anthropic's most-advanced models for coding and knowledge work; same underlying model, different safeguard levels. Headline price unchanged at $10/$50 per MTok, but cache-read pricing drops 75% to **$0.25/MTok (0.025×)** — Anthropic estimates this cuts typical workload costs by ~25% and highly agentic workload costs by up to ~45%. Model ID: `claude-fable-5-1`.
>
> ✅ **September 1, 2026 — Claude Sonnet 5's $2/$10 pricing is now PERMANENT.** The scheduled increase to $3/$15 did not occur.
>
> ✅ **Claude Sonnet 4 + Opus 4 RETIRED on June 15, 2026. ❌** API calls to `claude-sonnet-4-20250514` and `claude-opus-4-20250514` now return errors (except via Amazon Bedrock and Google Cloud). Migration: Sonnet 4 → Sonnet 5.5; Opus 4 → Opus 5.5 or Opus 4.8.

---

## ✅ Active / Recommended Models

### 🆕 Claude Opus 5.5 *(Released September 22, 2026 — New Recommended Default Model)*

> The first model in Anthropic's new "Claude 5.5" family. Performs at roughly Claude Fable 5.1's level on most work, at 40% lower cost than Opus 5. Now Anthropic's recommended default in place of Opus 5, which drops out of the primary "Compare models" grid (though it remains fully active).

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-5-5` |
| **Released** | September 22, 2026 |
| **Status** | ✅ Active — **New recommended default model; replaces Opus 5** |
| **Input price** | $4.00 / MTok *(20% cheaper than Opus 5's $5.00)* |
| **Output price** | $20.00 / MTok *(20% cheaper than Opus 5's $25.00)* |
| **Cache write (5 min)** | $5.00 / MTok |
| **Cache write (1 hr)** | $8.00 / MTok |
| **Cache read (cache hit)** | 📉 **$0.20 / MTok** *(0.05× multiplier — 60% cheaper than Opus 5's $0.50/MTok 0.1× rate)* |
| **Batch input** | $2.00 / MTok |
| **Batch output** | $10.00 / MTok |
| **Fast Mode** | $8.00 input / $40.00 output per MTok — up to 2.5× standard speed |
| **Context window** | 1,000,000 tokens |
| **Max output** | 128,000 tokens |
| **Reliable knowledge cutoff** | June 2026 |
| **Thinking mode** | Adaptive — always on; **can no longer be disabled** (unlike Opus 5) |
| **Default reasoning effort** | `medium` |
| **Tool-use system prompt (`auto`/`none`)** | 286 tokens *(identical to Opus 5; `any`/`tool` figure not yet separately published)* |
| **Availability** | Claude API/Platform (`claude-opus-5-5`) · Claude.ai · Claude Code · Claude Cowork · Amazon Web Services · Google Cloud · Microsoft Azure |
| **Data retention** | Zero data retention available, as with previous Opus models |
| **Safety** | Fable-5.1-class safeguards on cybersecurity/biology; most cybersecurity tasks transparently fall back to Claude Opus 4.8; advanced biology work requires the Life Sciences Verification Program; first Opus model with "preserved thinking" anti-distillation protection |
| **Notable** | Beats GPT-6 Astra on FrontierCode at ~20% of the cost per task; matches GPT-6 Astra on Terminal-Bench 4.0 (66.4%) at ~40% of the cost; ~85% fewer containment-boundary-circumvention attempts than Opus 5/Mythos 5.1 on Anthropic's alignment eval; output >30% faster than Opus 5 |

> 🔜 **Claude Haiku 5.5** is confirmed to be following "in the coming weeks," rounding out the Claude 5.5 family. **Still not released as of October 5, 2026 — no model ID, pricing, context window, or benchmark published.** Claude Haiku 4.5's own retirement floor ("not sooner than October 15, 2026") is now about 10 days away with no successor yet announced.

---

### 🆕 Claude Sonnet 5.5 *(Released September 28, 2026 — The Best Combination of Speed and Intelligence)*

> The second model in Anthropic's "Claude 5.5" family, arriving six days after Opus 5.5. A faster, lower-cost complement to Opus 5.5: strongest at well-scoped everyday tasks, bug fixes, and polished documents/slides/spreadsheets. Replaces Claude Sonnet 5 as Anthropic's primary Sonnet-tier model.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-5-5` |
| **Released** | September 28, 2026, 18:03 UTC |
| **Status** | ✅ Active — **Primary Sonnet-tier model; replaces Sonnet 5** |
| **Input price** | $2.00 / MTok *(unchanged from Sonnet 5)* |
| **Output price** | $10.00 / MTok *(unchanged from Sonnet 5)* |
| **Cache write (5 min)** | $2.50 / MTok |
| **Cache write (1 hr)** | $4.00 / MTok |
| **Cache read (cache hit)** | $0.20 / MTok *(standard 0.1× multiplier — not discounted like Fable 5.1/Opus 5.5)* |
| **Batch input** | $1.00 / MTok *(50% off)* |
| **Batch output** | $5.00 / MTok *(50% off)* |
| **Context window** | 1,000,000 tokens |
| **Max output** | 128,000 tokens |
| **Thinking mode** | Adaptive — on by default |
| **Tool-use system prompt (`auto`/`none`)** | 286 tokens *(down from Sonnet 5's 354 tokens; `any`/`tool` figure not yet separately published)* |
| **Availability** | Claude API (`claude-sonnet-5-5`) · Claude.ai · Claude Code · Claude Cowork · Amazon Bedrock · Google Cloud · Microsoft Foundry |
| **Benchmarks (Anthropic's own)** | Terminal-Bench 4.0: **70.6%** (vs. Sonnet 5's 10.3%, Opus 5.5's 66.4%) · GDPval-AA: 1844 (Opus 5.5: 1846) |
| **Safety** | First Sonnet-tier model with real-time cybersecurity safeguards, with cyber capability Anthropic describes as comparable to Claude Opus 5; thinking blocks are now account-bound (usable only in the account that produced them, or a linked account) to curb distillation attacks via account-switching |
| **Notable** | Anthropic says it runs 30%+ faster than Sonnet 5 and costs up to 30% less for most work (via token efficiency, not a price cut); first Sonnet model to beat Pokémon Red from screenshots alone; Anthropic's own benchmarks show it beating Opus 5.5 on agentic coding. Migrating from Sonnet 5 is **not a drop-in swap** — forced tool-choice behavior and effort-level calibration both change. |

---

### 🆕 Claude Fable 5.1 *(Released September 1, 2026 — Most Advanced Model for Coding & Knowledge Work)*

> Fable 5.1 and Mythos 5.1 are the same underlying model, differing only in safeguard configuration. Anthropic recommends Fable 5.1 specifically for "demanding reasoning and long-horizon agentic work," reserving Opus 5.5 as the default for most other workloads.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-fable-5-1` |
| **Released** | September 1, 2026 |
| **Status** | ✅ Active — **Recommended for demanding reasoning & long-horizon agentic work** |
| **Input price** | $10.00 / MTok |
| **Output price** | $50.00 / MTok |
| **Cache write (5 min)** | $12.50 / MTok |
| **Cache write (1 hr)** | $20.00 / MTok |
| **Cache read (cache hit)** | 📉 **$0.25 / MTok** *(0.025× multiplier — cheapest cache-read rate of any Anthropic model)* |
| **Batch input** | $5.00 / MTok *(50% off)* |
| **Batch output** | $25.00 / MTok *(50% off)* |
| **US-only inference** | 1.1× pricing |
| **Context window** | 1,000,000 tokens (standard pricing — no long-context surcharge) |
| **Max output** | 128,000 tokens |
| **Thinking mode** | Adaptive only — always on; defaults to High effort in Claude Code, Medium in Claude Cowork/Claude.ai |
| **Tokenizer** | Newer tokenizer — ~30% more tokens for the same text vs. Sonnet 4.6-and-earlier |
| **Availability** | Claude API (`claude-fable-5-1`) · Claude.ai · Claude Code · Claude Cowork · Amazon Web Services · Google Cloud · Microsoft Azure |
| **Data retention** | Enterprise Frontier Safeguards (EFS) rolling out from fall 2026; eligible customers can use Fable 5.1 with zero data retention today |
| **Notable** | Estimated ~25% cheaper for typical workloads and up to ~45% cheaper for highly agentic workloads vs. Fable 5, purely from the cache-read price cut |

---

### 🔒 Claude Mythos 5.1 *(Trusted Access — Released September 1, 2026)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-mythos-5-1` |
| **Released** | September 1, 2026 |
| **Status** | 🔒 Trusted access only — replaces Mythos 5 |
| **Pricing** | $10.00 / MTok input · $50.00 / MTok output (identical to Fable 5.1, including the $0.25/MTok cache-read rate) |
| **Context window** | 1,000,000 tokens · Max output: 128,000 tokens |
| **Access** | Cyber Verification Program (CVP) and Life Sciences Verification Program (LSVP) |
| **Notable** | Now also powers Claude Security. Opus 5.5 is now "comparable to Mythos 5.1" in biology and cybersecurity per Anthropic, narrowing Mythos 5.1's unique-capability advantage |

---

### Claude Fable 5 *(🔄 Replaced by Fable 5.1 — still active)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-fable-5` |
| **Released** | June 9, 2026 · Suspended June 12–30, 2026 · Restored July 1, 2026 |
| **Status** | ✅ Active — 🔄 Replaced by Fable 5.1 as flagship (September 1, 2026) |
| **Input price** | $10.00 / MTok |
| **Output price** | $50.00 / MTok |
| **Cache write (5 min)** | $12.50 / MTok |
| **Cache write (1 hr)** | $20.00 / MTok |
| **Cache read** | $1.00 / MTok *(older 0.1× rate — not discounted to Fable 5.1's $0.25/MTok)* |
| **Batch input** | $5.00 / MTok *(50% off)* |
| **Batch output** | $25.00 / MTok *(50% off)* |
| **Context window** | 1,000,000 tokens |
| **Max output** | 128,000 tokens |
| **Availability** | Claude API · Claude.ai · Claude Code · Claude Cowork · Claude Platform on AWS · Amazon Bedrock · Google Vertex AI · Microsoft Foundry |

---

### 🔒 Claude Mythos 5 *(🔄 Replaced by Mythos 5.1 — still active for approved orgs)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-mythos-5` |
| **Status** | 🔒 Restricted — 🔄 Replaced by Mythos 5.1; still active for previously approved Project Glasswing organizations |
| **Pricing** | $10.00 / MTok input · $50.00 / MTok output (cache read at older $1.00/MTok rate) |
| **Context window** | 1,000,000 tokens · Max output: 128,000 tokens |

---

### Claude Opus 5 *(🔄 Replaced by Opus 5.5 — still active)*

> Claude Opus 5.5 has replaced Opus 5 as Anthropic's recommended default model, at 20% lower token pricing and 60% lower cache-read pricing. Opus 5 remains fully API-accessible and is not deprecated — it also continues to serve as the automatic safety-fallback target when Opus 5.5's cybersecurity classifiers flag a request.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-5` |
| **Released** | July 24, 2026 |
| **Status** | ✅ Active — 🔄 Replaced by Opus 5.5 as leading model (September 22, 2026); still the safety-fallback target for Opus 5.5 and Fable 5.1 |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok *(standard 0.1× multiplier)* |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Fast Mode** | ~2.5× standard speed at 2× base price ($10.00/$50.00 per MTok) |
| **Context window** | 1,000,000 tokens |
| **Tool-use system prompt (`auto`/`none` — `any`/`tool`)** | 286 tokens — 406 tokens |
| **Availability** | Claude API (`claude-opus-5`) · Claude.ai · Claude Code · Amazon Bedrock · Claude Platform on AWS · Google Cloud · Microsoft Foundry |

---

### Claude Opus 4.8 *(🔄 Replaced by Opus 5, then Opus 5.5 — still active)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-opus-4-8` |
| **Status** | ✅ Active — 🔄 Replaced by Opus 5.5; still the safety-fallback target for Fable 5.1 and Opus 5.5's cybersecurity safeguards |
| **Input price** | $5.00 / MTok |
| **Output price** | $25.00 / MTok |
| **Fast Mode (input/output)** | $10.00 / MTok / $50.00 / MTok *(2× standard)* |
| **Cache write (5 min)** | $6.25 / MTok |
| **Cache write (1 hr)** | $10.00 / MTok |
| **Cache read** | $0.50 / MTok |
| **Batch input** | $2.50 / MTok |
| **Batch output** | $12.50 / MTok |
| **Context window** | 1,000,000 tokens (standard API) · 200,000 tokens (Microsoft Foundry only) |
| **Max output** | 128,000 tokens (sync) / 300,000 tokens (Batch API with beta header) |
| **Availability** | Claude API · Claude Platform on AWS · Amazon Bedrock (Messages API) · Google Vertex AI · Microsoft Foundry (200k ctx) |

---

### Claude Sonnet 5 *(🔄 Replaced by Sonnet 5.5 — still active; pricing permanent since Sept 1, 2026)*

> Claude Sonnet 5.5 has replaced Sonnet 5 as Anthropic's primary Sonnet-tier model at identical pricing with significant speed and benchmark gains. Sonnet 5 remains fully API-accessible with no retirement date yet.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-5` |
| **Released** | June 30, 2026 |
| **Status** | ✅ Active — 🔄 Replaced by Sonnet 5.5 as the primary Sonnet-tier model (Sept 28, 2026); not sooner than June 30, 2027 retirement floor |
| **Input price** | **$2.00 / MTok** *(permanent, not introductory)* |
| **Output price** | **$10.00 / MTok** *(permanent, not introductory)* |
| **Cache write (5 min)** | $2.50 / MTok |
| **Cache write (1 hr)** | $4.00 / MTok |
| **Cache read** | $0.20 / MTok |
| **Batch input** | $1.00 / MTok |
| **Batch output** | $5.00 / MTok |
| **Context window** | 1,000,000 tokens (at standard pricing — no surcharge) |
| **Max output** | 128,000 tokens (sync) / 300,000 tokens (Batch API with beta header) |
| **Reliable knowledge cutoff** | January 2026 |
| **Thinking mode** | Adaptive (default effort `high`) |
| **Tool-use system prompt (`auto`/`none` — `any`/`tool`)** | 354 tokens — 474 tokens |
| **Availability** | Claude API · Claude.ai (Free/Pro/Max/Team/Enterprise) · Claude Code · Claude Platform on AWS · Amazon Bedrock · Google Cloud · Microsoft Foundry |

---

### Claude Sonnet 4.6 *(🔄 Replaced by Sonnet 5 as default — still active)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-4-6` |
| **Released** | February 17, 2026 |
| **Status** | ✅ Active — 🔄 Replaced by Sonnet 5 as default; now the more expensive of the two |
| **Input price** | $3.00 / MTok |
| **Output price** | $15.00 / MTok |
| **Cache write (5 min)** | $3.75 / MTok |
| **Cache write (1 hr)** | $6.00 / MTok |
| **Cache read** | $0.30 / MTok |
| **Batch input** | $1.50 / MTok |
| **Batch output** | $7.50 / MTok |
| **Context window** | 1,000,000 tokens |
| **Max output** | 64,000 tokens (sync) / 300,000 tokens (Batch API with beta header) |
| **Extended thinking** | ✅ Yes |
| **Availability** | API · AWS Bedrock · Google Vertex AI · Microsoft Foundry |

---

### 🆕 Claude Haiku 5.5 *(Released October 7, 2026 — Fastest, Cheapest, Most Capable Small Model)*

> Anthropic's fourth and final "Claude 5.5" family member. Built for high-volume, latency-sensitive tasks such as classification, extraction, routing, and subagent work. Replaces Claude Haiku 4.5 as Anthropic's small-model recommendation, with a 5× larger context window and Anthropic's first tiered small-model pricing.

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-haiku-5-5` |
| **Released** | October 7, 2026 |
| **Status** | ✅ Active (latest) — **Replaces Haiku 4.5** |
| **Input price (prompts ≤100K tokens)** | $0.10 / MTok |
| **Input price (prompts >100K tokens)** | $0.50 / MTok |
| **Output price (prompts ≤100K tokens)** | $0.50 / MTok |
| **Output price (prompts >100K tokens)** | $2.50 / MTok |
| **Cache write 5 min (≤100K / >100K)** | $0.125 / MTok · $0.625 / MTok |
| **Cache write 1 hr (≤100K / >100K)** | $0.20 / MTok · $1.00 / MTok |
| **Cache read / hit (≤100K / >100K)** | 📉 **$0.01 / MTok · $0.05 / MTok** *(0.1× multiplier — cheapest absolute cache-read rate of any Claude model)* |
| **Batch input (≤100K / >100K)** | $0.05 / MTok · $0.25 / MTok *(50% off)* |
| **Batch output (≤100K / >100K)** | $0.25 / MTok · $1.25 / MTok *(50% off)* |
| **Context window** | 📈 **1,000,000 tokens** *(5× Haiku 4.5's 200K)* |
| **Max output** | 128,000 tokens (sync) / 300,000 tokens (Batch API, `output-300k-2026-03-24` beta header) |
| **Reliable knowledge cutoff** | June 2026 |
| **Thinking mode** | Adaptive — on by default, default effort `medium` |
| **Tokenizer** | Newer tokenizer (same as Claude 4.7+) — ~30% more tokens for the same text vs. Haiku 4.5 |
| **Tool-use system prompt (`auto`/`none` — `any`/`tool`)** | 286 tokens — 406 tokens |
| **Availability** | Claude API (`claude-haiku-5-5`) · Amazon Bedrock · Google Cloud · Microsoft Foundry · Claude Platform on AWS |
| **Retirement floor** | Not sooner than October 7, 2027 |
| **Notable** | Thinking blocks are account-bound (anti-distillation), like Sonnet 5.5/Opus 5.5; Anthropic calls it "our fastest, cheapest, and most capable small model yet" |

---

### Claude Haiku 4.5 *(🔄 Replaced by Haiku 5.5 — still active)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-haiku-4-5` |
| **Released** | October 2025 |
| **Status** | ✅ Active — 🔄 Replaced by Haiku 5.5 (October 7, 2026); no retirement date published yet |
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
| **Availability** | API · AWS Bedrock (all regions) · Google Vertex AI · Microsoft Foundry |

---

## 📊 Thinking Capabilities Matrix (Active Models)

| Model | Extended Thinking | Adaptive Thinking | Notes |
|---|---|---|---|
| Claude Opus 5.5 | ❌ No | ✅ Yes (always on — cannot be disabled) | New leading model; replaces Opus 5. |
| Claude Sonnet 5.5 | ❌ No | ✅ Yes (on by default) | Replaces Sonnet 5; same price, 30%+ faster. |
| Claude Fable 5.1 | ❌ No | ✅ Yes (always on) | Defaults: High effort (Claude Code), Medium (Cowork/Claude.ai). |
| Claude Mythos 5.1 | ❌ No | ✅ Yes (always on) | 🔒 Trusted access only (CVP / LSVP). |
| Claude Opus 5 | ❌ No | ✅ Yes | 🔄 Replaced by Opus 5.5; still active. |
| Claude Opus 4.8 | ❌ No | ✅ Yes | Fast Mode at 2× pricing. |
| Claude Sonnet 5 | ❌ No | ✅ Yes | 🔄 Replaced by Sonnet 5.5; $2/$10 pricing unchanged. |
| Claude Sonnet 4.6 | ✅ Yes | ✅ Yes | Only Sonnet-tier model with Extended Thinking. |
| Claude Haiku 5.5 | ❌ No | ✅ Yes (on by default, default effort `medium`) | Replaces Haiku 4.5; 1M context, tiered pricing. |
| Claude Haiku 4.5 | ✅ Yes | ❌ No | 🔄 Replaced by Haiku 5.5; still active. |

---

## 🔧 Tools & Agents Pricing

### Server-side tools

| Tool | Pricing |
|---|---|
| **Web search** | $10 per 1,000 searches, plus standard token costs for search-generated content. |
| **Web fetch** | No additional charge — standard token costs only for fetched content. |
| **Code execution** | Free when used alongside `web_search_20260209`+ or `web_fetch_20260209`+. Otherwise 1,550 free container-hours/month per org, then $0.05/hour per container. |
| **Bash tool** | Adds 325 input tokens (Opus 4.7/4.8/5) or 244 tokens (Opus 4.6, Sonnet 4.6 and earlier). |
| **Text editor tool** | Adds 700 input tokens (Claude 4.x `text_editor_20250429`). |
| **Computer use tool** | `computer_toolset_20260801`: ~4,500 input tokens overhead. |
| **Browser use tool** | `browser_toolset_20260801`: ~6,600 input tokens overhead. |

### Tool-use system-prompt overhead (per request, when ≥1 tool is defined)

| Model | `auto`/`none` | `any`/`tool` |
|---|---|---|
| Claude Opus 5.5 | 286 tokens | *(not yet separately published)* |
| Claude Sonnet 5.5 | 286 tokens | *(not yet separately published)* |
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
| Claude Haiku 5.5 | 286 tokens | 406 tokens |
| Claude Haiku 4.5 | 496 tokens | 588 tokens |
| Claude Haiku 3.5 (retired, except Bedrock/Google Cloud) | 264 tokens | 355 tokens |

### Claude Managed Agents *(billed on tokens + session runtime)*

| SKU | Rate | Notes |
|---|---|---|
| **Session runtime** | $0.08 per session-hour | Metered to the millisecond, accrues only while session status is `running` |
| **Tokens** | Standard per-model rates | Prompt caching multipliers apply identically |
| **Not applicable** | Batch API discount, Fast Mode premium (unless `model.speed: "fast"`), cloud-platform pricing | Sessions are stateful/interactive |

---

## ⚠️ Legacy / Deprecated / Retired Models

> **LEGACY** = still API-accessible but in the provider's legacy section. **DEPRECATED** = still accessible, published retirement date. **RETIRED** = API calls return errors ❌. **🔄 REPLACED** = superseded but still fully active/priced.

### 🔄 REPLACED — Claude Opus 5 *(Superseded by Opus 5.5, Sept 22, 2026 — still active)*

| Field | Value |
|---|---|
| **Pricing** | $5.00 / MTok input · $25.00 / MTok output · $0.50/MTok cache read |
| **Migration** | → **Claude Opus 5.5** — 20% cheaper tokens, 60% cheaper cache reads |

### 🔄 REPLACED — Claude Sonnet 5 *(Superseded by Sonnet 5.5, Sept 28, 2026 — still active)*

| Field | Value |
|---|---|
| **Pricing** | $2.00 / MTok input · $10.00 / MTok output · $0.20/MTok cache read *(identical to Sonnet 5.5)* |
| **Migration** | → **Claude Sonnet 5.5** — same price, 30%+ faster, much higher Terminal-Bench score; note forced tool-choice and effort calibration change |

### 🆕 🔄 REPLACED — Claude Haiku 4.5 *(Superseded by Haiku 5.5, Oct 7, 2026 — still active)*

| Field | Value |
|---|---|
| **Pricing** | $1.00 / MTok input · $5.00 / MTok output · $0.10/MTok cache read |
| **Migration** | → **Claude Haiku 5.5** — tiered $0.10/$0.50 (≤100K tokens), 5× larger context (1M vs 200K), cheaper absolute cache-read rate ($0.01/MTok) |

### ⚠️ LEGACY — Claude Fable 5 *(Superseded by Fable 5.1)*

| Field | Value |
|---|---|
| **Pricing** | $10.00 / MTok input · $50.00 / MTok output · $1.00/MTok cache read (not discounted) |
| **Migration** | → **Claude Fable 5.1** |

### ⚠️ LEGACY — Claude Mythos 5 *(Superseded by Mythos 5.1)*

| Field | Value |
|---|---|
| **Pricing** | $10.00 / MTok input · $50.00 / MTok output |
| **Migration** | → **Claude Mythos 5.1** via CVP / LSVP |

### ⚠️ LEGACY — Claude Mythos Preview

| Field | Value |
|---|---|
| **Last-known Pricing** | $25.00 / MTok input · $125.00 / MTok output |
| **Migration** | → **Claude Mythos 5.1** |

### ⚠️ LEGACY — Claude Opus 4.7 *(Fast Mode ❌ REMOVED July 24, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-7` |
| **Input/Output price** | $5.00 / $25.00 per MTok |
| **Migration** | → **Claude Opus 5.5**, **Opus 5**, or **Opus 4.8** |

### ⚠️ LEGACY — Claude Opus 4.6 *(Fast Mode REMOVED June 29, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-6` |
| **Input/Output price** | $5.00 / $25.00 per MTok |
| **Migration** | → **Claude Opus 5.5**, **Opus 5**, or **Opus 4.8** |

### ⚠️ DEPRECATED — Claude Sonnet 4.5 *(Retires November 30, 2026 on the Claude API)*

| Field | Value |
|---|---|
| **Model ID** | `claude-sonnet-4-5-20250929` |
| **Status** | ⚠️ Deprecated September 30, 2026 — tentative retirement **November 30, 2026** on the Claude API (Bedrock/Google Cloud set their own schedules) |
| **1M context beta** | RETIRED April 30, 2026; max context now 200K |
| **Input/Output price** | $3.00 / $15.00 per MTok |
| **Migration** | → **Claude Sonnet 5.5** (`claude-sonnet-5-5`), Anthropic's recommended replacement |

### ⚠️ LEGACY — Claude Opus 4.5

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-5` |
| **Input/Output price** | $5.00 / $25.00 per MTok |
| **Context window** | 200,000 tokens |
| **Migration** | → **Claude Opus 5.5**, **Opus 5**, or **Opus 4.8** |

### ⚠️ LEGACY — Claude Opus 4.1 *(retired, except Bedrock/Google Cloud — RETIRED Aug 5, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-1` |
| **Input/Output price** | $15.00 / $75.00 per MTok |
| **Migration** | → **Claude Opus 5.5** ($4/$20) — 80% cheaper |

### ⚠️ RETIRED — Claude Sonnet 4 *(June 15, 2026 ❌ — except Bedrock/Google Cloud)*

| Field | Value |
|---|---|
| **Model ID** | `claude-sonnet-4-20250514` |
| **Input/Output price** | $3.00 / $15.00 per MTok |
| **Migration** | → **Claude Sonnet 5** or **Claude Sonnet 4.6** |

### ⚠️ RETIRED — Claude Opus 4 *(June 15, 2026 ❌ — except Google Cloud)*

| Field | Value |
|---|---|
| **Model ID** | `claude-opus-4-20250514` |
| **Input/Output price** | $15.00 / $75.00 per MTok |
| **Migration** | → **Claude Opus 5.5** ($4/$20) — 80% cheaper |

### ⚠️ LEGACY — Claude Haiku 3.5 *(RETIRED February 19, 2026 on Claude API)*

| Field | Value |
|---|---|
| **Model ID** | `claude-3-5-haiku-20241022` |
| **Input/Output price** | $0.80 / $4.00 per MTok |
| **Migration** | → **Claude Haiku 4.5** ($1/$5) |

### ⚠️ LEGACY — Claude Haiku 3 *(RETIRED February 19, 2026)*

→ **Claude Haiku 4.5** ($1/$5)

### ⚠️ LEGACY — Claude Sonnet 3.7 *(RETIRED October 28, 2025)*

→ **Claude Sonnet 5** or **Claude Sonnet 4.6**

### ⚠️ LEGACY — Claude 3 Series

| Model | Status | Migration |
|---|---|---|
| Claude 3 Opus | RETIRED January 2026 | → Claude Opus 5.5, Opus 5, or 4.8 |
| Claude 3.5 Sonnet (v1 & v2) | RETIRED February 2026 | → Claude Sonnet 5 or Sonnet 4.6 |
| Claude 3 Sonnet | RETIRED | → Claude Sonnet 5 or Sonnet 4.6 |
| Claude 3 Haiku | RETIRED April 2026 | → Claude Haiku 4.5 |

### ⚠️ LEGACY — Claude 2.x Series *(RETIRED)*

| Model | Last Known Price |
|---|---|
| Claude 2.0 / 2.1 | ~$8.00 input / $24.00 output per MTok |

---

## 💡 Cost Optimization Notes

| Feature | Savings |
|---|---|
| **🆕 Opus 5.5 is now the default recommendation** | $4/$20 per MTok, 20% cheaper than Opus 5, with a 60% cheaper cache-read rate ($0.20 vs $0.50/MTok) |
| **🆕 Sonnet 5.5 replaces Sonnet 5 at the same price** | $2/$10 per MTok, 30%+ faster, Terminal-Bench 4.0 70.6% vs Sonnet 5's 10.3% |
| **🆕 Haiku 5.5 replaces Haiku 4.5 — tiered pricing, 5× context** | $0.10/$0.50 per MTok for prompts ≤100K tokens ($0.50/$2.50 beyond); 1M-token context (vs. 200K); cheapest absolute cache-read rate of any Claude model ($0.01/MTok) |
| **Batch API** | 50% off input + output (all models, 24 hr turnaround) |
| **Fable 5.1 / Opus 5.5 / Haiku 5.5 cache-read discounts** | Fable 5.1: $0.25/MTok (0.025×); Opus 5.5: $0.20/MTok (0.05×); Haiku 5.5: $0.01/MTok (≤100K, 0.1×) — all cheaper in absolute terms than the standard rate; Sonnet 5.5 stays on the standard 0.1× rate |
| **⚠️ Sonnet 4.5 deprecated** | Retires November 30, 2026 on the Claude API — migrate to Sonnet 5.5 |
| **US-only inference (data residency)** | 1.1× pricing on Opus 4.6+, Sonnet 4.6+, Sonnet 5, Sonnet 5.5, Opus 5, Opus 5.5, Haiku 5.5, and Fable 5.1/Mythos 5.1 |
| **⚠️ Sonnet 4 + Opus 4 RETIRED** | Retired June 15, 2026 ❌ on Claude API |
| **⚠️ Opus 4.1 RETIRED** | Retired August 5, 2026 on the Claude API (still on Bedrock/Google Cloud) |
| **Claude Managed Agents** | $0.08/session-hour runtime + standard token rates |

---

*Sources last verified: October 7, 2026 against `platform.claude.com/docs/en/about-claude/pricing`, `platform.claude.com/docs/en/models/haiku-5-5/overview`, `platform.claude.com/docs/en/models/overview`, `claude.com/pricing`, and `anthropic.com/news`. **This refresh:** Claude Haiku 5.5 launched October 7, 2026 — Anthropic's fastest, cheapest, small model, with tiered $0.10/$0.50 (≤100K tokens) / $0.50/$2.50 (>100K tokens) pricing, a 1,000,000-token context window, and the cheapest absolute cache-read rate of any Claude model ($0.01/MTok ≤100K). Claude Haiku 4.5 is now 🔄 REPLACED (still fully active, no retirement date published). Also noted: October 6, 2026 Cyber Verification Program expansion (non-pricing). Re-confirmed Claude Sonnet 5.5 ($2/$10) remains the primary Sonnet-tier model and Claude Sonnet 4.5's tentative November 30, 2026 retirement on the Claude API is unchanged. All other active and legacy model prices re-confirmed unchanged against the official pricing table.*
