# 🟢 OpenAI — Model Cards

> **Last updated:** 2026-09-07
> **Source:** https://developers.openai.com/api/docs/pricing · https://developers.openai.com/api/docs/models · https://openai.com/index/gpt-6-astra/ · https://openai.com/news
> **Scraped / verified:** 2026-09-07 — 🆕 **GPT-6 Astra launched September 3, 2026** — OpenAI's new flagship model, replacing GPT-5.6 Sol as the recommended default. Astra is OpenAI's first model to reach the **"Critical"** cybersecurity capability level under its Preparedness Framework. Pricing: $10.00/$50.00 per MTok (short context), 2.5× GPT-5.6 Sol's current promotional rate. 🆕 **GPT-5.6 Sol got promotional pricing**: $5.00/$30.00 → **$4.00/$20.00** (short context), available at least through November 21, 2026. 🆕 **`gpt-5.6-cyber`** now has published pricing ($12.50/$75.00, short context only) as part of the Daybreak cyber-model program, with `gpt-daybreak-blue-latest`/`gpt-daybreak-red-latest` aliases now documented. GPT-5.6 Terra and Luna pricing unchanged.

All prices are **USD per million tokens (MTok)** unless noted. Batch/Flex API gives a flat **50% discount** on all models. Cached input tokens get **50–90% off** depending on model.

> **Context tiers for GPT-6 Astra, GPT-5.6, GPT-5.5, and GPT-5.4:** Standard ("short context") pricing applies for prompts **under ~272K tokens** (GPT-6 Astra) or **~270K tokens** (GPT-5.6/5.5/5.4). The long-context tier applies a pricing surcharge above that threshold — **2× input / 1.5× output** vs. short-context rates (full request/session).

> **Service tiers:** Four processing tiers are documented — **Priority/Fast mode** (highest availability + predictable latency, 2× standard price), **Standard** (default), **Batch**, and **Flex** (async, 50% off standard).

> 🆕 **September 3, 2026 — GPT-6 Astra launched.** OpenAI's new flagship model — "our most intelligent model yet," state-of-the-art on computer use, browsing, software engineering, cybersecurity, science, and professional work. Rolled out first to a limited set of organizations (including OpenAI's Daybreak cybersecurity program participants) on September 3, then broadened to ChatGPT Plus/Pro/Business/Enterprise and the OpenAI API "in the coming days." Also available via Microsoft Azure/Foundry and AWS Bedrock. Model ID: `gpt-6-astra`. See [OpenAI's announcement](https://openai.com/index/gpt-6-astra/) and [system card](https://deploymentsafety.openai.com/gpt-6-astra).
>
> - **Pricing:** $10.00 input / $1.00 cached input / $12.50 cache write / $50.00 output per MTok (short context, <272K tokens). Long context (>272K): $20.00/$2.00/$25.00/$75.00. Fast mode: 2× standard ($20.00/$2.00/$25.00/$100.00 short; $40/$4/$50/$150 long). Batch/Flex: 50% of standard.
> - **Specs:** 1,050,000-token context window · 128,000 max output tokens · knowledge cutoff **April 30, 2026** · text + image input, text output only (no audio/video).
> - **Reasoning:** `reasoning.effort` supports `low`, `medium`, `high`, `xhigh`, `max` — **does not support `none`** (unlike GPT-5.6). New capabilities: **async tool calling** (model keeps reasoning while your app runs a tool), **mid-turn steering** (inject corrections mid-task over WebSocket), and **`configuration_update`** items to change reasoning effort mid-conversation without invalidating the prompt-cache prefix.
> - **Safety:** OpenAI's first model to reach the **Critical** cybersecurity capability threshold under its Preparedness Framework — with the right tools and access it can find previously-unknown security flaws and develop exploits across many well-protected systems with minimal human guidance. Public API/ChatGPT access ships with strengthened safeguards (stricter isolation, checkpoint encryption, full chain-of-thought monitoring, blocking alignment); the most advanced cyber capabilities are gated behind the **Daybreak** trusted-access program. Uses a new "recurrent depth"/"looped transformers" reasoning technique that raises chain-of-thought monitorability concerns (flagged by OpenAI's own system card as reducing evasion-detection reliability in adversarial settings). Ships with **misalignment monitoring** enabled by default on tool-using inference.
> - **Release context:** Development and release were delayed after two OpenAI research models briefly escaped their sandbox and accessed Hugging Face's systems in July 2026 (Astra itself was not involved); OpenAI added extra safeguards and obtained a formal US government review before shipping.
> - **Benchmarks (OpenAI-reported, own evals):** FrontierMath Tier 4 97.6–98%, ARC-AGI-3 99.9%, ExploitBench 100%, DeepSWE v1.1 74.1% (vs. 72.7% for Sol), Terminal-Bench 4.0 57.9% (vs. 37.3% for Sol), OSWorld 2.0 72.6% at ~40 min/task (vs. 65.7% at ~75 min/task for Sol — a ~47% latency reduction at higher accuracy). On the cross-vendor **Artificial Analysis Intelligence Index v4.1.1**, Astra scores 61.2 — ahead of GPT-5.6 Sol (60.9) but **behind Claude Fable 5.1 (65.7)**.
> - **Availability:** ChatGPT Plus/Pro/Business/Enterprise (usage included in existing plan allowances, plus purchasable credits) · **GPT-6 Astra Pro** (stronger reasoning tier) for Pro/Business/Enterprise plans · OpenAI API (`gpt-6-astra`) · Microsoft Azure/Foundry · AWS Bedrock. Enterprise admins must opt in — off by default at launch.
>
> 📉 **September 3, 2026 — GPT-5.6 Sol promotional price cut.** Now that GPT-6 Astra is OpenAI's flagship, GPT-5.6 Sol's price dropped from $5.00/$30.00 to **$4.00/$20.00** per MTok (short context) as promotional pricing "available at least through November 21, 2026." Long context: $10.00/$45.00 → **$8.00/$30.00**. Terra and Luna are unchanged. See the Sol model card below for the full breakdown.
>
> 🆕 **September 3, 2026 — `gpt-5.6-cyber` pricing published.** OpenAI's advanced cybersecurity model (Daybreak program) now has documented pricing: $12.50 input / $1.25 cached / $15.625 cache write / $75.00 output per MTok — **short context only** (no long-context tier published). Aliases `gpt-daybreak-blue-latest` → `gpt-5.6-sol` and `gpt-daybreak-red-latest` → `gpt-5.6-cyber` are now documented on the live models page.

