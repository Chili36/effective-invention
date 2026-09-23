# 🟠 Anthropic — Claude Model Cards

> **Last updated:** 2026-09-23
> **Source:** https://www.anthropic.com/pricing · https://claude.com/pricing · https://platform.claude.com/docs/en/about-claude/models/overview · https://platform.claude.com/docs/en/about-claude/pricing · https://www.anthropic.com/claude-opus-5-5 · https://www.anthropic.com/claude-fable-and-mythos-5-1 · https://www.anthropic.com/news
> **Scraped / verified:** 2026-09-23 — ✅ Independently re-checked `platform.claude.com/docs/en/about-claude/pricing`, `platform.claude.com/docs/en/models/overview`, and `anthropic.com/news` through September 23, 2026. **No new model releases, retirements, or price changes since the September 22 refresh.** Claude Opus 5.5 (launched Sept 22, 2026) remains the newest model and Anthropic's new recommended default — it replaces Claude Opus 5 at **20% cheaper tokens and 60% cheaper cache reads** ($4/$20 per MTok vs. Opus 5's $5/$25; cache reads $0.20/MTok vs. $0.50/MTok), with Anthropic estimating ~40% lower cost than Opus 5 on typical workloads. Claude Sonnet 5.5 and Haiku 5.5 remain announced as "coming in the following weeks" but are **not yet released — no pricing published**. All other active model prices (Fable 5.1, Mythos 5.1, Fable 5, Mythos 5, Opus 5, Opus 4.8, Sonnet 5 $2/$10 permanent, Sonnet 4.6, Haiku 4.5) and the full legacy table are unchanged.

All prices are **USD per million tokens (MTok)**. Batch API gives a flat **50% discount** on all models. Prompt caching gives up to **90% off** on repeated input context (up to **97.5% off** on Fable 5.1 / Mythos 5.1 cache reads, and **95% off** on Opus 5.5 cache reads — see below).

