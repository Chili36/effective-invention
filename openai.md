# 🟢 OpenAI — Model Cards

> **Last updated:** 2026-09-14
> **Source:** https://developers.openai.com/api/docs/pricing · https://developers.openai.com/api/docs/models · https://developers.openai.com/api/docs/deprecations · https://openai.com/index/gpt-6-astra/ · https://openai.com/news
> **Scraped / verified:** 2026-09-14 — ✅ Re-verified all GPT-6 Astra / GPT-5.6 (Sol/Terra/Luna) pricing directly against the live `developers.openai.com/api/docs/pricing` page — **unchanged** since the Sept 7 refresh. 🆕 **GPT-Live-1 launched in the API (Sept 10, 2026)** at **$0.05/minute** for the voice layer (backend model/tools billed separately) — previously unpriced/ChatGPT-only. 🆕 **Agents API launched in public beta (Sept 10, 2026)** — no additional fees; billed at standard per-model token/tool rates. 🆕 **GPT-Image-2.5 Sunburst and Flare** discovered as the new flagship image-generation models (now carrying the pricing GPT-Image-2 used to have); **GPT-Image-2 was repriced 50% cheaper** and now sits as the value-tier active image model. 🆕 **`gpt-rosalind-research`** (Life Sciences, trusted-access) now has published pricing — billing begins **October 5, 2026**. ⚠️ **Confirmed via the official Deprecations page: `o4-mini` and `gpt-4.1-nano` are now deprecated, shutting down October 23, 2026** (→ migrate to `gpt-5.6-terra` and `gpt-5.6-luna` respectively) — moved to the Legacy section below. `o1` and `o3-mini` are also on the same Oct 23, 2026 shutdown list. Also newly deprecated: `gpt-5.4-cyber` (shuts down Oct 1, 2026 → `gpt-5.6-cyber`).

All prices are **USD per million tokens (MTok)** unless noted. Batch/Flex API gives a flat **50% discount** on all models. Cached input tokens get **50–90% off** depending on model.

> **Context tiers for GPT-6 Astra, GPT-5.6, GPT-5.5, and GPT-5.4:** Standard ("short context") pricing applies for prompts **under ~272K tokens** (GPT-6 Astra) or **~270K tokens** (GPT-5.6/5.5/5.4). The long-context tier applies a pricing surcharge above that threshold — **2× input / 1.5× output** vs. short-context rates (full request/session).

> **Service tiers:** Four processing tiers are documented — **Priority/Fast mode** (highest availability + predictable latency, 2× standard price), **Standard** (default), **Batch**, and **Flex** (async, 50% off standard).

> 🆕 **September 14, 2026 refresh — no change to GPT-6 Astra / GPT-5.6 pricing.** Independently re-fetched the live `developers.openai.com/api/docs/pricing` page. All flagship-tier prices (`gpt-6-astra`, `gpt-5.6-sol`, `gpt-5.6-terra`, `gpt-5.6-luna` — Standard/Batch/Flex/Fast-mode, short- and long-context) are byte-for-byte unchanged from the September 7 refresh. GPT-5.6 Sol's promotional pricing is confirmed still in effect, "available at least through November 21, 2026." Four other developments were found and are documented below.