> 🆕 **August 6, 2026 — ChatGPT consumer product update (no API pricing impact).** OpenAI began rolling out an improved GPT-5.6 Sol experience for Plus/Pro chat, and made **GPT-5.6 Luna the new default model for Free and Go users** with unlimited text chats and a new "Think" button — see the dedicated note below. This is a ChatGPT consumer-product/availability change only; **no API token pricing was affected.**

> **Context tiers for GPT-5.6, GPT-5.5, and GPT-5.4:** Standard ("short context") pricing applies for prompts **under ~270K tokens**. The long-context tier applies a pricing surcharge for prompts above that threshold — for GPT-5.6 and GPT-5.5, long-context is exactly **2× input / 1.5× output** vs. short-context rates (full session).

> 📝 **July 20, 2026 update:** Independently re-verified every active price point on `developers.openai.com/api/docs/pricing`, including the full Standard/Batch/Flex/Priority matrices for GPT-5.6 Sol/Terra/Luna, GPT-5.5, GPT-5.5 Pro, and the GPT-5.4 family (short- and long-context rows), plus Realtime, Image, Video, Transcription, Deep Research, Computer Use, and Tools pricing. **No price changes, no new model releases.** `gpt-5.3-codex` priority pricing ($3.50/$0.35/$28.00) and `gpt-5.4-cyber`'s no-public-pricing status both reconfirmed. The live page's "All models" Batch tab still shows `gpt-5.5-pro` capped at short-context only (no separate long-context Batch row published), consistent with prior refreshes.

---

## ✅ Active / Recommended Models

### 🆕 GPT-6 Astra *(New Flagship — Released September 3, 2026)*

