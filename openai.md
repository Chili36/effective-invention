# 🟢 OpenAI — Model Cards

> **Last updated:** 2026-08-10
> **Source:** https://developers.openai.com/api/docs/pricing · https://developers.openai.com/api/docs/models · https://openai.com/index/gpt-5-6/ · https://openai.com/news
> **Scraped / verified:** 2026-08-10 — ✅ **Re-verified against the live `developers.openai.com/api/docs/pricing` page.** Every active price point (GPT-5.6 Sol/Terra/Luna, GPT-5.5, GPT-5.5 Pro, GPT-5.4 family, GPT-4.1 family, o3/o3-pro/o4-mini, Realtime, Image, Video, Transcription, Deep Research, Computer Use, Codex, and Tools pricing) matches exactly — **no price changes since the August 3, 2026 refresh.** 🆕 **New (non-pricing) ChatGPT product update discovered:** on August 6, 2026, OpenAI began rolling out an improved GPT-5.6 Sol experience for Plus/Pro chat, and made **GPT-5.6 Luna the new default model for Free and Go users** with unlimited text chats and a new "Think" button — see the dedicated note below. This is a ChatGPT consumer-product/availability change only; **no API token pricing was affected.**

All prices are **USD per million tokens (MTok)** unless noted. Batch/Flex API gives a flat **50% discount** on all models. Cached input tokens get **50–90% off** depending on model.

> **Context tiers for GPT-5.6, GPT-5.5, and GPT-5.4:** Standard ("short context") pricing applies for prompts **under ~270K tokens**. The long-context tier applies a pricing surcharge for prompts above that threshold — for GPT-5.6 and GPT-5.5, long-context is exactly **2× input / 1.5× output** vs. short-context rates (full session).

> **Service tiers:** Four processing tiers are now documented — **Priority** (highest availability + predictable latency), **Standard** (default), **Batch**, and **Flex** (async, 50% off standard). Priority tier is available for GPT-5.6 (all three tiers), GPT-5.5, GPT-5.4, and GPT-5.4 mini.