> 🆕 **September 10, 2026 — GPT‑Live‑1 launched in the API.** Previously a ChatGPT-only, unpriced voice model, GPT-Live-1 is now available to developers at **$0.05 per minute** for the front-end full-duplex voice layer (billed per second, not rounded up). This does **not** include the backend reasoning model or tool costs — developers pair GPT-Live-1 with a text model (e.g., GPT-6 Astra, GPT-5.6 Terra/Luna) and pay that model's standard token rates on top. Key capabilities: single-model listen-while-speaking (no chained STT→LLM→TTS), reasoning/tool-call delegation to a backend model, tone/pace/style steering via system prompt, native turn detection despite being full-duplex, and telephony support. Full Duplex Bench improves 30 points over `gpt-realtime-2.1`; paired with GPT-6 Astra at medium reasoning effort, it ranks #1 on Tau³ (frontier voice-agent intelligence benchmark). Custom voice access requires contacting sales. See [OpenAI's announcement](https://openai.com/index/introducing-gpt-live-1-in-the-api/).

> 🆕 **September 10, 2026 — Agents API launched (public beta).** A managed service that brings the Codex harness (context compaction, tool search, programmatic/async tool calling, multi-agent subagent orchestration) to any developer via a single API call. **No additional fees** — you pay only for the tokens and tools your agents use at the standard rates on the pricing page. Choose an OpenAI-hosted sandbox or a self-hosted/partner sandbox (Blaxel, Cloudflare, Daytona, DigitalOcean, E2B, Modal, Oracle, Runloop, Vercel). This is a **harness/infrastructure product, not a separately priced model** — it can be used with any compatible model, e.g. `gpt-6-astra`. See [OpenAI's announcement](https://openai.com/index/introducing-the-agents-api/).

> 🆕 **September 2026 — GPT-Image-2.5 Sunburst and Flare identified as the new flagship image models.** OpenAI's model catalog and pricing page now list `gpt-image-2.5-sunburst` ("our most capable model for image generation and editing") and `gpt-image-2.5-flare` ("fast, high-quality everyday image generation") as the current flagship-tier image models, both priced at **$8.00/MTok image input · $2.00/MTok cached · $30.00/MTok image output · $5.00/MTok text input · $1.25/MTok cached text** — exactly the price that "GPT-Image-2" carried in the prior refresh. **GPT-Image-2 itself was repriced 50% cheaper** (now $4.00/$1.00 cached/$15.00 image; $2.50/$0.625 cached text) and is now positioned as the value-tier "All models" option rather than the flagship. GPT-Image-2 is **not deprecated** — it remains a fully active, cheaper alternative.

> ⚠️ **September 2026 — Confirmed model deprecations via the official Deprecations page (`developers.openai.com/api/docs/deprecations`):**
> - **`o4-mini`** (`o4-mini-2025-04-16`) — shuts down **October 23, 2026** → migrate to **`gpt-5.6-terra`**.
> - **`gpt-4.1-nano`** (`gpt-4.1-nano-2025-04-14`) — shuts down **October 23, 2026** → migrate to **`gpt-5.6-luna`**.
> - **`o1`** (`o1-2024-12-17`) — shuts down **October 23, 2026** → migrate to **`gpt-5.6-sol`** (previously documented migration target of "o3" is superseded by OpenAI's own recommendation).
> - **`o3-mini`** (`o3-mini-2025-01-31`) — shuts down **October 23, 2026** → migrate to **`gpt-5.6-sol`**. (Not previously tracked as a full card; noted for completeness.)
> - **`gpt-image-1`** — shuts down **October 23, 2026** → migrate to **`gpt-image-2`**.
> - **`gpt-5.4-cyber`** — deprecated Sept 11, 2026, shuts down **October 1, 2026** → migrate to **`gpt-5.6-cyber`**.
> - `gpt-3.5-turbo-0125`/`gpt-4-0613`/`gpt-4-1106-preview`/`gpt-4-turbo`/`gpt-4o-2024-05-13` also shut down Oct 23, 2026 (already tracked as RETIRED below).
> - `o4-mini` and `gpt-4.1-nano` have been **moved from Active to the Legacy/Deprecated section** below; their original card fields are preserved with a deprecation notice.
>
> 🆕 **September 10, 2026 — `gpt-rosalind-research` (Life Sciences, trusted access) pricing published.** $5.00 input / $0.50 cached input / $25.00 output per MTok. Billing begins **October 5, 2026**; cache-write pricing does not apply. Access limited to approved internal research through OpenAI's trusted-access program for life-sciences researchers. See card below.

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
| **Tools** | Web search, file search, image generation, code interpreter, hosted shell, apply patch, skills, computer use, MCP, tool search — full Responses API toolset; also usable as the backend model behind GPT-Live-1 and via the new Agents API |
| **Rate limits (RPM / TPM)** | Free: not supported · Tier 1: 500 / 500K · Tier 2: 5,000 / 1M · Tier 3: 5,000 / 2M · Tier 4: 10,000 / 4M · Tier 5: 15,000 / 40M |
| **Availability** | ChatGPT Plus/Pro/Business/Enterprise · GPT-6 Astra Pro (Pro/Business/Enterprise) · OpenAI API · Microsoft Azure/Foundry · AWS Bedrock |
| **Notable** | New async tool calling, mid-turn steering, and mid-conversation `configuration_update` reasoning-effort changes (cache-prefix preserving); first model with default-on misalignment monitoring; uses a "recurrent depth"/"looped transformers" reasoning technique that OpenAI's own system card flags as reducing chain-of-thought monitorability under adversarial conditions; pairs with GPT-Live-1 as the reasoning backend for full-duplex voice agents |

> 🔗 Source: [openai.com/index/gpt-6-astra](https://openai.com/index/gpt-6-astra/) · [deploymentsafety.openai.com/gpt-6-astra](https://deploymentsafety.openai.com/gpt-6-astra) (system card) · `developers.openai.com/api/docs/pricing` (re-verified September 14, 2026 — unchanged)

---

### GPT-5.6 — Sol / Terra / Luna *(🔄 Sol replaced by GPT-6 Astra as flagship — family still fully active; Sol now promotionally priced)*

> **GPT-5.6 reached General Availability on July 9, 2026** and remains fully active. As of **September 3, 2026**, GPT-6 Astra has replaced **GPT-5.6 Sol** as OpenAI's recommended flagship, and Sol's price was cut to promotional levels (at least through November 21, 2026). Terra and Luna are unaffected and remain the recommended balanced/budget tiers. ✅ Re-verified September 14, 2026 — all Sol/Terra/Luna prices below are unchanged.

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
- Usable as the reasoning/tool-calling backend behind **GPT-Live-1** voice sessions and via the **Agents API**.

**Availability by plan:**
| Surface | Access |
|---|---|
| ChatGPT Plus / Pro / Business / Enterprise | Sol via medium+ reasoning effort (now secondary to GPT-6 Astra as flagship) |
| ChatGPT Free / Go | Luna (default since Aug 6, 2026 — unlimited text chats, "Think" button) |
| ChatGPT Work & Codex | Choice of Sol, Terra, or Luna with configurable effort |
| API | Self-serve — Sol, Terra, and Luna all reachable directly |

**Notable:** GPT-5.6 Sol still holds strong benchmark standing (e.g., DeepSWE v1.1 72.7%, OSWorld 2.0 65.7%) and, at its new **$4.00/$20.00** promotional price, is now meaningfully cheaper than before while GPT-6 Astra takes over as the premium/flagship option at $10.00/$50.00. **Terra remains the price/performance story of the release** at less than a fifth of Astra's price. Luna covers high-volume classification/extraction/tagging work at the bottom of the ladder and is also the default model powering ChatGPT's free tier.

> 🔗 Source: [openai.com/index/gpt-5-6/](https://openai.com/index/gpt-5-6/) · `developers.openai.com/api/docs/pricing` (re-verified September 14, 2026 — unchanged)

---

### 🆕 GPT-5.6 Cyber *(Daybreak Program — Pricing Published September 3, 2026)*

> Part of OpenAI's **Daybreak** cybersecurity program for authorized vulnerability research and security testing. Previously unpriced (`gpt-5.4-cyber` had no public rate); the current generation `gpt-5.6-cyber` now has documented pricing. ⚠️ `gpt-5.4-cyber` itself was deprecated September 11, 2026 and shuts down October 1, 2026 — migrate to `gpt-5.6-cyber`.

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
| **Notable** | Most advanced OpenAI cybersecurity model prior to GPT-6 Astra's Critical-tier capabilities; the Daybreak aliases will be repointed to newer underlying models (and pricing adjusted) as the program evolves. Predecessor `gpt-5.4-cyber` shuts down October 1, 2026 |

---

### 🆕 GPT-Rosalind (Research) *(Life Sciences — Trusted Access — Pricing Published September 10, 2026)*

> A specialized model for approved life-sciences research organizations, powering tools like the "Rosalind Workbench." Billing begins **October 5, 2026**; before that date usage is not charged. Access is limited to approved internal research through OpenAI's trusted-access program — all eligible organizations continue to get access to the latest GPT-Rosalind models as they're released.

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-rosalind-research` |
| **Status** | ✅ Active — Trusted access only; billing starts Oct 5, 2026 |
| **Input price** | $5.00 / MTok |
| **Cached input** | $0.50 / MTok |
| **Output price** | $25.00 / MTok |
| **Cache write** | Not applicable — cache-write pricing does not apply to this model |
| **Regional processing** | +10% uplift (eligible endpoints) |
| **Availability** | Trusted-access program for approved life-sciences research organizations only |
| **Notable** | Sibling product to "Rosalind Workbench," aimed at letting scientists run their own research teams with AI assistance |

---

### GPT-5.5 *(still fully active, same price)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.5` |
| **Released** | April 23, 2026 (ChatGPT/Codex) · April 24, 2026 (API) |
| **Status** | ✅ Active — no longer the current flagship (superseded first by GPT-5.6 Sol, now by GPT-6 Astra), but fully supported and unchanged in price. Confirmed still listed with its own model page on `developers.openai.com/api/docs/models/gpt-5.5` as of Sept 14, 2026 refresh |
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
| **Notable** | Cheapest proprietary model in the GPT-5.4 family; GPT-5.6 Luna is priced almost identically on input but marginally cheaper on output. Do not confuse with the now-deprecated **GPT-4.1 nano** (see Legacy section) |

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
| **Notable** | 1M context at lower cost than GPT-5.4; better instruction-following and coding vs GPT-4o. Not on the current deprecation list (unlike its `gpt-4.1-nano` sibling — see Legacy) |

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
| **Notable** | Chain-of-thought reasoning; best for math, logic, multi-step coding. Not on the current deprecation list |

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

## 🎙️ Multimodal, Realtime & Specialized Models

### 🆕 GPT-Live-1 *(Full-Duplex Voice — Now Priced in the API — September 10, 2026)*

> **Status update:** GPT-Live-1 was ChatGPT-only and unpriced as of the last refresh. As of **September 10, 2026**, it is available directly in the API with published pricing.

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-live-1` |
| **Status** | ✅ Active — **Now available in the API with published pricing** |
| **Price** | **$0.05 per minute**, billed per second (not rounded up to a whole minute) |
| **What's included** | Front-end full-duplex voice layer only — listening + speaking, interruption handling, turn detection, telephony support |
| **What's billed separately** | Backend reasoning/tool-calling model (e.g., GPT-6 Astra, GPT-5.6 Terra/Luna) at that model's standard token rates, plus any tool usage |
| **Availability** | API (`v1/live/sessions`) · ChatGPT (where it originally launched) · custom voice access via sales contact |
| **Notable** | Full Duplex Bench +30 points vs. `gpt-realtime-2.1`; #1 on Tau³ when paired with GPT-6 Astra (medium reasoning); simplifies voice-agent architecture vs. chained STT→LLM→TTS designs; new expanded voice roster (Quartz, Ripple, Vesper, Willow, Stone, Gleam, Meridian, Bossa, Tempo, Beacon, Delta, Cinder) |
| **GPT-Live-1 mini** | Referenced in ChatGPT contexts; **not yet confirmed with its own published API price** as of this refresh |

> 🔗 Source: [openai.com/index/introducing-gpt-live-1-in-the-api](https://openai.com/index/introducing-gpt-live-1-in-the-api/) · `developers.openai.com/api/docs/pricing`

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

### 🆕 GPT-Image-2.5 Sunburst / Flare *(New Flagship Image Models)*

> Discovered on the current model catalog/pricing page as OpenAI's flagship image-generation models, carrying the pricing that "GPT-Image-2" used to have. Sunburst is described as "our most capable model for image generation and editing"; Flare is "fast, high-quality everyday image generation."

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Image** (both models) | $8.00 / MTok | $2.00 / MTok | $30.00 / MTok |
| **Text** (both models) | $5.00 / MTok | $1.25 / MTok | — |

| Field | Value |
|---|---|
| **Model IDs** | `gpt-image-2.5-sunburst` · `gpt-image-2.5-flare` |
| **Status** | ✅ Active — **New flagship image-generation tier** |
| **Notable** | Same pricing structure GPT-Image-2 previously carried; GPT-Image-2 itself was repriced 50% cheaper and demoted to the value tier (see below) |

---

### GPT-Image-2 *(Repriced — Now Value Tier, Not Flagship)*

> 📉 **Repriced 50% cheaper** and moved from the flagship tier to the "All models" value tier now that GPT-Image-2.5 Sunburst/Flare have launched. **Not deprecated** — still a fully active, cheaper image option.

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Image** | $4.00 / MTok *(was $8.00)* | $1.00 / MTok *(was $2.00)* | $15.00 / MTok *(was $30.00)* |
| **Text** | $2.50 / MTok *(was $5.00)* | $0.625 / MTok *(was $1.25)* | — |

> Batch pricing (legacy figures, likely also halved — verify at time of use): Image input $4.00, cached $1.00, output $15.00 per MTok; Text input $2.50, cached $0.625 *(these were the old Standard rates; a corresponding Batch discount table for the repriced GPT-Image-2 was not separately itemized on this refresh's pricing page — Batch is 50% of Standard as with other models)*.

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
| `gpt-4o-transcribe` | $2.50 / MTok input · $10.00 / MTok output (~$0.006 / min) | ⚠️ Deprecated Aug 26, 2026 — shuts down Feb 26, 2027 → `gpt-live-transcribe` or `gpt-transcribe` |
| `gpt-4o-mini-transcribe` | $1.25 / MTok input · $5.00 / MTok output (~$0.003 / min) | ⚠️ Deprecated Aug 26, 2026 — shuts down Feb 26, 2027 → `gpt-live-transcribe` or `gpt-transcribe` |
| `whisper-1` | Legacy | ⚠️ Deprecated Aug 26, 2026 — shuts down Feb 26, 2027 → `gpt-live-transcribe` or `gpt-transcribe` |

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
| 🆕 `gpt-rosalind-research` (Life Sciences, trusted access) | $5.00 / MTok | $0.50 / MTok | — | $25.00 / MTok | — |

---

## 🤖 Agents API *(🆕 Public Beta — September 10, 2026)*

> Brings the Codex harness (context compaction, tool search, programmatic/async tool calling, multi-agent subagent orchestration) to any developer via a single managed API call. **No separate fees** — billed entirely at standard per-model token and tool rates from the pricing tables above.

| Field | Value |
|---|---|
| **Status** | 🆕 Public beta (Sept 10, 2026) |
| **Pricing** | No additional fees; standard token/tool pricing applies for the model and tools used |
| **Environments** | OpenAI-hosted sandbox, or self-hosted/partner sandboxes (Blaxel, Cloudflare, Daytona, DigitalOcean, E2B, Modal, Oracle, Runloop, Vercel) |
| **Key features** | Automatic context compaction across long sessions, tool search (loads tool defs on demand to save tokens/preserve cache), programmatic tool calling (parallel/chained calls), multi-agent subagent orchestration |
| **Foundation** | Open-source Codex harness (github.com/openai/codex) |
| **Notable** | Reported customer results include a 0.71→0.85 eval-score improvement with 4× latency reduction on subagent workflows, 86% fewer failed agent responses from sandbox/harness separation, and 60% cost-per-case reduction after migration |

> 🔗 Source: [openai.com/index/introducing-the-agents-api](https://openai.com/index/introducing-the-agents-api/)

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
| 🆕 **GPT-Live-1 voice sessions** | Front-end voice layer, billed per second | $0.05 / minute |
| 🆕 **Agents API** | Managed Codex-harness agents | No additional fee — standard token/tool rates apply |

---

## 💰 Fine-tuning *(platform winding down)*

> OpenAI is winding down the fine-tuning platform — no longer accessible to new users. Existing users can create training jobs for a limited period; fine-tuned models remain available for inference until base models are deprecated.

| Model | Training | Input | Cached Input | Output |
|---|---|---|---|---|
| `o4-mini-2025-04-16` | $100.00 / hour | $4.00 / MTok | $1.00 / MTok | $16.00 / MTok |
| `o4-mini-2025-04-16` (data sharing) | $100.00 / hour | $2.00 / MTok | $0.50 / MTok | $8.00 / MTok |

> ⚠️ Note: the base `o4-mini` model used for inference (non-fine-tuning) is now **deprecated**, shutting down October 23, 2026 — see Legacy section. Fine-tuned `o4-mini` variants remain available for inference until the base model is deprecated per OpenAI's fine-tuning policy.

---

## ⚠️ Legacy / Deprecated / Retired Models

### ⚠️ DEPRECATED — o4-mini *(🆕 Confirmed shutdown October 23, 2026)*

> **Moved from Active to Legacy this refresh.** Confirmed via the official `developers.openai.com/api/docs/deprecations` page: `o4-mini` (`o4-mini-2025-04-16`) is deprecated and will shut down **October 23, 2026**.

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `o4-mini` (`o4-mini-2025-04-16`) |
| **Status** | ⚠️ DEPRECATED — **Shuts down October 23, 2026** |
| **Input price** | $1.10 / MTok |
| **Cached input** | $0.275 / MTok |
| **Output price** | $4.40 / MTok |
| **Context window** | 200,000 tokens |
| **Migration** | → **`gpt-5.6-terra`** (OpenAI's official recommended replacement) |

---

### ⚠️ DEPRECATED — GPT-4.1 nano *(🆕 Confirmed shutdown October 23, 2026)*

> **Moved from Active to Legacy this refresh.** Confirmed via the official `developers.openai.com/api/docs/deprecations` page: `gpt-4.1-nano` (`gpt-4.1-nano-2025-04-14`) is deprecated and will shut down **October 23, 2026**. Note: this is distinct from `gpt-5.4-nano`, which is not affected.

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4.1-nano` (`gpt-4.1-nano-2025-04-14`) |
| **Status** | ⚠️ DEPRECATED — **Shuts down October 23, 2026** |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.40 / MTok |
| **Context window** | 1M+ tokens |
| **Migration** | → **`gpt-5.6-luna`** (OpenAI's official recommended replacement) |

---

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

### ⚠️ DEPRECATED — GPT-Realtime (legacy family) and GPT-Audio family *(🆕 shuts down Jan 20, 2027)*

> Confirmed via the Deprecations page (notice issued July 20, 2026): `gpt-realtime`, `gpt-audio`, `gpt-4o-audio`, `gpt-4o-realtime`, `gpt-realtime-mini`, `gpt-audio-mini`, `gpt-4o-mini-realtime`, `gpt-4o-mini-audio` all shut down **January 20, 2027** → migrate to `gpt-realtime-2.1`, `gpt-realtime-2.1-mini`, or `gpt-audio-1.5` as applicable.

---

### ⚠️ DEPRECATED — o1 *(🆕 Confirmed shutdown October 23, 2026 — migration target corrected)*

| Field | Value |
|---|---|
| **Model ID** | `o1` (`o1-2024-12-17`) |
| **Status** | ⚠️ DEPRECATED — **Shuts down October 23, 2026** (confirmed via official Deprecations page) |
| **Input price** | $15.00 / MTok |
| **Output price** | $60.00 / MTok |
| **Migration** | → **`gpt-5.6-sol`** *(OpenAI's official recommended replacement — corrects the previous "o3/o3-pro" migration note)* |

---

### ⚠️ DEPRECATED — o3-mini *(🆕 Confirmed shutdown October 23, 2026 — newly tracked)*

| Field | Value |
|---|---|
| **Model ID** | `o3-mini` (`o3-mini-2025-01-31`) |
| **Status** | ⚠️ DEPRECATED — **Shuts down October 23, 2026** |
| **Migration** | → **`gpt-5.6-sol`** |
| **Notable** | Not previously tracked as a full card in this repo; added for completeness given the confirmed shutdown date |

---

### ⚠️ DEPRECATED — gpt-image-1 *(🆕 Confirmed shutdown October 23, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-image-1` |
| **Status** | ⚠️ DEPRECATED — **Shuts down October 23, 2026** |
| **Migration** | → **`gpt-image-2`** (now repriced 50% cheaper — see Active section) |

---

### ⚠️ DEPRECATED — GPT-4o Transcribe family *(shuts down Feb 26, 2027)*

| Model | Status | Migration |
|---|---|---|
| `whisper-1` | ⚠️ Deprecated Aug 26, 2026 | → `gpt-live-transcribe` or `gpt-transcribe` |
| `gpt-4o-transcribe` | ⚠️ Deprecated Aug 26, 2026 | → `gpt-live-transcribe` or `gpt-transcribe` |
| `gpt-4o-mini-transcribe` | ⚠️ Deprecated Aug 26, 2026 | → `gpt-live-transcribe` or `gpt-transcribe` |
| `gpt-4o-transcribe-diarize` | ⚠️ Deprecated Aug 26, 2026 | → `gpt-live-transcribe` or `gpt-transcribe` |

> All four shut down **February 26, 2027**.

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

### ⚠️ DEPRECATED — gpt-5.4-cyber *(🆕 shuts down October 1, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.4-cyber` |
| **Status** | ⚠️ DEPRECATED — Notice issued Sept 11, 2026; shuts down **October 1, 2026** |
| **Migration** | → **`gpt-5.6-cyber`** |

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
| **Status** | ⚠️ LEGACY — **All GPT-5.2 models retired from ChatGPT June 12, 2026 ❌** · GPT-5.2 Thinking variant RETIRED API June 5, 2026 · `gpt-5.2-chat-latest` shut down Aug 10, 2026 |
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
| **Status** | ⚠️ LEGACY — Superseded by GPT-4.1. Dated snapshot `gpt-4o-2024-05-13` confirmed shutting down October 23, 2026 |
| **Input price** | $2.50 / MTok |
| **Output price** | $10.00 / MTok |
| **Migration** | → **GPT-4.1** ($2/$8, 1M context) or **GPT-5.6 Sol** |

---

### ⚠️ LEGACY — GPT-4o mini

| Field | Value |
|---|---|
| **Model ID** | `gpt-4o-mini` |
| **Status** | ⚠️ LEGACY |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.60 / MTok |
| **Migration** | → **GPT-5.6 Luna** ($0.20/$1.20) or **GPT-4.1 nano** *(also now deprecated — see above)* |

---

### ⚠️ LEGACY — o1-pro *(Deep Reasoning, dated snapshot deprecated Oct 23, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `o1-pro` (`o1-pro-2025-03-19`) |
| **Status** | ⚠️ DEPRECATED — Shuts down **October 23, 2026** |
| **Migration** | → **`gpt-5.6-sol`** (`reasoning.mode: pro`) |

---

### ⚠️ LEGACY — GPT-4 Turbo / GPT-3.5 Turbo / GPT-4-0613 *(RETIRED / shutting down Oct 23, 2026)*

| Model | Status |
|---|---|
| GPT-4 Turbo (`gpt-4-turbo`, `gpt-4-turbo-2024-04-09`) | ⚠️ Shuts down October 23, 2026 → `gpt-5.6-sol` |
| GPT-4 (`gpt-4-0613`) | ⚠️ Shuts down October 23, 2026 → `gpt-5.6-sol` |
| `gpt-4-1106-preview` | ⚠️ Shuts down October 23, 2026 → `gpt-5.6-sol` |
| GPT-3.5 Turbo (`gpt-3.5-turbo-0125`) | ⚠️ Shuts down October 23, 2026 → `gpt-5.6-terra` |
| `gpt-3.5-turbo-instruct`, `babbage-002`, `davinci-002`, `gpt-3.5-turbo-1106` | ⚠️ Shuts down September 28, 2026 → `gpt-5.6-terra` |

---

## 💡 Cost Optimization Notes

| Feature | Savings |
|---|---|
| **Batch/Flex API** | 50% off all tokens (24 hr turnaround) |
| **Cached input tokens** | 50–90% off depending on model |
| **🆕 GPT-6 Astra is the new premium ceiling** | $10.00/$50.00 (short ctx) — 2.5× GPT-5.6 Sol's new promotional rate. OpenAI argues it finishes tasks in fewer tokens/retries, potentially lowering effective cost-per-task despite the higher per-token price — budget carefully and benchmark on your own workloads |
| **📉 GPT-5.6 Sol promotional pricing** | Cut from $5.00/$30.00 to **$4.00/$20.00** (short ctx) — available at least through November 21, 2026. Now the cheapest way to access "flagship-class" GPT-5.6 |
| **GPT-5.6 / GPT-5.5 / GPT-6 Astra long-context** | Stay under ~270–272K input tokens to avoid the 2× input / 1.5× output surcharge |
| **🆕 gpt-5.6-cyber now priced** | $12.50/$75.00 (short ctx only) — previously unpriced; part of the Daybreak vetted-access cybersecurity program. Its predecessor `gpt-5.4-cyber` shuts down Oct 1, 2026 |
| **🆕 Terra remains the best GPT-5.5 replacement** | GPT-5.6 Terra at $2.00/$12.00 — under half GPT-5.5's price ($5/$30) and a fifth of GPT-6 Astra's; now also the official migration target for the deprecated `o4-mini` |
| **⚠️ o4-mini and GPT-4.1 nano are now deprecated** | Both shut down **October 23, 2026** — migrate to `gpt-5.6-terra` and `gpt-5.6-luna` respectively well ahead of the deadline |
| **⚠️ o1, o3-mini, o1-pro, gpt-image-1 also shut down Oct 23, 2026** | Migrate to `gpt-5.6-sol` (o-series) or `gpt-image-2` (image) |
| **ChatGPT Free/Go defaults to Luna** | Free/Go consumer users get unlimited text chats on GPT-5.6 Luna plus a "Think" button — a ChatGPT product change, not an API pricing change |
| **Cheap transcription option** | `gpt-transcribe` at $0.0045/min is the cheapest high-accuracy transcription model in the lineup; note `gpt-4o-transcribe`/`gpt-4o-mini-transcribe`/`whisper-1` are now deprecated (shut down Feb 26, 2027) |
| **Regional processing** | +10% uplift for GPT-6 Astra/5.6/5.5/5.4 family data residency endpoints |
| **GPT-6 Astra Fast mode caveat** | Unavailable with EU data residency; no latency SLA even where available |
| **Fine-tuning platform** | OpenAI is winding down the fine-tuning platform — no longer accessible to new users |
| **🆕 Image models: two tiers now** | `gpt-image-2.5-sunburst`/`flare` are the new flagship ($8/$2/$30 image); `gpt-image-2` was repriced 50% cheaper ($4/$1/$15 image) and is now the value tier. Migrate off `gpt-image-1`, `gpt-image-1.5`, `gpt-image-1-mini`, and `chatgpt-image-latest` (all shutting down by Dec 1, 2026 at the latest) |
| **Realtime models** | Use `gpt-realtime-2.1` ($32/$64 audio) or `gpt-realtime-2.1-mini` ($10/$20 audio); the whole prior-generation Realtime/Audio family (`gpt-realtime`, `gpt-audio`, `gpt-4o-realtime`, etc.) shuts down Jan 20, 2027 |
| **🆕 GPT-Live-1 is now API-priced** | $0.05/minute for the voice layer (Sept 10, 2026) — pair with a text model for reasoning/tools, billed separately at that model's rates |
| **🆕 Agents API is free to adopt** | Public beta (Sept 10, 2026) — no separate fee, just standard token/tool costs, for a managed Codex-harness agent runtime |
| **Web search tool choice matters** | Non-preview web search is $10/1K calls with metered content tokens; the non-reasoning-model "preview" variant is $25/1K calls but content tokens are free |
| **Computer Use is a distinct SKU** | `computer-use-preview` ($1.50/$6.00) is priced independently of the underlying model family |

---

*Sources last verified: September 14, 2026 against `developers.openai.com/api/docs/pricing`, `developers.openai.com/api/docs/models`, `developers.openai.com/api/docs/deprecations`, `developers.openai.com/api/docs/models/gpt-5.5`, `openai.com/news`, and the GPT-Live-1 / Agents API launch posts. **Major updates this cycle:** (1) GPT-Live-1 launched in the API at $0.05/minute (Sept 10); (2) the new Agents API launched in public beta with no added fees (Sept 10); (3) GPT-Image-2.5 Sunburst/Flare identified as the new flagship image models, with GPT-Image-2 repriced 50% cheaper as the value tier; (4) `gpt-rosalind-research` (Life Sciences) gained published pricing, billing from Oct 5, 2026; (5) confirmed via the official Deprecations page that `o4-mini` and `gpt-4.1-nano` are deprecated and shut down October 23, 2026 (moved to Legacy, with `o1`, `o3-mini`, `o1-pro`, and `gpt-image-1` on the same shutdown date), and that `gpt-5.4-cyber` shuts down October 1, 2026. GPT-6 Astra and the full GPT-5.6 (Sol/Terra/Luna) pricing tables were independently re-verified and are unchanged since Sept 7. GPT-5.5, GPT-5.5 Pro, GPT-5.4 family, GPT-4.1/mini, o3/o3-pro were individually spot-checked (via `gpt-5.5`'s dedicated model page) and confirmed still active and unchanged — they simply do not appear in the redesigned pricing page's default "Flagship models" view.*