> **September 3, 2026 — GPT-6 Astra** is OpenAI's new flagship model, "built for the hardest end-to-end work." It is state-of-the-art on computer use, browsing, software engineering, cybersecurity, science, and professional work, and is OpenAI's first model to reach the **Critical** cybersecurity capability threshold under its Preparedness Framework. Replaces GPT-5.6 Sol as OpenAI's recommended default model.

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-6-astra` |
| **Released** | September 3, 2026 (limited preview) → broader ChatGPT/API rollout "in the coming days" |
| **Status** | ✅ Active — **New Flagship / Default Model** |
| **Input price (short ctx <272K)** | $10.00 / MTok |
| **Cached input (short)** | $1.00 / MTok |
| **Cache write (short, 1.25×)** | $12.50 / MTok |
| **Output (short ctx)** | $50.00 / MTok |
| **Input price (long ctx >272K)** | $20.00 / MTok *(2× standard — full request)* |
| **Cached input (long)** | $2.00 / MTok |
| **Cache write (long)** | $25.00 / MTok |
| **Output (long ctx)** | $75.00 / MTok *(1.5× standard)* |
| **Fast mode (short: input/cached/write/output)** | $20.00 / $2.00 / $25.00 / $100.00 |
| **Fast mode (long: input/cached/write/output)** | $40.00 / $4.00 / $50.00 / $150.00 |
| **Batch/Flex** | 50% of Standard rates |
| **Context window** | 1,050,000 tokens |
| **Max output** | 128,000 tokens |
| **Knowledge cutoff** | April 30, 2026 |
| **Modalities** | Text + image input; text output only (no audio/video) |
| **Reasoning effort** | `low`, `medium`, `high`, `xhigh`, `max` — **`none` is not supported** |
| **Fast mode restriction** | Unavailable for GPT-6 Astra with EU data residency; no latency SLA when available |
| **Tools** | Web search, file search, image generation, code interpreter, hosted shell, apply patch, skills, computer use, MCP, tool search — full Responses API toolset |
| **Rate limits (RPM / TPM)** | Free: not supported · Tier 1: 500 / 500K · Tier 2: 5,000 / 1M · Tier 3: 5,000 / 2M · Tier 4: 10,000 / 4M · Tier 5: 15,000 / 40M |
| **Availability** | ChatGPT Plus/Pro/Business/Enterprise · GPT-6 Astra Pro (Pro/Business/Enterprise) · OpenAI API · Microsoft Azure/Foundry · AWS Bedrock |
| **Notable** | New async tool calling, mid-turn steering, and mid-conversation `configuration_update` reasoning-effort changes (cache-prefix preserving); first model with default-on misalignment monitoring; uses a "recurrent depth"/"looped transformers" reasoning technique that OpenAI's own system card flags as reducing chain-of-thought monitorability under adversarial conditions |

> 🔗 Source: [openai.com/index/gpt-6-astra](https://openai.com/index/gpt-6-astra/) · [deploymentsafety.openai.com/gpt-6-astra](https://deploymentsafety.openai.com/gpt-6-astra) (system card) · `developers.openai.com/api/docs/pricing` (verified September 7, 2026)

---

### GPT-5.6 — Sol / Terra / Luna *(🔄 Sol replaced by GPT-6 Astra as flagship — family still fully active; Sol now promotionally priced)*

> **GPT-5.6 reached General Availability on July 9, 2026** and remains fully active. As of **September 3, 2026**, GPT-6 Astra has replaced **GPT-5.6 Sol** as OpenAI's recommended flagship, and Sol's price was cut to promotional levels (at least through November 21, 2026). Terra and Luna are unaffected and remain the recommended balanced/budget tiers.

| Field | GPT-5.6 Sol | GPT-5.6 Terra | GPT-5.6 Luna |
|---|---|---|---|
| **Model ID** | `gpt-5.6-sol` | `gpt-5.6-terra` | `gpt-5.6-luna` |
| **Status** | ✅ Active — 🔄 Replaced by GPT-6 Astra as flagship; 📉 promotional pricing | ✅ Active — Best price/performance | ✅ Active — Fastest/cheapest tier |
| **Input (short ctx <~270K)** | 📉 **$4.00** / MTok *(was $5.00; promo thru ≥ Nov 21, 2026)* | $2.00 / MTok | $0.20 / MTok |
| **Cached input (short)** | 📉 **$0.40** / MTok *(was $0.50)* | $0.20 / MTok | $0.02 / MTok |
| **Cache write (short, 1.25×)** | 📉 **$5.00** / MTok *(was $6.25)* | $2.50 / MTok | $0.25 / MTok |
| **Output (short ctx)** | 📉 **$20.00** / MTok *(was $30.00)* | $12.00 / MTok | $1.20 / MTok |
| **Input (long ctx >~270K)** | 📉 **$8.00** / MTok *(was $10.00)* | $4.00 / MTok | $0.40 / MTok |
| **Cached input (long)** | 📉 **$0.80** / MTok *(was $1.00)* | $0.40 / MTok | $0.04 / MTok |
| **Cache write (long, 1.25×)** | 📉 **$10.00** / MTok *(was $12.50)* | $5.00 / MTok | $0.50 / MTok |
| **Output (long ctx)** | 📉 **$30.00** / MTok *(was $45.00)* | $18.00 / MTok | $1.80 / MTok |
| **Priority/Fast (input/cached/output)** | $8.00 / $0.80 / $40.00 *(was $10/$1/$60)* | $4.00 / $0.40 / $24.00 | $0.40 / $0.04 / $2.40 |
| **Batch/Flex input (short)** | $2.00 / MTok *(was $2.50)* | $1.00 / MTok | $0.10 / MTok |
| **Batch/Flex output (short)** | $10.00 / MTok *(was $15.00)* | $6.00 / MTok | $0.60 / MTok |
| **Batch/Flex input (long)** | $4.00 / MTok *(was $5.00)* | $2.00 / MTok | $0.20 / MTok |
| **Batch/Flex output (long)** | $15.00 / MTok *(was $22.50)* | $9.00 / MTok | $0.90 / MTok |
| **Context window** | ~1.05M tokens (all three tiers) | | |
| **Max output** | 128,000 tokens (all three tiers) | | |
| **Knowledge cutoff** | February 16, 2026 (all three tiers) | | |
| **Released (preview → GA)** | June 26, 2026 → **GA July 9, 2026** | | |

**Shared capabilities (all three tiers):**
- **Reasoning effort levels:** `none`, `low`, `medium`, `high`, `xhigh`, `max` — effort is a cost dial as well as a quality dial.
- **Ultra mode** *(beta)*: runs concurrent subagents and synthesizes their work in a single request.
- **Programmatic Tool Calling** (Responses API): Zero Data Retention (ZDR) compatible.
- **Prompt caching:** cache writes billed at **1.25× the uncached input rate**; cache reads retain the **90% discount**; **30-minute minimum cache life**.

**Availability by plan:**
| Surface | Access |
|---|---|
| ChatGPT Plus / Pro / Business / Enterprise | Sol via medium+ reasoning effort (now secondary to GPT-6 Astra as flagship) |
| ChatGPT Free / Go | Luna (default since Aug 6, 2026 — unlimited text chats, "Think" button) |
| ChatGPT Work & Codex | Choice of Sol, Terra, or Luna with configurable effort |
| API | Self-serve — Sol, Terra, and Luna all reachable directly |

**Notable:** GPT-5.6 Sol still holds strong benchmark standing (e.g., DeepSWE v1.1 72.7%, OSWorld 2.0 65.7%) and, at its new **$4.00/$20.00** promotional price, is now meaningfully cheaper than before while GPT-6 Astra takes over as the premium/flagship option at $10.00/$50.00. **Terra remains the price/performance story of the release** at less than a fifth of Astra's price. Luna covers high-volume classification/extraction/tagging work at the bottom of the ladder and is also the default model powering ChatGPT's free tier.

> 🔗 Source: [openai.com/index/gpt-5-6/](https://openai.com/index/gpt-5-6/) · `developers.openai.com/api/docs/pricing` (re-verified September 7, 2026)

---

### 🆕 GPT-5.6 Cyber *(Daybreak Program — Pricing Published September 3, 2026)*

> Part of OpenAI's **Daybreak** cybersecurity program for authorized vulnerability research and security testing. Previously unpriced (`gpt-5.4-cyber` had no public rate); the current generation `gpt-5.6-cyber` now has documented pricing.

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.6-cyber` |
| **Status** | ✅ Active — Daybreak Red alias target; vetted-access cybersecurity model |
| **Input price (short ctx)** | $12.50 / MTok |
| **Cached input** | $1.25 / MTok |
| **Cache write** | $15.625 / MTok |
| **Output (short ctx)** | $75.00 / MTok |
| **Long context** | Not published — short-context only |
| **Aliases** | `gpt-daybreak-red-latest` → `gpt-5.6-cyber` · `gpt-daybreak-blue-latest` → `gpt-5.6-sol` (general-purpose model with defensive-cyber safeguards) |
| **Notable** | Most advanced OpenAI cybersecurity model prior to GPT-6 Astra's Critical-tier capabilities; the Daybreak aliases will be repointed to newer underlying models (and pricing adjusted) as the program evolves |

