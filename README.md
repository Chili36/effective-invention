# 🤖 LLM Pricing Tracker

Up-to-date pricing and specifications for large language models from **Anthropic**, **OpenAI**, **Google Gemini**, **Mistral AI**, and top **OpenRouter picks**.

> **Last updated:** 2026-06-08 (refresh #18)
> **Sources:** Official provider pricing pages + third-party verification — scraped/verified on date above.

---

## 📋 Quick-Reference Index — Active Models

### 🟠 Tier 1 — Anthropic Claude

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Max Output | Availability |
|---|---|---|---|---|---|
| **Claude Opus 4.8** *(Current Flagship)* | $5.00 | $25.00 | **1M tokens** | 128k sync / 300k Batch | API, AWS Bedrock (Messages API), Vertex AI, MS Foundry (200k ctx) |
| **Claude Sonnet 4.6** | $3.00 | $15.00 | **1M tokens** | 64k sync / 300k Batch | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Haiku 4.5** | $1.00 | $5.00 | 200K tokens | 64k | API, AWS Bedrock (all regions), Vertex AI, MS Foundry |

> 💡 Batch API: 50% off · Prompt caching: up to 90% off
> ⚡ **Opus 4.8 Fast Mode:** $10/$50 per MTok (2× standard) — up to 2.5× faster speeds
> ⚡ **Opus 4.6 / Opus 4.7 Fast Mode (Legacy):** $30/$150 per MTok (6× standard) — prefer Opus 4.8 Fast Mode for cost efficiency
> 🧠 **Thinking:** Opus 4.8 = Adaptive only · Sonnet 4.6 = Adaptive + Extended · Haiku 4.5 = Extended only
> 🔒 Claude Mythos Preview (Project Glasswing) — restricted access only; no public API; general release expected per May 28 announcement
> 🚨 **URGENT: Claude Sonnet 4 + Opus 4 retiring June 15, 2026 (7 DAYS AWAY)** — migrate to Sonnet 4.6 / Opus 4.8 immediately

---

### 🟢 Tier 1 — OpenAI (Proprietary)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|---|
| **GPT-5.5** *(Current Flagship)* | $5.00 / $10.00* | $0.50 | $30.00 / $45.00* | **1.05M tokens** | API |
| **GPT-5.5 Pro** | $30.00 | — | $180.00 | 1M tokens | API |
| GPT-5.4 *(prev flagship)* | $2.50 / $5.00† | $0.25 / $0.50† | $15.00 / $22.50† | 1.05M tokens | API |
| GPT-5.4 Pro *(prev ultra-premium)* | $30.00 | — | $180.00 | 1.05M tokens | API |
| **GPT-5.4 mini** | $0.75 | $0.075 | $4.50 | 400K tokens | API |
| **GPT-5.4 nano** | $0.20 | $0.020 | $1.25 | 400K tokens | API |
| GPT-4.1 | $2.00 | $0.50 | $8.00 | 1.04M tokens | API |
| **GPT-4.1 mini** | $0.40 | $0.10 | $1.60 | 1.00M tokens | API |
| GPT-4.1 nano | $0.10 | — | $0.40 | 1M+ tokens | API |
| o3 *(reasoning)* | $2.00 | $0.50 | $8.00 | 200K tokens | API |
| o3-pro *(reasoning)* | $20.00 | — | $80.00 | 200K tokens | API |
| o4-mini *(reasoning)* | $1.10 | $0.275 | $4.40 | 200K tokens | API |

> 💡 Batch/Flex API: 50% off all models · Cached inputs: 50–90% off · Regional processing: +10% on GPT-5.5 and GPT-5.4 family
> **Priority tier (GPT-5.5 std):** $12.50 input / $75.00 output per MTok (2.5× standard)
> *GPT-5.5 long-context pricing (>272K tokens): **2× input ($10.00) / 1.5× output ($45.00)** for the full session — plan context budgets accordingly
> †GPT-5.4 tiered pricing: short ctx (<272K) / long ctx (>272K) — standard rates below 272K
> 🔒 GPT-5.4-Cyber — limited vetted access only; no public API pricing

---

### 🔵 Tier 1 — Google Gemini

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Notes |
|---|---|---|---|---|
| **Gemini 3.5 Flash** 🆕 *(New Flagship — May 19, 2026)* | $1.50 | $9.00 | **1M tokens** | GA Stable; thinking supported; fastest frontier model |
| **Gemini 3.1 Pro Preview** | $2.00 / $4.00* | $12.00 / $18.00* | **1M tokens** | *Tiered at >200K; Preview |
| **Gemini 3.1 Flash-Lite** 🆕 *(Stable GA)* | $0.25 | $1.50 | **1M tokens** | GA Stable (May 2026); thinking supported |
| **Gemini 3.1 Flash-Lite Preview** | $0.25 | $1.50 | **1M tokens** | Preview |
| **Gemini 2.5 Pro** | $1.25 / $2.50* | $10.00 / $15.00* | **1M tokens** | *Tiered at >200K; GA |
| **Gemini 2.5 Flash** | $0.30 | $2.50 | **1M tokens** | GA; optional thinking mode |
| **Gemini 2.5 Flash-Lite** | $0.10 | $0.40 | **1M tokens** | GA; cheapest Gemini |
| ~~Gemini 2.0 Flash~~ ⚠️ | $0.10 | $0.40 | 1M tokens | ⚠️ **DEPRECATED — Shutdown June 1, 2026** |

> 💡 Batch API: 50% off · Context caching: 90% off repeated prefixes · Free tier via AI Studio · Pro models: double input cost for prompts >200K
> 🆕 **Gemini 3.5 Flash** (May 19, 2026): New stable GA flagship; outperforms Gemini 3.1 Pro on agentic/coding benchmarks at a lower price ($1.50 vs $2.00 input); 4× faster
> ⚠️ **Gemini 2.0 Flash DEPRECATED** — official shutdown **June 1, 2026**. Migrate to 2.5 Flash or 3.5 Flash

---

### 🟡 Tier 1 — Mistral AI

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Mistral Medium 3.5** 🆕 *(Apr 29, 2026)* | $1.50 | $7.50 | 256K tokens | API (Mistral AI Studio) |
| **Mistral Large 3 (2512)** | $0.50 | $1.50 | 256K tokens | API (Mistral AI Studio) |
| **Magistral Medium 1.2** | $2.00 | $5.00 | 128K tokens *(best <40K)* | API (Mistral AI Studio) |
| Magistral Small *(latest alias)* | $0.50 | $1.50 | 128K tokens | API (Mistral AI Studio) |
| Mistral Medium 3.1 *(removed from pricing page June 8)* | $0.40 | $2.00 | 131K tokens | API (verify availability) |
| **Mistral Small 4** *(Mar 2026)* | $0.10 | $0.30 | **256K tokens** | API (Mistral AI Studio) |
| Codestral 2508 | $0.30 | $0.90 | 256K tokens | API (Mistral AI Studio) |
| **Devstral 2 (2512)** | $0.40 | $2.00 | 256K tokens | API (Mistral AI Studio) |
| **Devstral Small 2** | $0.10 | $0.30 | **256K tokens** | API (Mistral AI Studio) |
| Voxtral Small 24B | $0.004/min (audio) | $0.40 | 128K tokens | API (Mistral AI Studio) |
| **Voxtral Mini** *(3B)* | $0.001/min (audio) / $0.04 (text) | $0.04 | 32K tokens | API (Mistral AI Studio) |
| **Voxtral Mini Transcribe** | $0.002/min | — | — | API (Mistral AI Studio) |
| Voxtral TTS | $0.016/1K chars | — | — | API (Mistral AI Studio) |
| 🆕 **OCR 3** *(Premier)* | $2.00/1K pages | $3.00/1K pages (annot.) | — | API (Mistral AI Studio) |
| 🆕 **Codestral Embed** *(Premier)* | $0.15 (input only) | — | — | API (Mistral AI Studio) |
| 🆕 **Mistral Embed** | $0.10 (input only) | — | — | API (Mistral AI Studio) |
| 🆕 **Mistral Moderation** | $0.10 (input only) | — | — | API (Mistral AI Studio) |
| 🆕 **Leanstral** *(Labs, Free)* | Free | Free | — | API (Mistral AI Studio) |
| 🆕 **Mistral Small Creative** *(Labs)* | $0.10 | $0.30 | ~128K tokens | API (Mistral AI Studio) |
| Mistral Nemo | $0.15 | $0.15 | 128K tokens | API (Mistral AI Studio) |
| Ministral 3 14B | $0.20 | $0.20 | 256K tokens | API (Mistral AI Studio) |
| Ministral 3 8B | $0.15 | $0.15 | 256K tokens | API (Mistral AI Studio) |
| Ministral 3 3B | $0.10 | $0.10 | 556K tokens | API (Mistral AI Studio) |
| Mixtral 8x22B *(legacy API)* | $2.00 | $6.00 | 64K tokens | API (Mistral AI Studio) |
| Mixtral 8x7B *(legacy API)* | $0.70 | $0.70 | 32K tokens | API (Mistral AI Studio) |

> 💡 Batch API: 50% off (confirmed) · EU data residency by default · Open-weight models (Apache 2.0/modified MIT) for self-hosting
> 🆕 **Mistral Medium 3.5** (Apr 29, 2026) — 128B dense flagship; $1.50/$7.50; 256K ctx; vision + configurable reasoning + coding in one model
> 🆕 **Leanstral** (Labs) — Free; first open-source code agent for Lean 4 formal proof engineering
> 🆕 **Mistral Small Creative** (Labs) — $0.10/$0.30; fine-tuned for creative writing, roleplay, chat
> 🆕 **OCR 3** (Premier) — $2.00/1K pages + $3.00/1K annotation pages; best-in-class document extraction
> ⚠️ **Mistral Medium 3.1 removed from mistral.ai/pricing** (June 8) — still in docs but verify accessibility before building new workloads

---

### 🟣 Tier 2 — OpenRouter Picks (One Best Model Per Provider)

| Provider | Model | Input ($/MTok) | Output ($/MTok) | Context Window |
|---|---|---|---|---|
| **OpenAI open-weight** | gpt-oss-120b | $0.039 | $0.190 | 131K tokens |
| **DeepSeek** | DeepSeek V3.2 | $0.26 | $0.38 | 163K tokens |
| **Qwen (Alibaba)** | Qwen3.6 Plus | Free (preview)* | Free (preview)* | **1M tokens** |
| **Nvidia** | Nemotron 3 Super 120B | $0.10 | $0.50 | 262K tokens |
| **MiniMax** | MiniMax M2.7 | $0.30 | $1.20 | 205K tokens |
| **xAI (Grok)** | Grok 4.1 Fast | $0.20 | $0.50 | **2M tokens** |

> 💡 *Qwen3.6 Plus free preview ended ~April 7, 2026. Paid pricing TBD. Fallback: Qwen3.5 Plus at $0.26/$1.56.

---

## 📁 Model Card Files

| Provider | Tier | File | Description |
|---|---|---|---|
| Anthropic | 1 | [anthropic.md](./anthropic.md) | Full model cards incl. Opus 4.8 (flagship), Sonnet 4.6, Haiku 4.5; Fast Mode correction for Opus 4.7; June 15 retirement urgency |
| OpenAI | 1 | [openai.md](./openai.md) | Full model cards incl. GPT-5.5 Priority tier, reasoning models; GPT-5.2 Thinking RETIRED June 5, 2026 |
| Google Gemini | 1 | [gemini.md](./gemini.md) | Full model cards incl. Gemini 3.5 Flash (new flagship), 3.1 Flash-Lite stable GA, 2.0 Flash deprecation |
| Mistral AI | 1 | [mistral.md](./mistral.md) | Full model cards incl. 6 new models (Leanstral, Small Creative, OCR 3, Codestral Embed, Mistral Embed, Moderation); Medium 3.1 pricing page removal note |
| OpenRouter Picks | 2 | [openrouter-picks.md](./openrouter-picks.md) | One best-performing model per Tier 2 provider, all via OpenRouter |

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new deployments.

### 🟠 Anthropic — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ Claude Opus 4.7 | **LEGACY** · Moved to Legacy section (May 28, 2026); still API-accessible; Fast Mode available at $30/$150 (6× — same as 4.6) | $5.00 | $25.00 | → Claude Opus 4.8 (same price, improved performance, cheaper Fast Mode at 2×) |
| ⚠️ Claude Opus 4.6 | **LEGACY** · Moved to Legacy section (May 25, 2026); still API-accessible; Fast Mode $30/$150 (6×) | $5.00 | $25.00 | → Claude Opus 4.8 (same price, cheaper Fast Mode at 2×) |
| ⚠️ Claude Sonnet 4.5 | **LEGACY** · Moved to Legacy section (May 25, 2026); 1M beta RETIRED Apr 30, 2026 | $3.00 | $15.00 | → Claude Sonnet 4.6 (same price, 1M context) |
| ⚠️ Claude Opus 4.5 | **LEGACY** · Moved to Legacy section (May 25, 2026); still API-accessible | $5.00 | $25.00 | → Claude Opus 4.8 (same price, 1M context, 128k output) |
| ⚠️ Claude Opus 4.1 | LEGACY | $15.00 | $75.00 | → Claude Opus 4.8 (67% cheaper) |
| ⚠️ Claude Sonnet 4 | **DEPRECATED · 🚨 Retiring June 15, 2026 (7 DAYS AWAY)** — migrate immediately | $3.00 | $15.00 | → Claude Sonnet 4.6 — **migrate NOW** |
| ⚠️ Claude Opus 4 | **DEPRECATED · 🚨 Retiring June 15, 2026 (7 DAYS AWAY)** — migrate immediately | $15.00 | $75.00 | → Claude Opus 4.8 — **migrate NOW** |
| ⚠️ Claude Haiku 3.5 | **RETIRED Feb 19, 2026 ❌ (Claude API)** — still on Bedrock/Vertex AI | $0.80 | $4.00 | → Claude Haiku 4.5 |
| ⚠️ Claude Haiku 3 | **RETIRED February 19, 2026 ❌ API ERRORS** | $0.25 | $1.25 | → Claude Haiku 4.5 |
| ⚠️ Claude Sonnet 3.7 | **RETIRED October 28, 2025 ❌ API ERRORS** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 3 Opus | **DEPRECATED** Jan 2026 — available by request for paying customers | $15.00 | $75.00 | → Claude Opus 4.8 |
| ⚠️ Claude 3.5 Sonnet | **RETIRED January 5, 2026** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 2.x | **RETIRED** | ~$8.00 | ~$24.00 | → Claude Sonnet 4.6 |

### 🟢 OpenAI — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ GPT-5.4 Pro | LEGACY · Superseded by GPT-5.5 Pro | $30.00 | $180.00 | → GPT-5.5 Pro (same price, better performance) |
| ⚠️ GPT-5.3 / Codex | LEGACY · Phasing out Jun 2026 | $1.75 | $14.00 | → GPT-5.5 or GPT-5.4 |
| ⚠️ GPT-5.2 | LEGACY · Phasing out Jun 2026 · **GPT-5.2 Thinking RETIRED June 5, 2026 ❌** | $1.75 | $14.00 | → GPT-5.4 or GPT-5.5 |
| ⚠️ GPT-5.1 | **RETIRED March 11, 2026** | — | — | → GPT-5.5 |
| ⚠️ GPT-4o | LEGACY | $2.50 | $10.00 | → GPT-4.1 (cheaper, 1M ctx) |
| ⚠️ GPT-4o mini | LEGACY | $0.15 | $0.60 | → GPT-5.4 nano or GPT-4.1 nano |
| ⚠️ o1 | LEGACY (very expensive) | $15.00 | $60.00 | → o3 (87% cheaper) |
| ⚠️ GPT-4 Turbo | **RETIRED** | — | — | → GPT-4.1 |
| ⚠️ GPT-3.5 Turbo | **RETIRED** | — | — | → GPT-4.1 nano |

### 🔵 Google Gemini — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ Gemini 2.0 Flash | **DEPRECATED · Shutdown June 1, 2026** | → Gemini 2.5 Flash ($0.30/$2.50) or Gemini 3.5 Flash ($1.50/$9.00) |
| ⚠️ Gemini 2.0 Flash-Lite | **DEPRECATED · Shutdown June 1, 2026** | → Gemini 2.5 Flash-Lite ($0.10/$0.40) |
| ⚠️ Gemini 3 Pro Preview | **RETIRED** March 9, 2026 | → Gemini 3.5 Flash or Gemini 3.1 Pro Preview |
| ⚠️ Gemini 1.5 Pro | LEGACY | → Gemini 2.5 Pro |
| ⚠️ Gemini 1.5 Flash | LEGACY | → Gemini 2.5 Flash |

### 🟡 Mistral AI — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ Pixtral Large | **LEGACY** · Deprecated per docs.mistral.ai (May 2026); removed from pricing page | → Mistral Medium 3.5 ($1.50/$7.50, vision + reasoning) or Mistral Small 4 ($0.10/$0.30, vision) |
| ⚠️ Magistral Small 1.2 (v2509) | **LEGACY** · Specific version deprecated per docs.mistral.ai (May 25, 2026); `magistral-small-latest` still active at $0.50/$1.50 | → Mistral Small 4 with `reasoning_effort=high` ($0.10/$0.30) |
| ⚠️ Devstral Small 1.1 | LEGACY · Superseded by Devstral Small 2 (Dec 2025) | → Devstral Small 2 ($0.10/$0.30, 256K ctx) |
| ⚠️ Devstral Medium | LEGACY · Superseded by Devstral 2 (Dec 2025) | → Devstral 2 ($0.40/$2.00) or Medium 3.5 |
| ⚠️ Mistral Small 3.2 24B | LEGACY · Superseded Mar 2026 | → Mistral Small 4 |
| ⚠️ Mistral Small 3.1 | LEGACY · Superseded Jun 2025 | → Mistral Small 4 |
| ⚠️ Mistral Large 2 (2407) | LEGACY | → Mistral Large 3 |
| ⚠️ Mistral Medium 3 (original) | LEGACY · Superseded Aug 2025 | → Mistral Medium 3.1 or Medium 3.5 |
| ⚠️ Codestral 2501 | LEGACY · Superseded Aug 2025 | → Codestral 2508 |
| ⚠️ Mixtral 8×7B (API) | Active API at $0.70/$0.70 — legacy generation; prefer Ministral 3 8B | → Mistral Nemo or Ministral 3 8B ($0.15/$0.15) |

---

## 🏷️ Price Change Log

| Date | Provider | Model | Change |
|---|---|---|---|
| 2026-06-08 | Anthropic | **Claude Opus 4.7** | 🔁 CORRECTION — Previous note incorrectly stated "Fast Mode was NOT available on Opus 4.7." Official `platform.claude.com/docs/en/about-claude/pricing` confirms **Fast Mode IS available on Opus 4.7 at $30/$150 per MTok** (same rate as Opus 4.6). Opus 4.7 entry updated. |
| 2026-06-08 | Anthropic | **Claude Sonnet 4 + Opus 4** | 🚨 URGENCY UPDATE — Retirement is **7 days away (June 15, 2026)**. Migrate to Sonnet 4.6 and Opus 4.8 immediately. |
| 2026-06-08 | Anthropic | **All active models** | ✅ RE-VERIFIED — Opus 4.8 $5/$25, Sonnet 4.6 $3/$15, Haiku 4.5 $1/$5 confirmed unchanged. |
| 2026-06-08 | OpenAI | **GPT-5.2 Thinking** | 🚨 RETIRED June 5, 2026 — API calls to `gpt-5.2-thinking` now return errors. Migrate to GPT-5.4 or GPT-5.5. |
| 2026-06-08 | OpenAI | **All active models** | ✅ RE-VERIFIED — All prices confirmed unchanged. Source: openai.com/api/pricing/. |
| 2026-06-08 | Mistral | **Leanstral** | 🆕 ADDED — Now listed on official `mistral.ai/pricing`. First open-source code agent for Lean 4. **Free** during feedback-collection period. API ID: `labs-leanstral-2603`. |
| 2026-06-08 | Mistral | **Mistral Small Creative** | 🆕 ADDED — Now listed on official `mistral.ai/pricing` as Labs model. Fine-tuned for creative writing, roleplay, chat. **$0.10/$0.30 per MTok**. API ID: `labs-mistral-small-creative`. |
| 2026-06-08 | Mistral | **OCR 3** | 🆕 DOCUMENTED — Now formally documented with pricing from official `mistral.ai/pricing`. **$2.00/1K pages** (OCR) + **$3.00/1K pages** (Annotations). API ID: `mistral-ocr-latest`. |
| 2026-06-08 | Mistral | **Codestral Embed** | 🆕 DOCUMENTED — Now formally documented. **$0.15/MTok** input only. API ID: `codestral-embed`. |
| 2026-06-08 | Mistral | **Mistral Embed** | 🆕 DOCUMENTED — Now formally documented. **$0.10/MTok** input only. API ID: `mistral-embed`. |
| 2026-06-08 | Mistral | **Mistral Moderation** | 🆕 DOCUMENTED — Version 2603 (March 2026). **$0.10/MTok** input. API ID: `mistral-moderation-2603`. |
| 2026-06-08 | Mistral | **Mistral Medium 3.1** | ⚠️ PRICING PAGE REMOVAL — `mistral-medium-3-1` is no longer listed on `mistral.ai/pricing` as of June 8, 2026. Still in `docs.mistral.ai` as Premier. Verify accessibility before building new workloads; last known price $0.40/$2.00. |
| 2026-06-08 | Mistral | **All other active models** | ✅ RE-VERIFIED — All prices confirmed unchanged. Source: mistral.ai/pricing. |
| 2026-06-01 | Anthropic | **Claude Sonnet 4 + Opus 4** | 🔁 CORRECTION — Previous entry incorrectly stated "RETIRED April 20, 2026." Official retirement date is **June 15, 2026** per `platform.claude.com/docs/en/release-notes/overview` and `docs.anthropic.com/en/docs/about-claude/model-deprecations`. Both models are still API-accessible until June 15. Status updated to DEPRECATED. |
| 2026-06-01 | OpenAI | **GPT-5.5 Priority Tier** | 🆕 DOCUMENTED — Priority processing tier confirmed at **$12.50 input / $75.00 output per MTok** (2.5× standard). Batch/Flex at $2.50/$15.00 (50% off standard). Source: developers.openai.com/api/docs/pricing. |
| 2026-06-01 | Mistral | **Voxtral Mini** | 🆕 ADDED — New model now listed on official `mistral.ai/pricing`. 3B lightweight audio understanding model. Audio input: **$0.001/min**; text input: **$0.04/MTok**; output: **$0.04/MTok**. Model ID: `voxtral-mini-latest`. Apache 2.0 open-weight. |
| 2026-06-01 | Mistral | **Voxtral Mini Transcribe** | 🆕 ADDED — Transcription-optimized endpoint. Pricing: **$0.002/min**. Model ID: `voxtral-mini-latest` transcription endpoint. Supports diarization, 13 languages. |
| 2026-06-01 | Mistral | **Mixtral 8x7B + 8x22B (API)** | 📝 DOCUMENTED — Both models confirmed active on `mistral.ai/pricing`. 8x7B: **$0.70/$0.70** per MTok. 8x22B: **$2.00/$6.00** per MTok. |
| 2026-05-28 | Anthropic | **Claude Opus 4.8** | 🚨 LAUNCHED — New active flagship. Model ID `claude-opus-4-8`. $5/$25 per MTok. Fast Mode: 2× standard ($10/$50) for up to 2.5× speed. Context: 1M tokens (200k on MS Foundry). Max output: 128k sync / 300k Batch. |
| 2026-05-28 | Anthropic | **Claude Opus 4.7** | ⚠️ STATUS CHANGE → LEGACY — Official Anthropic pricing page now lists Opus 4.7 in "Legacy models" section. |
| 2026-05-28 | Mistral | **Devstral 2 (2512)** | ✏️ PRICE CORRECTION — Output corrected from $0.90 → **$2.00 per MTok**. |
| 2026-05-28 | Mistral | **Pixtral Large** | ⚠️ MOVED TO LEGACY — No longer listed on `mistral.ai/pricing`. |
| 2026-05-28 | Mistral | **Mistral Small 4** | ✏️ PRICE UPDATE — Input: $0.15 → **$0.10** / Output: $0.60 → **$0.30** per MTok. |
| 2026-05-28 | Mistral | **Ministral 3B** | ✏️ PRICE UPDATE — $0.04/$0.04 → **$0.10/$0.10** per MTok. |
| 2026-05-28 | Mistral | **Ministral 8B** | ✏️ PRICE UPDATE — $0.10/$0.10 → **$0.15/$0.15** per MTok. |
| 2026-05-28 | Mistral | **Voxtral Small** | ✏️ UPDATE — Audio input: $0.004/min; Output updated $0.30 → **$0.40/MTok**. |
| 2026-05-25 | Anthropic | **Claude Opus 4.6** | ⚠️ STATUS CHANGE → LEGACY |
| 2026-05-25 | Anthropic | **Claude Sonnet 4.5** | ⚠️ STATUS CHANGE → LEGACY |
| 2026-05-25 | Anthropic | **Claude Opus 4.5** | ⚠️ STATUS CHANGE → LEGACY |
| 2026-05-21 | Google | **Gemini 3.5 Flash** | 🆕 ADDED — Released May 19, 2026 (Google I/O). $1.50/$9.00 per MTok; 1M context. |
| 2026-05-04 | Mistral | **Mistral Medium 3.5** | 🆕 ADDED — Released April 29, 2026. $1.50/$7.50 per MTok. |
| 2026-04-25 | OpenAI | **GPT-5.5 / GPT-5.5 Pro** | 🆕 LAUNCHED April 23-24, 2026. $5.00/$30.00 / $30.00/$180.00 per MTok. |
| 2026-04-16 | Anthropic | **Claude Opus 4.7** | 🆕 LAUNCHED — $5/$25 per MTok. SWE-bench Verified 87.6%. |

---

## ℹ️ Notes
- All prices are in **USD** and listed **per million tokens (MTok)**.
- **Batch API discounts (50%)** are available from Anthropic, OpenAI, Google Gemini, and **Mistral** (confirmed May 28, 2026).
- **Prompt/context caching** discounts apply where noted. Mistral does **not** offer prompt caching.
- Enterprise/volume pricing is available from all providers on a negotiated basis.
- **OpenAI GPT-5.4 and GPT-5.5** use short context (<272K) and long context (>272K) pricing tiers. For GPT-5.5: long-context = 2× input / 1.5× output.
- **OpenAI service tiers:** Priority (2.5× standard) → Standard (default) → Batch/Flex (50% off). For GPT-5.5: Priority=$12.50/$75, Standard=$5/$30, Batch=$2.50/$15.
- **Google Gemini Pro** models (2.5 Pro, 3.1 Pro) double input cost for prompts >200K tokens.
- **Mistral** processes all API data in the EU by default — key compliance advantage for GDPR workloads.
- **Anthropic** offers US-only inference (data residency) at 1.1× pricing via `inference_geo: "us"` parameter (Opus 4.6, Sonnet 4.6, and later models).
- **Tier 2 OpenRouter Picks** use OpenRouter prices which are typically at or near direct provider API rates.
- ⚠️ Models marked **RETIRED** return API errors. Models marked **DEPRECATED** still work but have a published end-of-life date. Models marked **LEGACY** are still API-accessible but listed in the provider's legacy/deprecated section.
- 🔒 **Restricted models** (Mythos Preview, GPT-5.4-Cyber) have no public API or general pricing — noted for awareness only.
- 🚨 **URGENT June 2026 deadlines:** Gemini 2.0 Flash shutdown June 1 (passed) · GPT-5.2 Thinking RETIRED June 5 (passed) · **Claude Sonnet 4 + Opus 4 retire June 15 (7 days — migrate NOW)**
- 🔁 **Correction (June 8, 2026):** Claude Opus 4.7 Fast Mode IS available at $30/$150 per MTok (same as Opus 4.6) — a previous note in this tracker incorrectly stated it was not available. Official Anthropic pricing page confirmed.
- 🆕 **New Mistral models (June 8, 2026):** Leanstral (Labs, Free), Mistral Small Creative (Labs, $0.10/$0.30), OCR 3 ($2/1K pages), Codestral Embed ($0.15/MTok input), Mistral Embed ($0.10/MTok input), Mistral Moderation ($0.10/MTok input) documented; Mistral Medium 3.1 removed from pricing page.