> 🆕 **August 6, 2026 — ChatGPT consumer product update (no API pricing impact).** OpenAI announced ["Improving GPT‑5.6 Sol in ChatGPT—and expanding access to GPT‑5.6 Luna for free users."](https://openai.com/index/improving-gpt-5-6-sol-in-chatgpt/) Key points:
> - **Plus/Pro chat:** GPT-5.6 Sol in the ChatGPT Chat experience was updated for more focused answers, more reliable facts (OpenAI reports ~68% fewer factual errors vs. GPT-5.5 Instant on an internal financial/medical/legal eval, vs. ~62% fewer for Luna), and a new slider to control how much "thought" is applied per response. This tuned version of Sol is scoped to ChatGPT Chat only — the API/Work/Codex version of Sol is unchanged.
> - **Free/Go users:** GPT‑5.6 Luna becomes the **default model**, with **unlimited text chats** (previously rate-limited) and a new "Think" button for deeper reasoning on harder questions, subject to abuse guardrails. File uploads, images, and other tools remain rate-limited.
> - **No API/developer pricing changed as part of this release** — it is purely a ChatGPT consumer availability and quality update. `gpt-5.6-luna` and `gpt-5.6-sol` API pricing (see table below) are unaffected.

> 📝 **July 20, 2026 update:** Independently re-verified every active price point on `developers.openai.com/api/docs/pricing`, including the full Standard/Batch/Flex/Priority matrices for GPT-5.6 Sol/Terra/Luna, GPT-5.5, GPT-5.5 Pro, and the GPT-5.4 family (short- and long-context rows), plus Realtime, Image, Video, Transcription, Deep Research, Computer Use, and Tools pricing. **No price changes, no new model releases.** `gpt-5.3-codex` priority pricing ($3.50/$0.35/$28.00) and `gpt-5.4-cyber`'s no-public-pricing status both reconfirmed. The live page's "All models" Batch tab still shows `gpt-5.5-pro` capped at short-context only (no separate long-context Batch row published), consistent with prior refreshes.

---

## ✅ Active / Recommended Models

### 🆕 GPT-5.6 — Sol / Terra / Luna *(Current Flagship Family — General Availability July 9, 2026)*

> **GPT-5.6 reached General Availability on July 9, 2026**, live across ChatGPT, Codex, and the OpenAI API — a 13-day arc from its June 26, 2026 limited preview (~20 trusted partners, gated pending US government review per the June 2, 2026 executive order on frontier model releases). GPT-5.6 introduces a new naming system: the version number (5.6) identifies the model generation, while **Sol**, **Terra**, and **Luna** are durable capability tiers (flagship / balanced / speed-and-cost) that can each advance on their own release cadence — replacing the old flagship/mini/nano suffix convention. The bare `gpt-5.6` alias routes to Sol.
>
> 📉 **August 3, 2026 — Terra and Luna price cut, confirmed on the live pricing page and model catalog.** GPT-5.6 Terra's short-context input fell from $2.50 to **$2.00**/MTok (output $15.00 → **$12.00**/MTok); GPT-5.6 Luna's short-context input fell from $1.00 to **$0.20**/MTok (output $6.00 → **$1.20**/MTok) — an ~80% cut on Luna's headline rate. Sol is unchanged at $5.00/$30.00. The table below reflects the new, lower prices; the previous rates are noted inline for reference.
>
> 🆕 **August 6, 2026 — GPT-5.6 Luna becomes the default ChatGPT model for Free/Go users** (unlimited text chats; API token pricing unchanged — see the dedicated note above).

| Field | GPT-5.6 Sol | GPT-5.6 Terra | GPT-5.6 Luna |
|---|---|---|---|
| **Model ID** | `gpt-5.6-sol` | `gpt-5.6-terra` | `gpt-5.6-luna` |
| **Input (short ctx <~270K)** | $5.00 / MTok | $2.00 / MTok 📉 *(was $2.50)* | $0.20 / MTok 📉 *(was $1.00)* |
| **Cached input (short)** | $0.50 / MTok | $0.20 / MTok *(was $0.25)* | $0.02 / MTok *(was $0.10)* |
| **Cache write (short, 1.25×)** | $6.25 / MTok | $2.50 / MTok *(was $3.125)* | $0.25 / MTok *(was $1.25)* |
| **Output (short ctx)** | $30.00 / MTok | $12.00 / MTok 📉 *(was $15.00)* | $1.20 / MTok 📉 *(was $6.00)* |
| **Input (long ctx >~270K)** | $10.00 / MTok | $4.00 / MTok *(was $5.00)* | $0.40 / MTok *(was $2.00)* |
| **Cached input (long)** | $1.00 / MTok | $0.40 / MTok *(was $0.50)* | $0.04 / MTok *(was $0.20)* |
| **Cache write (long, 1.25×)** | $12.50 / MTok | $5.00 / MTok *(was $6.25)* | $0.50 / MTok *(was $2.50)* |
| **Output (long ctx)** | $45.00 / MTok | $18.00 / MTok *(was $22.50)* | $1.80 / MTok *(was $9.00)* |
| **Priority input / cached / output** | $10.00 / $1.00 / $60.00 | $4.00 / $0.40 / $24.00 *(was $5.00/$0.50/$30.00)* | $0.40 / $0.04 / $2.40 *(was $2.00/$0.20/$12.00)* |
| **Batch/Flex input (short)** | $2.50 / MTok | $1.00 / MTok *(was $1.25)* | $0.10 / MTok *(was $0.50)* |
| **Batch/Flex output (short)** | $15.00 / MTok | $6.00 / MTok *(was $7.50)* | $0.60 / MTok *(was $3.00)* |
| **Batch/Flex input (long)** | $5.00 / MTok | $2.00 / MTok *(was $2.50)* | $0.20 / MTok *(was $1.00)* |
| **Batch/Flex output (long)** | $22.50 / MTok | $9.00 / MTok *(was $11.25)* | $0.90 / MTok *(was $4.50)* |
| **Context window** | ~1.05M tokens (all three tiers) | | |
| **Max output** | 128,000 tokens (all three tiers) | | |
| **Knowledge cutoff** | February 16, 2026 (all three tiers) | | |
| **Released (preview → GA)** | June 26, 2026 → **GA July 9, 2026** | | |
| **Status** | ✅ Active — **Current Flagship Family** | ✅ Active — Best price/performance, now cheaper | ✅ Active — Fastest/cheapest tier, now ~80% cheaper; 🆕 new default for ChatGPT Free/Go |

**Shared capabilities (all three tiers):**
- **Reasoning effort levels:** `none`, `low`, `medium`, `high`, `xhigh`, `max` — effort is a cost dial as well as a quality dial (higher settings burn more output tokens, the expensive direction).
- **Ultra mode** *(beta)*: runs concurrent subagents and synthesizes their work in a single request. Available to ChatGPT Work Pro/Enterprise and Codex Plus+ plans; same per-token pricing, higher token consumption.
- **Programmatic Tool Calling** (Responses API): lets the model write and run in-memory programs that coordinate tools, making it Zero Data Retention (ZDR) compatible.
- **Prompt caching:** cache writes billed at **1.25× the uncached input rate**; cache reads retain the **90% discount**; **30-minute minimum cache life**; explicit cache breakpoints supported.
- **Safety:** most extensive evaluation period to date (~700,000 A100e GPU-hours of automated red-teaming plus human red-teaming); cyber safeguards block roughly **10× more potentially harmful activity** than prior models; a "retry on lower-capability model" option is offered in ChatGPT/Codex to reduce friction from safety refusals.

**Availability by plan:**
| Surface | Access |
|---|---|
| ChatGPT Plus / Pro / Business / Enterprise | Sol (updated Aug 6, 2026 for more focused/accurate Chat responses) via medium+ reasoning effort settings |
| ChatGPT Pro / Enterprise | Sol Pro (highest-quality mode) also available |
| ChatGPT Free / Go | 🆕 Luna (new default as of Aug 6, 2026 — unlimited text chats, "Think" button for harder questions) |
| ChatGPT Work & Codex | Choice of Sol, Terra, or Luna with configurable effort; `max` effort and `ultra` mode available (Pro/Enterprise in Work, Plus+ in Codex); unaffected by the Aug 6 Chat-only tuning update |
| API | Self-serve — Sol, Terra, and Luna all reachable directly; pricing unaffected by ChatGPT product changes |

**Notable:** On the Artificial Analysis Coding Agent Index, **GPT-5.6 Sol with max reasoning sets a new state of the art at 80** — 2.8 points above Claude Fable 5 — while using less than half the output tokens, less than half the time, and about one-third the cost. Sol's headline price **matches GPT-5.5 exactly** ($5/$30) — no flagship price increase, just more capability at the same rate. **Terra is the price/performance story of the release:** OpenAI positions it as competitive with GPT-5.5-class quality at **half the price**, making it the natural default migration target for most production traffic. Luna covers high-volume classification/extraction/tagging work at the bottom of the ladder, and as of August 6, 2026 is also the default model powering ChatGPT's free tier. There is no mini/nano suffix in this generation — Terra and Luna fill that role as durable tiers.

> 🔗 Source: [openai.com/index/gpt-5-6/](https://openai.com/index/gpt-5-6/) · [openai.com/index/improving-gpt-5-6-sol-in-chatgpt/](https://openai.com/index/improving-gpt-5-6-sol-in-chatgpt/) · `developers.openai.com/api/docs/pricing` (re-verified August 10, 2026)

---

### GPT-5.5 *(🔄 Replaced by GPT-5.6 Sol as flagship — still fully active, same price)*

> 🔄 **REPLACED (July 9, 2026):** GPT-5.6 Sol has replaced GPT-5.5 as OpenAI's current recommended flagship. GPT-5.5 remains **fully active, unchanged in price, and not deprecated** — it continues to be listed on the live pricing page and via the API/ChatGPT/Codex. Its price is identical to Sol's ($5/$30 short context), so there is no cost reason to force a migration; the difference is purely capability (Sol is stronger on coding/agentic/reasoning benchmarks per OpenAI's own evals).

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.5` |
| **Released** | April 23, 2026 (ChatGPT/Codex) · April 24, 2026 (API) |
| **Status** | ✅ Active — 🔄 Replaced by GPT-5.6 Sol as current flagship (July 9, 2026) |
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
| **Batch/Flex cached input (std)** | $0.25 / MTok |
| **Context window** | 1,000,000 tokens (1,050,000 tokens on the pricing page rounding) |
| **Max output** | 128,000 tokens |
| **Knowledge cutoff** | December 1, 2025 |
| **Availability** | API (Responses + Chat Completions) · ChatGPT Plus/Pro/Business/Enterprise · Codex |
| **Regional processing** | +10% uplift |
| **Notable** | No prompt-caching-write premium (unlike GPT-5.6); still natively omnimodal (text+image+audio+video); remains the closest drop-in for teams not yet ready to move to GPT-5.6 Terra/Sol |

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
| **Notable** | Extra parallel test-time compute; deep research, legal, financial, scientific workloads; no GPT-5.6 Pro variant announced yet — "Pro" is a reasoning mode on Sol in the GPT-5.6 generation, not a separate model ID |

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
| **Notable** | Still the most competitive mid-tier model on price; GPT-5.6 Luna ($0.20/$1.20) now dramatically undercuts it on both input and output |

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
| **Notable** | Cheapest proprietary model in the GPT-5.4 family; ideal for classification, extraction; GPT-5.6 Luna is now priced almost identically on input ($0.20 vs $0.20) but costs slightly more on output ($1.20 vs $1.25 — Luna is actually marginally cheaper) |

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

### GPT-Live-1 / GPT-Live-1 mini *(Full-Duplex Voice — ChatGPT only, launched July 8, 2026)*

> **Status:** ✅ Active in ChatGPT — 🔒 **No API pricing published yet.** GPT-Live is OpenAI's full-duplex voice model family (it can listen and speak simultaneously, supporting natural interruption/barge-in), launched July 8, 2026 and rolled into ChatGPT's Voice experience — it is **not the same product as the Realtime API** (`gpt-realtime-2.1`/`2.1-mini`), which remains the only developer-facing voice API today. GPT-Live is bundled entirely into ChatGPT consumer/business plans with no separate charge and no per-minute or per-token rate: Free gets GPT-Live-1 mini; Go ($8/mo), Plus ($20/mo), and Pro (from $100/mo) get the full GPT-Live-1 with usage allowances that scale by plan (e.g., ChatGPT Pro $200/mo tier gets unlimited access). OpenAI has stated GPT-Live-1 and mini are "coming soon" to the API with no published token/per-minute rates — **treat this as unpriced/API-pending; do not assume Realtime API pricing applies.** Track `developers.openai.com/api/docs/pricing` for when API rates go live. Still unpriced as of the August 10, 2026 refresh.

---

### GPT-Realtime-2.1 *(Latest Realtime Model — supersedes GPT-Realtime-2)*

> **Status:** ✅ Active — Now the latest realtime voice interaction model on the live pricing page (previously listed as `gpt-realtime-2`, same pricing carried forward as a version refresh). Supports audio, text, and image inputs.

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $32.00 / MTok | $0.40 / MTok | $64.00 / MTok |
| **Text** | $4.00 / MTok | $0.40 / MTok | $24.00 / MTok |
| **Image** | $5.00 / MTok | $0.50 / MTok | — |

---

### GPT-Realtime-2.1-mini *(Cost-Efficient Realtime — supersedes GPT-Realtime-Mini)*

> **Status:** ✅ Active — Cost-efficient version of GPT-Realtime-2.1, now listed by this name on the live pricing page (previously `gpt-realtime-mini`, same pricing carried forward).

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $10.00 / MTok | $0.30 / MTok | $20.00 / MTok |
| **Text** | $0.60 / MTok | $0.06 / MTok | $2.40 / MTok |
| **Image** | $0.80 / MTok | $0.08 / MTok | — |

---

### GPT-Realtime-Translate *(Live Translation)*

> **Status:** ✅ Active — Live translation model; translates speech in real time at speaker pace.

| Pricing | Value |
|---|---|
| **Price** | $0.034 / minute |

---

### GPT-Realtime-Whisper *(Real-time Speech Recognition)*

> **Status:** ✅ Active — Real-time Whisper-based speech recognition model.

| Pricing | Value |
|---|---|
| **Price** | $0.017 / minute |

---

### GPT-Image-2 *(Latest Image Generation)*

> **Status:** ✅ Active — State-of-the-art image generation model. **Recommended migration target from deprecated image models.**

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Image** | $8.00 / MTok | $2.00 / MTok | $30.00 / MTok |
| **Text** | $5.00 / MTok | $1.25 / MTok | — |

> Batch pricing: Image input $4.00, cached $1.00, output $15.00 per MTok; Text input $2.50, cached $0.625.

---

### ⚠️ GPT-Image-1.5 *(DEPRECATED — Shutdown Dec 1, 2026)*

> **Status:** ⚠️ DEPRECATED — OpenAI notified developers June 2, 2026 of deprecation and removal December 1, 2026. **Migrate to `gpt-image-2`.**

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Image** | $8.00 / MTok | $2.00 / MTok | $32.00 / MTok |
| **Text** | $5.00 / MTok | $1.25 / MTok | $10.00 / MTok |

---

### ⚠️ GPT-Image-1-mini *(DEPRECATED — Shutdown Dec 1, 2026)*

> **Status:** ⚠️ DEPRECATED — OpenAI notified developers June 2, 2026 of deprecation and removal December 1, 2026. **Migrate to `gpt-image-2`.**

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Image** | $2.50 / MTok | $0.25 / MTok | $8.00 / MTok |
| **Text** | $2.00 / MTok | $0.20 / MTok | — |

---

### Sora-2 *(Video Generation)*

> **Status:** ✅ Active — Video generation at 720p.

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
| `gpt-5.4-cyber` | 🔒 No public pricing (Trusted Access for Cyber program only) | — | — | — | — |

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

> Note: for `gpt-4o-mini` and `gpt-4.1-mini` using the non-preview web search tool, search content tokens are billed as a fixed block of 8,000 input tokens per call rather than metered by actual retrieval size.

---

## ⚠️ Legacy / Deprecated / Retired Models

### ⚠️ LEGACY — GPT-Realtime-2 *(🔄 Superseded by GPT-Realtime-2.1)*

> **Status:** ⚠️ LEGACY — As of the July 9, 2026 pricing refresh, `gpt-realtime-2` no longer appears on the live pricing page; `gpt-realtime-2.1` is the documented model at identical pricing. Treat as a version rename rather than a price change.

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $32.00 / MTok *(last known)* | $0.40 / MTok | $64.00 / MTok |
| **Text** | $4.00 / MTok | $0.40 / MTok | $24.00 / MTok |
| **Image** | $5.00 / MTok | $0.50 / MTok | — |

> **Migration:** → `gpt-realtime-2.1` (same price)

---

### ⚠️ LEGACY — GPT-Realtime-1.5 *(Superseded by GPT-Realtime-2.1)*

> **Status:** ⚠️ LEGACY — Superseded first by `gpt-realtime-2`, now by `gpt-realtime-2.1` as the recommended model for audio in/out. Last known pricing below.

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $32.00 / MTok *(last known)* | $0.40 / MTok | $64.00 / MTok |
| **Text** | $4.00 / MTok | $0.40 / MTok | $16.00 / MTok |
| **Image** | $5.00 / MTok | $0.50 / MTok | — |

> **Migration:** → `gpt-realtime-2.1`

---

### ⚠️ LEGACY — GPT-Realtime-Mini *(Superseded by GPT-Realtime-2.1-mini)*

> **Status:** ⚠️ LEGACY — Superseded by `gpt-realtime-2.1-mini`, the current cost-efficient realtime model. Last known pricing below (identical to the new model).

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
| **Migration** | → **GPT-5.6** family |

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
| **🆕 GPT-5.6 caching model** | Cache writes cost 1.25× the uncached input rate (new); cache reads keep the 90% discount; 30-min minimum cache life |
| **GPT-5.6 / GPT-5.5 long-context** | Stay under ~270K input tokens to avoid 2× input / 1.5× output surcharge |
| **📉 Terra and Luna price cuts (Aug 3, 2026)** | Terra now $2.00/$12.00 (was $2.50/$15.00); Luna now $0.20/$1.20 (was $1.00/$6.00, an ~80% cut). Terra remains the natural GPT-5.5 replacement at well under half GPT-5.5's price; Luna is now dramatically cheaper than GPT-5.4 mini/nano for high-volume classification and extraction workloads |
| **🆕 Terra as GPT-5.5 replacement** | GPT-5.6 Terra now $2.00/$12.00 — under half GPT-5.5's price ($5/$30) — the single biggest lever for teams currently on GPT-5.5 |
| **🆕 ChatGPT Free/Go now defaults to Luna (Aug 6, 2026)** | Free/Go consumer users get unlimited text chats on GPT-5.6 Luna plus a "Think" button — a ChatGPT product change, not an API pricing change; API rates for `gpt-5.6-luna` are unchanged |
| **🆕 Cheap transcription option** | `gpt-transcribe` at $0.0045/min is now the cheapest high-accuracy transcription model in the lineup — cheaper than `gpt-4o-mini-transcribe`'s ~$0.003/min-equivalent MTok pricing for typical audio |
| **Sol vs GPT-5.5** | Same headline price ($5/$30) — pure capability upgrade, no cost penalty to move |
| **Regional processing** | +10% uplift for GPT-5.6/5.5/5.4 family data residency endpoints |
| **Fine-tuning platform** | OpenAI is winding down the fine-tuning platform — no longer accessible to new users |
| **Image models** | Migrate from `gpt-image-1.5` and `gpt-image-1-mini` to `gpt-image-2` before Dec 1, 2026 |
| **Realtime models** | Use `gpt-realtime-2.1` ($32/$64 audio) or `gpt-realtime-2.1-mini` ($10/$20 audio) — both supersede the `-2`/`-mini` names at the same price |
| **🆕 GPT-Live is not API-priced yet** | GPT-Live-1/mini (ChatGPT full-duplex voice, launched July 8, 2026) is bundled into ChatGPT plans with no separate charge and no published API rate — do not budget it as a token-priced model until OpenAI publishes Realtime-style API pricing. Still unpriced as of Aug 10, 2026. |
| **🆕 GPT-5.6 GA** | Reached general availability July 9, 2026 — no longer restricted; self-serve API access for all three tiers (Sol/Terra/Luna) |
| **Web search tool choice matters** | Non-preview web search is $10/1K calls with metered content tokens; the non-reasoning-model "preview" variant is $25/1K calls but content tokens are free — the cheaper option depends on how much search content your prompts actually consume |
| **Computer Use is a distinct SKU** | `computer-use-preview` ($1.50/$6.00) is priced independently of the underlying model family — budget it separately from GPT-5.x token costs |

---

*Sources last verified: August 10, 2026 against `developers.openai.com/api/docs/pricing`, `developers.openai.com/api/docs/models`, and `openai.com/news` (through August 7, 2026). **No API token pricing changes detected this cycle** — every price point (GPT-5.6 Sol/Terra/Luna, GPT-5.5, GPT-5.5 Pro, GPT-5.4 family, GPT-4.1 family, o3/o3-pro/o4-mini, Realtime, Image, Video, Transcription, Deep Research, Computer Use, Codex, and Tools) was independently re-checked and matches the August 3, 2026 refresh exactly. **Newly discovered (non-pricing):** an August 6, 2026 ChatGPT product update — "Improving GPT‑5.6 Sol in ChatGPT—and expanding access to GPT‑5.6 Luna for free users" — made GPT-5.6 Luna the new default model for ChatGPT Free/Go users with unlimited text chats, and refreshed GPT-5.6 Sol's tone/accuracy in the ChatGPT Chat surface. This is a consumer-product/availability change only and does not alter any API token rate. Other August 2026 OpenAI news items reviewed (Aug 7 cyber-capabilities response, Aug 6 APA partnership, Aug 4 ChatGPT Work/Codex education update, Aug 3 GPT Live continuous-voice engineering post) contain no additional pricing changes.*