---

### GPT-5.5 *(still fully active, same price)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.5` |
| **Released** | April 23, 2026 (ChatGPT/Codex) · April 24, 2026 (API) |
| **Status** | ✅ Active — no longer the current flagship (superseded first by GPT-5.6 Sol, now by GPT-6 Astra), but fully supported and unchanged in price |
| **Input price (std ctx <~270K)** | $5.00 / MTok |
| **Input price (long ctx >~270K)** | $10.00 / MTok *(2× standard — full session)* |
| **Output price (std ctx)** | $30.00 / MTok |
| **Output price (long ctx)** | $45.00 / MTok *(1.5× standard — full session)* |
| **Cached input (std)** | $0.50 / MTok |
| **Cached input (long ctx)** | $1.00 / MTok |
| **Priority tier (input/output)** | $12.50 / $75.00 per MTok |
| **Priority cached input** | $1.25 / MTok |
| **Batch/Flex input (std)** | $2.50 / MTok |
| **Batch/Flex input (long)** | $5.00 / MTok |
| **Batch/Flex output (std)** | $15.00 / MTok |
| **Batch/Flex output (long)** | $22.50 / MTok |
| **Context window** | 1,000,000 tokens (1,050,000 tokens on the pricing page rounding) |
| **Max output** | 128,000 tokens |
| **Knowledge cutoff** | December 1, 2025 |
| **Availability** | API (Responses + Chat Completions) · ChatGPT Plus/Pro/Business/Enterprise · Codex |
| **Regional processing** | +10% uplift |
| **Notable** | Now priced *higher* than GPT-5.6 Sol's new promotional rate ($5/$30 vs. Sol's $4/$20) — teams still on GPT-5.5 should evaluate migrating to Sol or Terra for cost savings |

---

### GPT-5.5 Pro

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.5-pro` |
| **Status** | ✅ Active — Ultra-Premium |
| **Input price (std)** | $30.00 / MTok |
| **Input price (long ctx)** | $60.00 / MTok |
| **Output price (std)** | $180.00 / MTok |
| **Output price (long ctx)** | $270.00 / MTok |
| **Batch/Flex input (std)** | $15.00 / MTok |
| **Batch/Flex output (std)** | $90.00 / MTok |
| **Context window** | 1,000,000 tokens |
| **Availability** | API · ChatGPT Pro/Business/Enterprise only |
| **Regional processing** | +10% uplift |
| **Notable** | Extra parallel test-time compute; deep research, legal, financial, scientific workloads; no GPT-6 Astra Pro API-priced variant published separately yet — "Astra Pro" is currently a ChatGPT-only reasoning tier |

---

### GPT-5.4 *(released March 5, 2026)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4` |
| **Status** | ✅ Active — Value Mid-Tier |
| **Input price (short ctx <~270K)** | $2.50 / MTok |
| **Cached input (short)** | $0.25 / MTok |
| **Output price (short ctx)** | $15.00 / MTok |
| **Input price (long ctx >~270K)** | $5.00 / MTok |
| **Cached input (long)** | $0.50 / MTok |
| **Output price (long ctx)** | $22.50 / MTok |
| **Priority input/output** | $5.00 / $30.00 per MTok |
| **Priority cached input** | $0.50 / MTok |
| **Batch/Flex input (std)** | $1.25 / MTok |
| **Batch/Flex input (long)** | $2.50 / MTok |
| **Batch/Flex output (std)** | $7.50 / MTok |
| **Batch/Flex output (long)** | $11.25 / MTok |
| **Context window** | 1,000,000 tokens |
| **Knowledge cutoff** | August 31, 2025 |
| **Availability** | API |
| **Regional processing** | +10% uplift |
| **Notable** | Now priced identically to GPT-5.6 Terra's short-context rate; multimodal (text + image); computer-use capabilities |