> 🆕 **September 22, 2026 — Claude Opus 5.5 launched.** The first model in Anthropic's new "Claude 5.5" family. Anthropic says it performs at the level of Claude Fable 5.1 on most work and costs 40% less to run than Opus 5 on typical workloads, thanks to lower per-token pricing plus using fewer tokens per task. It scored the best of any Claude model to date on Anthropic's automated behavioral audit (its primary alignment suite) and was evaluated pre-release by METR and Frontier Design. Claude Sonnet 5.5 and Claude Haiku 5.5 are announced to follow "in the coming weeks."
>
> - **Pricing:** $4.00 input / $20.00 output per MTok (20% cheaper than Opus 5's $5/$25) · Cache write (5 min): $5.00/MTok · Cache write (1 hr): $8.00/MTok · **Cache read (hit): $0.20/MTok — a 0.05× multiplier, 60% cheaper than Opus 5's $0.50/MTok (0.1×)**. Batch: $2.00 input / $10.00 output. Fast Mode: $8.00 input / $40.00 output (up to 2.5× speed).
> - **Specs:** 1,000,000-token context window · 128,000 max output tokens · reliable knowledge cutoff June 2026 · thinking is **adaptive only and can no longer be disabled** (unlike Opus 5) · default reasoning effort `medium` · tool-use system prompt overhead (`auto`/`none`): 286 tokens, identical to Opus 5.
> - **Safety:** First Opus model to launch with Fable-5.1-class safeguards on cybersecurity, biology, and anti-distillation (preserved thinking) — most cybersecurity tasks re-route to Claude Opus 4.8; advanced biology work requires the Life Sciences Verification Program. Available with zero data retention, like previous Opus models.
> - **Benchmarks (Anthropic's own):** Terminal-Bench 4.0 66.4% (vs. Fable 5.1's 55.8%, Opus 5's 52.3%, GPT-6 Astra's 57.9%); beats GPT-6 Astra on FrontierCode at ~20% of the cost per task; matches GPT-6 Astra on Terminal-Bench 4.0 at ~40% of the cost.
> - **Availability:** Claude API/Platform (`claude-opus-5-5`), Claude.ai, Claude Code, Claude Cowork, Amazon Web Services, Google Cloud, Microsoft Azure.
> - **Notable:** Anthropic's `platform.claude.com/docs/en/models/overview` "Compare models" grid now recommends Opus 5.5 (not Opus 5) alongside Fable 5.1, Sonnet 5, and Haiku 4.5 as the four primary model choices. Claude Sonnet 5.5 and Haiku 5.5 are confirmed upcoming but **not yet released/priced**.
>
> 🆕 **September 1, 2026 — Claude Fable 5.1 and Claude Mythos 5.1 launched.** Anthropic's most-advanced models for coding and knowledge work; same underlying model, different safeguard levels. Headline price unchanged at $10/$50 per MTok, but cache-read pricing drops 75% to **$0.25/MTok (0.025×)** — Anthropic estimates this cuts typical workload costs by ~25% and highly agentic workload costs by up to ~45%. Model ID: `claude-fable-5-1`.
>
> ✅ **September 1, 2026 — Claude Sonnet 5's $2/$10 pricing is now PERMANENT.** The scheduled increase to $3/$15 did not occur.
>
> ✅ **Claude Sonnet 4 + Opus 4 RETIRED on June 15, 2026. ❌** API calls to `claude-sonnet-4-20250514` and `claude-opus-4-20250514` now return errors (except via Amazon Bedrock and Google Cloud). Migration: Sonnet 4 → Sonnet 5 or Sonnet 4.6; Opus 4 → Opus 5.5 or Opus 4.8.

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

> 🔜 **Claude Sonnet 5.5 and Claude Haiku 5.5** are confirmed to be following "in the coming weeks." **Not yet released — no pricing published.**

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

### Claude Sonnet 5 *(Default Sonnet-Tier Model — pricing permanent since Sept 1, 2026)*

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-sonnet-5` |
| **Released** | June 30, 2026 |
| **Status** | ✅ Active — **Default Sonnet-Tier Model; best combination of speed and intelligence** |
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

### Claude Haiku 4.5

| Field | Value |
|---|---|
| **Provider** | Anthropic |
| **Model ID** | `claude-haiku-4-5` |
| **Released** | October 2025 |
| **Status** | ✅ Active — Fastest model with near-frontier intelligence |
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
| Claude Fable 5.1 | ❌ No | ✅ Yes (always on) | Defaults: High effort (Claude Code), Medium (Cowork/Claude.ai). |
| Claude Mythos 5.1 | ❌ No | ✅ Yes (always on) | 🔒 Trusted access only (CVP / LSVP). |
| Claude Opus 5 | ❌ No | ✅ Yes | 🔄 Replaced by Opus 5.5; still active. |
| Claude Opus 4.8 | ❌ No | ✅ Yes | Fast Mode at 2× pricing. |
| Claude Sonnet 5 | ❌ No | ✅ Yes | $2/$10 pricing permanent; effort defaults to `high`. |
| Claude Sonnet 4.6 | ✅ Yes | ✅ Yes | Only Sonnet-tier model with Extended Thinking. |
| Claude Haiku 4.5 | ✅ Yes | ❌ No | Fastest; extended thinking for budget reasoning. |

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

### ⚠️ LEGACY — Claude Sonnet 4.5

| Field | Value |
|---|---|
| **Model ID** | `claude-sonnet-4-5` |
| **Status** | 1M context beta RETIRED April 30, 2026; max context now 200K |
| **Input/Output price** | $3.00 / $15.00 per MTok |
| **Migration** | → **Claude Sonnet 5** or **Claude Sonnet 4.6** |

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
| **Batch API** | 50% off input + output (all models, 24 hr turnaround) |
| **Fable 5.1 / Opus 5.5 cache-read discounts** | Fable 5.1: $0.25/MTok (0.025×); Opus 5.5: $0.20/MTok (0.05×) — both far cheaper than the standard 0.1× multiplier |
| **✅ Sonnet 5 pricing permanent** | $2/$10 per MTok |
| **US-only inference (data residency)** | 1.1× pricing on Opus 4.6+, Sonnet 4.6+, Sonnet 5, Opus 5, Opus 5.5, and Fable 5.1/Mythos 5.1 |
| **⚠️ Sonnet 4 + Opus 4 RETIRED** | Retired June 15, 2026 ❌ on Claude API |
| **⚠️ Opus 4.1 RETIRED** | Retired August 5, 2026 on the Claude API (still on Bedrock/Google Cloud) |
| **Claude Managed Agents** | $0.08/session-hour runtime + standard token rates |

---

*Sources last verified: September 23, 2026 against `platform.claude.com/docs/en/about-claude/pricing`, `platform.claude.com/docs/en/models/overview`, `claude.com/pricing`, and `anthropic.com/news`. **This cycle:** independently re-checked all sources through September 23 — no new releases, retirements, or price changes since the September 22 refresh that introduced Claude Opus 5.5 as the new recommended default model. Claude Sonnet 5.5 and Haiku 5.5 remain announced but unreleased.*