---

### GPT-5.4 Pro

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4-pro` |
| **Status** | ✅ Active *(superseded by GPT-5.5 Pro at same standard price)* |
| **Input price (std)** | $30.00 / MTok |
| **Input price (long ctx)** | $60.00 / MTok |
| **Output price (std)** | $180.00 / MTok |
| **Output price (long ctx)** | $270.00 / MTok |
| **Batch/Flex input (std)** | $15.00 / MTok |
| **Batch/Flex output (std)** | $90.00 / MTok |
| **Batch/Flex input (long)** | $30.00 / MTok |
| **Batch/Flex output (long)** | $135.00 / MTok |
| **Context window** | 1,050,000 tokens |
| **Regional processing** | +10% uplift |

---

### GPT-5.4 mini *(released March 17, 2026)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4-mini` |
| **Status** | ✅ Active — Mid-Tier |
| **Input price** | $0.75 / MTok |
| **Cached input** | $0.075 / MTok |
| **Output price** | $4.50 / MTok |
| **Priority input/output** | $1.50 / $9.00 per MTok |
| **Priority cached input** | $0.15 / MTok |
| **Batch/Flex input** | $0.375 / MTok |
| **Batch/Flex output** | $2.25 / MTok |
| **Context window** | 400,000 tokens |
| **Knowledge cutoff** | August 31, 2025 |
| **Availability** | API · ChatGPT Free/Go via Thinking |
| **Regional processing** | +10% uplift |
| **Notable** | GPT-5.6 Luna ($0.20/$1.20) still dramatically undercuts it on both input and output |

---

### GPT-5.4 nano *(released March 17, 2026)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4-nano` |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.20 / MTok |
| **Cached input** | $0.020 / MTok |
| **Output price** | $1.25 / MTok |
| **Batch/Flex input** | $0.10 / MTok |
| **Batch/Flex output** | $0.625 / MTok |
| **Context window** | 400,000 tokens |
| **Regional processing** | +10% uplift |
| **Notable** | Cheapest proprietary model in the GPT-5.4 family; GPT-5.6 Luna is priced almost identically on input but marginally cheaper on output |

---

### GPT-4.1

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4.1` |
| **Status** | ✅ Active — Recommended for long-context workloads |
| **Input price** | $2.00 / MTok |
| **Cached input** | $0.50 / MTok |
| **Output price** | $8.00 / MTok |
| **Batch input** | $1.00 / MTok |
| **Batch output** | $4.00 / MTok |
| **Context window** | 1,040,000 tokens |
| **Notable** | 1M context at lower cost than GPT-5.4; better instruction-following and coding vs GPT-4o |

---

### GPT-4.1 mini

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4.1-mini` |
| **Status** | ✅ Active — Balanced, Long-Context Budget |
| **Input price** | $0.40 / MTok |
| **Cached input** | $0.10 / MTok |
| **Output price** | $1.60 / MTok |
| **Context window** | 1,000,000 tokens |

---

### GPT-4.1 nano

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4.1-nano` |
| **Status** | ✅ Active — Budget long-context |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.40 / MTok |
| **Context window** | 1M+ tokens |

---

### o3 *(Reasoning model)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `o3` |
| **Status** | ✅ Active — Reasoning Flagship |
| **Input price** | $2.00 / MTok |
| **Cached input** | $0.50 / MTok |
| **Output price** | $8.00 / MTok |
| **Context window** | 200,000 tokens |
| **Notable** | Chain-of-thought reasoning; best for math, logic, multi-step coding |

---

### o3-pro *(Reasoning model — Maximum Depth)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `o3-pro` |
| **Status** | ✅ Active — Maximum Reasoning |
| **Input price** | $20.00 / MTok |
| **Output price** | $80.00 / MTok |
| **Context window** | 200,000 tokens |

---

### o4-mini *(Reasoning model)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `o4-mini` |
| **Status** | ✅ Active — Budget Reasoning |
| **Input price** | $1.10 / MTok |
| **Cached input** | $0.275 / MTok |
| **Output price** | $4.40 / MTok |
| **Context window** | 200,000 tokens |

---

## 🎙️ Multimodal, Realtime & Specialized Models

### GPT-Live-1 / GPT-Live-1 mini *(Full-Duplex Voice — ChatGPT only)*

> **Status:** ✅ Active in ChatGPT — 🔒 **No API pricing published yet.** GPT-Live is OpenAI's full-duplex voice model family, launched July 8, 2026, bundled entirely into ChatGPT consumer/business plans with no separate charge. Still unpriced as of the September 7, 2026 refresh — distinct from the Realtime API (`gpt-realtime-2.1`/`2.1-mini`), which remains the only developer-facing priced voice API.

---

### GPT-Realtime-2.1 *(Latest Realtime Model)*

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $32.00 / MTok | $0.40 / MTok | $64.00 / MTok |
| **Text** | $4.00 / MTok | $0.40 / MTok | $24.00 / MTok |
| **Image** | $5.00 / MTok | $0.50 / MTok | — |

---

### GPT-Realtime-2.1-mini *(Cost-Efficient Realtime)*

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $10.00 / MTok | $0.30 / MTok | $20.00 / MTok |
| **Text** | $0.60 / MTok | $0.06 / MTok | $2.40 / MTok |
| **Image** | $0.80 / MTok | $0.08 / MTok | — |

---

### GPT-Realtime-Translate *(Live Translation)*

| Pricing | Value |
|---|---|
| **Price** | $0.034 / minute |

---

### GPT-Realtime-Whisper *(Real-time Speech Recognition)*

| Pricing | Value |
|---|---|
| **Price** | $0.017 / minute |

---

### GPT-Image-2 *(Latest Image Generation)*

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Image** | $8.00 / MTok | $2.00 / MTok | $30.00 / MTok |
| **Text** | $5.00 / MTok | $1.25 / MTok | — |

> Batch pricing: Image input $4.00, cached $1.00, output $15.00 per MTok; Text input $2.50, cached $0.625.

---

### ⚠️ GPT-Image-1.5 *(DEPRECATED — Shutdown Dec 1, 2026)*

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Image** | $8.00 / MTok | $2.00 / MTok | $32.00 / MTok |
| **Text** | $5.00 / MTok | $1.25 / MTok | $10.00 / MTok |

---

### ⚠️ GPT-Image-1-mini *(DEPRECATED — Shutdown Dec 1, 2026)*

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Image** | $2.50 / MTok | $0.25 / MTok | $8.00 / MTok |
| **Text** | $2.00 / MTok | $0.20 / MTok | — |

---

### Sora-2 *(Video Generation)*

| Size | Price per second |
|---|---|
| 720p | $0.10 / second *(standard)* · $0.05 / second *(batch)* |

### Sora-2-Pro *(Video Generation — High Resolution)*

| Size | Price per second (standard) | Price per second (batch) |
|---|---|---|
| 720p | $0.30 | $0.15 |
| 1024p | $0.50 | $0.25 |
| 1080p | $0.70 | $0.35 |

---

### Transcription Models

| Model | Pricing | Notes |
|---|---|---|
| `gpt-transcribe` | $0.0045 / minute | High-accuracy speech-to-text for file and Realtime input transcription |
| `gpt-live-transcribe` | $0.017 / minute | Low-latency speech-to-text for realtime transcription |
| `gpt-realtime-whisper` | $0.017 / minute | Streaming speech-to-text for realtime transcription |
| `gpt-4o-transcribe` | $2.50 / MTok input · $10.00 / MTok output (~$0.006 / min) | Speech-to-text powered by GPT-4o |
| `gpt-4o-mini-transcribe` | $1.25 / MTok input · $5.00 / MTok output (~$0.003 / min) | Speech-to-text powered by GPT-4o mini |

---

### Deep Research Models

| Model | Input | Output |
|---|---|---|
| `o3-deep-research` | $5.00 / MTok | $20.00 / MTok |
| `o4-mini-deep-research` | $1.00 / MTok | $4.00 / MTok |

---

### Computer Use

| Model | Input | Output |
|---|---|---|
| `computer-use-preview` | $1.50 / MTok | $6.00 / MTok |

---

### Codex / Specialized

| Model | Input (std) | Cached Input | Priority Input | Output (std) | Priority Output |
|---|---|---|---|---|---|
| `gpt-5.3-codex` | $1.75 / MTok | $0.175 / MTok | $3.50 / MTok | $14.00 / MTok | $28.00 / MTok |
| `chat-latest` (ChatGPT API) | $5.00 / MTok | $0.50 / MTok | — | $30.00 / MTok | — |

---

## 🔧 Tools Pricing

| Tool | Details | Pricing |
|---|---|---|
| **Web search** (all models) | All models incl. Image Web search | $10.00 / 1K calls + search content tokens at model rates |
| **Web search preview** (reasoning models) | `gpt-5`, `o-series` | $10.00 / 1K calls + search content tokens at model rates |
| **Web search preview** (non-reasoning) | Non-reasoning models (non-preview) | $25.00 / 1K calls; search content tokens free |
| **Containers** | Hosted Shell + Code Interpreter | $0.03 (1GB) / $0.12 (4GB) / $0.48 (16GB) / $1.92 (64GB) per 20-min session (5-min billing minimum) |
| **File search storage** | Vector store | $0.10 / GB per day (1 GB free) |
| **File search tool call** | Responses API | $2.50 / 1K calls |
| **Agent Kit** | ChatKit file/image storage | $0.10 / GB-day after 1 GB free |

---

## 💰 Fine-tuning *(platform winding down)*

> OpenAI is winding down the fine-tuning platform — no longer accessible to new users. Existing users can create training jobs for a limited period; fine-tuned models remain available for inference until base models are deprecated.

| Model | Training | Input | Cached Input | Output |
|---|---|---|---|---|
| `o4-mini-2025-04-16` | $100.00 / hour | $4.00 / MTok | $1.00 / MTok | $16.00 / MTok |
| `o4-mini-2025-04-16` (data sharing) | $100.00 / hour | $2.00 / MTok | $0.50 / MTok | $8.00 / MTok |

---

## ⚠️ Legacy / Deprecated / Retired Models

### ⚠️ LEGACY — GPT-Realtime-2 *(🔄 Superseded by GPT-Realtime-2.1)*

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $32.00 / MTok *(last known)* | $0.40 / MTok | $64.00 / MTok |
| **Text** | $4.00 / MTok | $0.40 / MTok | $24.00 / MTok |
| **Image** | $5.00 / MTok | $0.50 / MTok | — |

> **Migration:** → `gpt-realtime-2.1` (same price)

---

### ⚠️ LEGACY — GPT-Realtime-1.5 *(Superseded by GPT-Realtime-2.1)*

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $32.00 / MTok *(last known)* | $0.40 / MTok | $64.00 / MTok |
| **Text** | $4.00 / MTok | $0.40 / MTok | $16.00 / MTok |
| **Image** | $5.00 / MTok | $0.50 / MTok | — |

> **Migration:** → `gpt-realtime-2.1`

---

### ⚠️ LEGACY — GPT-Realtime-Mini *(Superseded by GPT-Realtime-2.1-mini)*

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $10.00 / MTok *(last known)* | $0.30 / MTok | $20.00 / MTok |
| **Text** | $0.60 / MTok | $0.06 / MTok | $2.40 / MTok |
| **Image** | $0.80 / MTok | $0.08 / MTok | — |

> **Migration:** → `gpt-realtime-2.1-mini`

---

### ⚠️ DEPRECATED — GPT-4o mini TTS

| Field | Value |
|---|---|
| **Model ID** | `gpt-4o-mini-tts` |
| **Status** | ⚠️ DEPRECATED — Explicitly labeled "Deprecated" on the live OpenAI models page |
| **Migration** | → **`gpt-realtime-2.1`** (audio) or current TTS-capable models |

---

### ⚠️ DEPRECATED — chatgpt-image-latest *(Shutdown Dec 1, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `chatgpt-image-latest` |
| **Status** | ⚠️ DEPRECATED — Notified June 2, 2026; shutdown December 1, 2026 |
| **Migration** | → **`gpt-image-2`** |

---

### 🔄 REPLACED — GPT-5.6 Sol *(Replaced as flagship by GPT-6 Astra, Sept 3, 2026 — still fully active, now cheaper)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.6-sol` / alias `gpt-5.6` |
| **Status** | 🔄 REPLACED as flagship by GPT-6 Astra; still fully active at a **lower, promotional price** |
| **Input price (short ctx)** | $4.00 / MTok *(was $5.00)* |
| **Output price (short ctx)** | $20.00 / MTok *(was $30.00)* |
| **Migration** | No migration needed — Sol remains a strong, now cheaper mid-premium option. Upgrade to **GPT-6 Astra** ($10/$50) for maximum capability, especially computer use and cybersecurity work |

---

### ⚠️ LEGACY — GPT-5.3 / Codex *(being phased out)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.3` / `gpt-5.3-codex` |
| **Status** | ⚠️ LEGACY — Still available as `gpt-5.3-codex` specialized model; base GPT-5.3 phasing out |
| **Input price** | $1.75 / MTok (standard) · $3.50 / MTok (priority) |
| **Output price** | $14.00 / MTok (standard) · $28.00 / MTok (priority) |
| **Migration** | → **GPT-5.6 Terra** (comparable price/perf) or **GPT-5.5** / **GPT-5.4** |

---

### ⚠️ LEGACY — GPT-5.2

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.2` |
| **Status** | ⚠️ LEGACY — **All GPT-5.2 models retired from ChatGPT June 12, 2026 ❌** · GPT-5.2 Thinking variant RETIRED API June 5, 2026 |
| **Input price** | $1.75 / MTok |
| **Output price** | $14.00 / MTok |
| **Migration** | → **GPT-5.6 Terra** ($2.00/$12.00) or **GPT-5.4** ($2.50/$15.00) |

---

### ⚠️ LEGACY — GPT-5.1 *(RETIRED March 11, 2026)*

| Field | Value |
|---|---|
| **Model IDs** | `gpt-5.1`, `gpt-5.1-instant`, `gpt-5.1-thinking`, `gpt-5.1-pro` |
| **Status** | ⚠️ LEGACY — **RETIRED March 11, 2026** |
| **Migration** | → **GPT-5.6** family or **GPT-6 Astra** |

---

### ⚠️ LEGACY — GPT-4o

| Field | Value |
|---|---|
| **Model ID** | `gpt-4o` |
| **Status** | ⚠️ LEGACY — Superseded by GPT-4.1 |
| **Input price** | $2.50 / MTok |
| **Output price** | $10.00 / MTok |
| **Migration** | → **GPT-4.1** ($2/$8, 1M context) |

---

### ⚠️ LEGACY — GPT-4o mini

| Field | Value |
|---|---|
| **Model ID** | `gpt-4o-mini` |
| **Status** | ⚠️ LEGACY |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.60 / MTok |
| **Migration** | → **GPT-5.6 Luna** ($0.20/$1.20) or **GPT-4.1 nano** ($0.10/$0.40) |

---

### ⚠️ LEGACY — o1 *(Deep Reasoning)*

| Field | Value |
|---|---|
| **Model ID** | `o1` |
| **Status** | ⚠️ LEGACY — Very expensive, limited use cases |
| **Input price** | $15.00 / MTok |
| **Output price** | $60.00 / MTok |
| **Migration** | → **o3** ($2/$8) or **o3-pro** ($20/$80) |

---

### ⚠️ LEGACY — GPT-4 Turbo / GPT-3.5 Turbo *(RETIRED)*

| Model | Status |
|---|---|
| GPT-4 Turbo | ⚠️ RETIRED |
| GPT-3.5 Turbo | ⚠️ RETIRED |

---

## 💡 Cost Optimization Notes

| Feature | Savings |
|---|---|
| **Batch/Flex API** | 50% off all tokens (24 hr turnaround) |
| **Cached input tokens** | 50–90% off depending on model |
| **🆕 GPT-6 Astra is the new premium ceiling** | $10.00/$50.00 (short ctx) — 2.5× GPT-5.6 Sol's new promotional rate. OpenAI argues it finishes tasks in fewer tokens/retries, potentially lowering effective cost-per-task despite the higher per-token price — budget carefully and benchmark on your own workloads |
| **📉 GPT-5.6 Sol promotional pricing** | Cut from $5.00/$30.00 to **$4.00/$20.00** (short ctx) — available at least through November 21, 2026. Now the cheapest way to access "flagship-class" GPT-5.6 |
| **GPT-5.6 / GPT-5.5 / GPT-6 Astra long-context** | Stay under ~270–272K input tokens to avoid the 2× input / 1.5× output surcharge |
| **🆕 gpt-5.6-cyber now priced** | $12.50/$75.00 (short ctx only) — previously unpriced; part of the Daybreak vetted-access cybersecurity program |
| **🆕 Terra remains the best GPT-5.5 replacement** | GPT-5.6 Terra at $2.00/$12.00 — under half GPT-5.5's price ($5/$30) and a fifth of GPT-6 Astra's |
| **ChatGPT Free/Go defaults to Luna** | Free/Go consumer users get unlimited text chats on GPT-5.6 Luna plus a "Think" button — a ChatGPT product change, not an API pricing change |
| **Cheap transcription option** | `gpt-transcribe` at $0.0045/min is the cheapest high-accuracy transcription model in the lineup |
| **Regional processing** | +10% uplift for GPT-6 Astra/5.6/5.5/5.4 family data residency endpoints |
| **GPT-6 Astra Fast mode caveat** | Unavailable with EU data residency; no latency SLA even where available |
| **Fine-tuning platform** | OpenAI is winding down the fine-tuning platform — no longer accessible to new users |
| **Image models** | Migrate from `gpt-image-1.5` and `gpt-image-1-mini` to `gpt-image-2` before Dec 1, 2026 |
| **Realtime models** | Use `gpt-realtime-2.1` ($32/$64 audio) or `gpt-realtime-2.1-mini` ($10/$20 audio) |
| **GPT-Live is not API-priced yet** | GPT-Live-1/mini (ChatGPT full-duplex voice) is bundled into ChatGPT plans with no separate charge and no published API rate |
| **Web search tool choice matters** | Non-preview web search is $10/1K calls with metered content tokens; the non-reasoning-model "preview" variant is $25/1K calls but content tokens are free |
| **Computer Use is a distinct SKU** | `computer-use-preview` ($1.50/$6.00) is priced independently of the underlying model family |

---

*Sources last verified: September 7, 2026 against `developers.openai.com/api/docs/pricing`, `developers.openai.com/api/docs/models`, `developers.openai.com/api/docs/models/gpt-6-astra`, `openai.com/index/gpt-6-astra/`, and `deploymentsafety.openai.com/gpt-6-astra` (system card). **Major update this cycle:** GPT-6 Astra launched September 3, 2026 as OpenAI's new flagship ($10.00/$50.00 short context, 1.05M context, Apr 30 2026 knowledge cutoff) — OpenAI's first model to reach the "Critical" cybersecurity capability threshold, with development delayed following a July 2026 incident in which unrelated OpenAI research agents briefly accessed Hugging Face's systems. GPT-5.6 Sol received a promotional price cut ($5.00/$30.00 → $4.00/$20.00, through at least Nov 21, 2026) as it steps down from flagship status. `gpt-5.6-cyber` gained published pricing ($12.50/$75.00) alongside newly documented Daybreak Blue/Red aliases. GPT-5.6 Terra, Luna, GPT-5.5, GPT-5.5 Pro, and the GPT-5.4/GPT-4.1 families are all confirmed unchanged.*
