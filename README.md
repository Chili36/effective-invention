# 🤖 LLM Pricing Tracker

Up-to-date pricing and specifications for large language models from **Anthropic**, **OpenAI**, **Google Gemini**, **Mistral AI**, and top **OpenRouter picks**.

> **Last updated:** 2026-06-29 (refresh #22)
> **Sources:** Official provider pricing pages — scraped/verified on date above.

---

## 📋 Quick-Reference Index — Active Models

### 🟠 Tier 1 — Anthropic Claude

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Max Output | Availability |
|---|---|---|---|---|---|
| **🚫 Claude Fable 5** *(SUSPENDED June 12 — US Gov't Export Control)* | $10.00 *(last known)* | $50.00 *(last known)* | **1M tokens** | 128k | 🚫 SUSPENDED — see [Anthropic statement](https://www.anthropic.com/news/fable-mythos-access) |
| **Claude Opus 4.8** *(Current Top-Tier / Daily Driver)* | $5.00 | $25.00 | **1M tokens** | 128k sync / 300k Batch | API, AWS Bedrock (Messages API), Vertex AI, MS Foundry (200k ctx) |
| **Claude Sonnet 4.6** | $3.00 | $15.00 | **1M tokens** | 64k sync / 300k Batch | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Haiku 4.5** | $1.00 | $5.00 | 200K tokens | 64k | API, AWS Bedrock (all regions), Vertex AI, MS Foundry |

> 💡 Batch API: 50% off · Prompt caching: up to 90% off
> 🚫 **Claude Fable 5 SUSPENDED June 12, 2026** — US government export control directive. All other Claude models unaffected. Fallback: Claude Opus 4.8 ($5/$25).
> ⚡ **Opus 4.8 Fast Mode:** $10/$50 per MTok (2× standard) — up to 2.5× faster
> 🧠 **Thinking:** Opus 4.8 = Adaptive only · Sonnet 4.6 = Adaptive + Extended · Haiku 4.5 = Extended only
> 🔒 Claude Mythos 5 — 🚫 SUSPENDED (Project Glasswing access also halted June 12, 2026)
> ✅ **Claude Sonnet 4 + Opus 4 RETIRED June 15, 2026 ❌** — API calls now return errors; migrate to Sonnet 4.6 / Opus 4.8
> 🆕 **Claude Tag** launched June 23, 2026 — Teams product integration (@Claude), not a new API model.

---

### 🟢 Tier 1 — OpenAI (Proprietary)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|---|
| **GPT-5.5** *(Current Flagship)* | $5.00 / $10.00* | $0.50 / $1.00* | $30.00 / $45.00* | **1.05M tokens** | API |
| **GPT-5.5 Pro** | $30.00 / $60.00* | — | $180.00 / $270.00* | 1M tokens | API |
| GPT-5.4 *(prev flagship)* | $2.50 / $5.00† | $0.25 / $0.50† | $15.00 / $22.50† | 1.05M tokens | API |
| GPT-5.4 Pro | $30.00 / $60.00* | — | $180.00 / $270.00* | 1.05M tokens | API |
| **GPT-5.4 mini** | $0.75 | $0.075 | $4.50 | 400K tokens | API |
| **GPT-5.4 nano** | $0.20 | $0.020 | $1.25 | 400K tokens | API |
| GPT-4.1 | $2.00 | $0.50 | $8.00 | 1.04M tokens | API |
| **GPT-4.1 mini** | $0.40 | $0.10 | $1.60 | 1.00M tokens | API |
| GPT-4.1 nano | $0.10 | — | $0.40 | 1M+ tokens | API |
| o3 *(reasoning)* | $2.00 | $0.50 | $8.00 | 200K tokens | API |
| o3-pro *(reasoning)* | $20.00 | — | $80.00 | 200K tokens | API |
| o4-mini *(reasoning)* | $1.10 | $0.275 | $4.40 | 200K tokens | API |

> 💡 Batch/Flex API: 50% off all models · Cached inputs: 50–90% off · Regional processing: +10% on GPT-5.5 and GPT-5.4 family
> *GPT-5.5 / GPT-5.5 Pro / GPT-5.4 Pro long-context pricing (>~270K tokens): standard × 2 input / × 1.5 output for GPT-5.5; standard × 2 for Pro models
> †GPT-5.4 tiered pricing: short ctx (<~270K) / long ctx (>~270K)
> 🔒 GPT-5.4-Cyber — limited vetted access only
> 📝 GPT-5.5 Pro batch: $15/$90 (std ctx) · GPT-5.4 Pro batch: $15/$90 (std), $30/$135 (long) · gpt-5.3-codex priority: $3.50/$28

**Multimodal / Specialized:**

| Model | Pricing |
|---|---|
| gpt-realtime-2 | Audio $32/$64 · Text $4/$24 · Image $5 input (per MTok) |
| gpt-realtime-translate | $0.034 / minute |
| **gpt-realtime-whisper** | **$0.017 / minute** |
| gpt-image-2 | Image $8 input / $30 output · Text $5 input (per MTok) |
| ⚠️ gpt-image-1.5 | DEPRECATED — shutdown Dec 1, 2026 → migrate to gpt-image-2 |
| ⚠️ gpt-image-1-mini | DEPRECATED — shutdown Dec 1, 2026 → migrate to gpt-image-2 |
| sora-2 | $0.10 / sec (720p) |
| sora-2-pro | $0.30–$0.70 / sec (720p–1080p) |
| o3-deep-research | $5.00 input / $20.00 output per MTok |
| o4-mini-deep-research | $1.00 input / $4.00 output per MTok |
| gpt-4o-transcribe | $2.50/$10.00 per MTok (~$0.006/min) |
| gpt-4o-mini-transcribe | $1.25/$5.00 per MTok (~$0.003/min) |

---

### 🔵 Tier 1 — Google Gemini

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Notes |
|---|---|---|---|---|
| **Gemini 3.5 Flash** 🆕 *(New Flagship — May 19, 2026)* | $1.50 | $9.00 | **1M tokens** | GA Stable; thinking supported |
| **Gemini 3.1 Pro Preview** | $2.00 / $4.00* | $12.00 / $18.00* | **1M tokens** | *Tiered at >200K; Preview |
| **Gemini 3.1 Flash-Lite** 🆕 *(Stable GA)* | $0.25 | $1.50 | **1M tokens** | GA Stable (May 2026) |
| **Gemini 2.5 Pro** | $1.25 / $2.50* | $10.00 / $15.00* | **1M tokens** | *Tiered at >200K; GA |
| **Gemini 2.5 Flash** | $0.30 | $2.50 | **1M tokens** | GA; optional thinking mode |
| **Gemini 2.5 Flash-Lite** | $0.10 | $0.40 | **1M tokens** | GA; cheapest Gemini |
| ~~Gemini 2.0 Flash~~ ⚠️ | $0.10 | $0.40 | 1M tokens | ⚠️ **DEPRECATED — Shutdown June 1, 2026** |

> 💡 Batch API: 50% off · Context caching: 90% off repeated prefixes · Free tier via AI Studio

---

### 🟡 Tier 1 — Mistral AI

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Mistral Medium 3.5** 🆕 *(Apr 29, 2026)* | $1.50 | $7.50 | 256K tokens | API |
| **Mistral Large 3 (2512)** | $0.50 | $1.50 | 256K tokens | API |
| **Magistral Medium** *(latest)* | $2.00 | $5.00 | 128K tokens | API |
| Magistral Small *(latest)* | $0.50 | $1.50 | 128K tokens | API |
| **Mistral Small 4** 📈 | $0.15 | $0.60 | **256K tokens** | API |
| Codestral 2508 | $0.30 | $0.90 | 256K tokens | API |
| **Devstral 2** *(devstral-medium-latest)* | $0.40 | $2.00 | 256K tokens | API |
| **Devstral Small 2** [Labs] | $0.10 | $0.30 | **256K tokens** | API |
| Voxtral Small 24B | $0.004/min (audio) | $0.40 | 128K tokens | API |
| **Voxtral Mini Transcribe 2** (v26.02, Premier) | $0.003/min | — | — | API |
| **Voxtral Mini Transcribe Realtime** (v26.02, Open) | $0.006/min | — | — | API |
| Voxtral TTS | $0.016/1K chars | — | — | API |
| 🆕 **OCR 4** *(Jun 23, 2026)* | $4.00/1K pages | $2.00/1K pages (Batch) · $5.00/1K pages (DocAI) | — | API |
| 🆕 **Classifier API 3B** | $0.10 + $1/MTok training | $0.10 | — | API |
| 🆕 **Classifier API 8B** | $0.04 + $1/MTok training | $0.04 | — | API |
| **Codestral Embed** *(Premier)* | $0.15 (input only) | — | — | API |
| **Mistral Embed** | $0.10 (input only) | — | — | API |
| **Mistral Moderation 2** | $0.10 (input only) | — | — | API |
| Mistral Nemo | $0.15 | $0.15 | 128K tokens | API |
| Ministral 3 14B | $0.20 | $0.20 | 256K tokens | API |
| Ministral 3 8B | $0.15 | $0.15 | 256K tokens | API |
| Ministral 3 3B | $0.10 | $0.10 | 556K tokens | API |
| Mixtral 8x22B *(legacy API)* | $2.00 | $6.00 | 64K tokens | API |
| Mixtral 8x7B *(legacy API)* | $0.70 | $0.70 | 32K tokens | API |

> 💡 Batch API: 50% off · EU data residency by default
> 📈 **Mistral Small 4** price increased to $0.15/$0.60 (was $0.10/$0.30) — verified June 29, 2026
> 🆕 **OCR 4** launched June 23, 2026 — supersedes OCR 3; adds bounding boxes, 170-language support
> ⚠️ **Voxtral Mini 3B** (`voxtral-mini-2507`) moved to legacy; `voxtral-mini-latest` now points to Voxtral Mini Transcribe 2

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
| Anthropic | 1 | [anthropic.md](./anthropic.md) | Full model cards — **🚫 Fable 5 + Mythos 5 SUSPENDED June 12 (US gov't export control)** · Opus 4.8 ($5/$25) is current top-tier · Sonnet 4 + Opus 4 RETIRED June 15 · Claude Tag product (June 23, not an API model) |
| OpenAI | 1 | [openai.md](./openai.md) | Full model cards — GPT-5.5 current flagship · gpt-realtime-whisper ($0.017/min) · gpt-image-1.5 + gpt-image-1-mini DEPRECATED (Dec 1, 2026) · batch/priority pricing for Pro models added |
| Google Gemini | 1 | [gemini.md](./gemini.md) | Full model cards incl. Gemini 3.5 Flash (new flagship), 3.1 Flash-Lite stable GA, 2.0 Flash deprecation |
| Mistral AI | 1 | [mistral.md](./mistral.md) | Full model cards — **🆕 OCR 4** (Jun 23) · **📈 Small 4 price +50%/+100%** · Voxtral Mini 3B legacy · all prices re-verified June 29, 2026 |
| OpenRouter Picks | 2 | [openrouter-picks.md](./openrouter-picks.md) | One best-performing model per Tier 2 provider, all via OpenRouter |

---

## ⚠️ Legacy / Deprecated / Retired Models

### 🟠 Anthropic — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| 🚫 Claude Fable 5 | **SUSPENDED ❌ June 12, 2026** — US gov't export control directive | $10.00 | $50.00 | → Claude Opus 4.8 ($5/$25) while suspended |
| 🚫 Claude Mythos 5 | **SUSPENDED ❌ June 12, 2026** — US gov't export control directive (Project Glasswing halted) | $10.00 | $50.00 | N/A — limited access model |
| ⚠️ Claude Opus 4.7 | **LEGACY** · Moved to Legacy May 28, 2026; Fast Mode $30/$150 (6×) | $5.00 | $25.00 | → Claude Opus 4.8 |
| ⚠️ Claude Opus 4.6 | **LEGACY** · Moved to Legacy May 25, 2026; Fast Mode $30/$150 (6×) | $5.00 | $25.00 | → Claude Opus 4.8 |
| ⚠️ Claude Sonnet 4.5 | **LEGACY** · 1M beta RETIRED Apr 30, 2026 | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude Opus 4.5 | **LEGACY** | $5.00 | $25.00 | → Claude Opus 4.8 |
| ⚠️ Claude Opus 4.1 | **LEGACY** (deprecated) | $15.00 | $75.00 | → Claude Opus 4.8 |
| ⚠️ Claude Sonnet 4 | **RETIRED ❌ June 15, 2026** — API calls return errors | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude Opus 4 | **RETIRED ❌ June 15, 2026** — API calls return errors | $15.00 | $75.00 | → Claude Opus 4.8 |
| ⚠️ Claude Haiku 3.5 | **RETIRED Feb 19, 2026 ❌ (Claude API)** | $0.80 | $4.00 | → Claude Haiku 4.5 |
| ⚠️ Claude Haiku 3 | **RETIRED Feb 19, 2026 ❌** | $0.25 | $1.25 | → Claude Haiku 4.5 |
| ⚠️ Claude Sonnet 3.7 | **RETIRED Oct 28, 2025 ❌** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 3 Opus | **DEPRECATED** Jan 2026 | $15.00 | $75.00 | → Claude Opus 4.8 |
| ⚠️ Claude 3.5 Sonnet | **RETIRED Jan 5, 2026** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 2.x | **RETIRED** | ~$8.00 | ~$24.00 | → Claude Sonnet 4.6 |

### 🟢 OpenAI — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ GPT-Realtime-1.5 | **LEGACY** · Removed from pricing page June 2026 | $4.00 (text) / $32.00 (audio) | $16.00 (text) / $64.00 (audio) | → gpt-realtime-2 |
| ⚠️ GPT-Realtime-Mini | **LEGACY** · Removed from pricing page June 2026 | $0.60 (text) / $10.00 (audio) | $2.40 (text) / $20.00 (audio) | → gpt-realtime-2 |
| ⚠️ GPT-Image-1.5 | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | $8.00 | $32.00 | → gpt-image-2 |
| ⚠️ GPT-Image-1-mini | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | $2.50 | $8.00 | → gpt-image-2 |
| ⚠️ chatgpt-image-latest | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | — | — | → gpt-image-2 |
| ⚠️ GPT-5.4 Pro | LEGACY · Superseded by GPT-5.5 Pro (same std price, better perf) | $30.00 | $180.00 | → GPT-5.5 Pro |
| ⚠️ GPT-5.3 / Codex | LEGACY · Phasing out Jun 2026 (still available as gpt-5.3-codex) | $1.75 | $14.00 | → GPT-5.5 or GPT-5.4 |
| ⚠️ GPT-5.2 | LEGACY · **All GPT-5.2 retired from ChatGPT June 12, 2026 ❌** | $1.75 | $14.00 | → GPT-5.4 or GPT-5.5 |
| ⚠️ GPT-5.1 | **RETIRED March 11, 2026** | — | — | → GPT-5.5 |
| ⚠️ GPT-4o | LEGACY | $2.50 | $10.00 | → GPT-4.1 |
| ⚠️ GPT-4o mini | LEGACY | $0.15 | $0.60 | → GPT-5.4 nano or GPT-4.1 nano |
| ⚠️ o1 | LEGACY | $15.00 | $60.00 | → o3 (87% cheaper) |
| ⚠️ GPT-4 Turbo | **RETIRED** | — | — | → GPT-4.1 |
| ⚠️ GPT-3.5 Turbo | **RETIRED** | — | — | → GPT-4.1 nano |

### 🔵 Google Gemini — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ Gemini 2.0 Flash | **DEPRECATED · Shutdown June 1, 2026** | → Gemini 2.5 Flash or Gemini 3.5 Flash |
| ⚠️ Gemini 2.0 Flash-Lite | **DEPRECATED · Shutdown June 1, 2026** | → Gemini 2.5 Flash-Lite |
| ⚠️ Gemini 3 Pro Preview | **RETIRED** March 9, 2026 | → Gemini 3.5 Flash or Gemini 3.1 Pro Preview |
| ⚠️ Gemini 1.5 Pro | LEGACY | → Gemini 2.5 Pro |
| ⚠️ Gemini 1.5 Flash | LEGACY | → Gemini 2.5 Flash |

### 🟡 Mistral AI — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ OCR 3 v25.12 | **LEGACY** · Superseded by OCR 4 (June 23, 2026); available for existing integrations | → OCR 4 ($4/1K pages std, $2/1K batch) |
| ⚠️ Voxtral Mini 3B v25.07 | **LEGACY** · `voxtral-mini-2507` in legacy table; `voxtral-mini-latest` alias reassigned | → Voxtral Mini Transcribe 2 ($0.003/min) |
| ⚠️ Devstral 2 v25.12 | **LEGACY** · `devstral-2512` in legacy table at docs.mistral.ai; `devstral-medium-latest` still active | Use `devstral-medium-latest` |
| ⚠️ Devstral Small 2 v25.12 | **LEGACY** · `labs-devstral-small-2512` in legacy table; `devstral-small-latest` still active | Use `devstral-small-latest` |
| ⚠️ Magistral Medium 1.2 v2509 | **LEGACY** · `magistral-medium-2509` in legacy table; `magistral-medium-latest` still active | Use `magistral-medium-latest` |
| ⚠️ Leanstral v26.03 | **LEGACY** · Moved to legacy table at docs.mistral.ai (June 15, 2026) | No direct successor |
| ⚠️ Mistral Medium 3.1 v25.08 | **LEGACY** · Confirmed in legacy table at docs.mistral.ai (June 15, 2026) | → Mistral Medium 3.5 or Mistral Large 3 |
| ⚠️ Voxtral Mini Transcribe v25.07 | **LEGACY** · Superseded by v26.02 (June 2026) | → Voxtral Mini Transcribe 2 (v26.02, $0.003/min) or Realtime ($0.006/min) |
| ⚠️ Mistral Small Creative v25.12 | **LEGACY** · Now in legacy per docs.mistral.ai | → Verify on console.mistral.ai |
| ⚠️ Pixtral Large | **LEGACY** · Deprecated May 2026 | → Mistral Medium 3.5 or Mistral Small 4 |
| ⚠️ Magistral Small 1.2 (v2509) | **LEGACY** · Specific version; `magistral-small-latest` still active | → Mistral Small 4 with `reasoning_effort=high` |
| ⚠️ Devstral Small 1.1 | LEGACY | → Devstral Small 2 |
| ⚠️ Devstral Medium | LEGACY | → Devstral 2 or Medium 3.5 |
| ⚠️ Mistral Small 3.2 24B | LEGACY | → Mistral Small 4 |
| ⚠️ Mistral Small 3.1/3.0 | LEGACY | → Mistral Small 4 |
| ⚠️ Mistral Large 2 (2407) | LEGACY | → Mistral Large 3 |
| ⚠️ Codestral 2501 | LEGACY | → Codestral 2508 |

---

## 🏷️ Price Change Log

| Date | Provider | Model | Change |
|---|---|---|---|
| 2026-06-29 | Mistral | **OCR 4** | 🆕 NEW MODEL — Launched June 23, 2026. $4/1K pages (standard), $2/1K pages (Batch-API 50% off), $5/1K pages (Document AI). `mistral-ocr-latest` alias now points to OCR 4. Adds bounding boxes, block classification, confidence scores, 170-language support. OCR 3 moved to legacy. Source: mistral.ai/news/ocr-4/ |
| 2026-06-29 | Mistral | **Mistral Small 4** | 📈 PRICE INCREASE — Input $0.10 → **$0.15/MTok** (+50%). Output $0.30 → **$0.60/MTok** (+100%). Confirmed on live mistral.ai/pricing. |
| 2026-06-29 | Mistral | **Voxtral Mini 3B** | ⚠️ MOVED TO LEGACY — `voxtral-mini-2507` now in legacy table at docs.mistral.ai. `voxtral-mini-latest` alias reassigned to Voxtral Mini Transcribe 2. |
| 2026-06-29 | Mistral | **Devstral 2 v25.12** | ⚠️ LEGACY — `devstral-2512` specific version in legacy table at docs.mistral.ai. `devstral-medium-latest` alias remains active at $0.40/$2.00. |
| 2026-06-29 | Mistral | **Devstral Small 2 v25.12** | ⚠️ LEGACY — `labs-devstral-small-2512` specific version in legacy table at docs.mistral.ai. `devstral-small-latest` alias remains active at $0.10/$0.30. |
| 2026-06-29 | Mistral | **Magistral Medium 1.2 v2509** | ⚠️ LEGACY — `magistral-medium-2509` specific version in legacy table at docs.mistral.ai. `magistral-medium-latest` alias remains active at $2/$5. |
| 2026-06-29 | OpenAI | **GPT-5.5 Pro batch pricing** | 📝 DOCUMENTED — Batch/Flex: $15/$90 per MTok (std ctx). Newly visible on live pricing page. |
| 2026-06-29 | OpenAI | **GPT-5.4 Pro batch pricing** | 📝 DOCUMENTED — Batch/Flex: $15/$90 (std), $30/$135 (long ctx). Newly visible on live pricing page. |
| 2026-06-29 | OpenAI | **gpt-5.3-codex priority pricing** | 📝 DOCUMENTED — Priority: $3.50 input / $0.35 cached / $28.00 output. Confirmed on live pricing page. |
| 2026-06-29 | Anthropic | **Claude Tag** | 🆕 NEW PRODUCT — @Claude Teams integration launched June 23, 2026. Not a new API model; billed at standard token rates. |
| 2026-06-29 | Anthropic | **All active models** | ✅ VERIFIED — Opus 4.8 $5/$25, Sonnet 4.6 $3/$15, Haiku 4.5 $1/$5 all confirmed unchanged. |
| 2026-06-22 | Anthropic | **Claude Fable 5 + Mythos 5** | 🚫 **SUSPENDED** — US government issued export control directive June 12, 2026 suspending all access. Previously missed in June 15 update. Source: [anthropic.com/news/fable-mythos-access](https://www.anthropic.com/news/fable-mythos-access). |
| 2026-06-22 | OpenAI | **gpt-realtime-whisper** | 🆕 NEW — Real-time speech recognition model at $0.017/min added to live pricing page. |
| 2026-06-22 | OpenAI | **gpt-realtime-1.5** | ⚠️ MOVED TO LEGACY — No longer listed on live pricing page as of June 2026. |
| 2026-06-22 | OpenAI | **gpt-realtime-mini** | ⚠️ MOVED TO LEGACY — No longer listed on live pricing page as of June 2026. |
| 2026-06-22 | OpenAI | **gpt-image-1.5** | ⚠️ DEPRECATED — June 2, 2026 notification; API shutdown December 1, 2026. Migrate to gpt-image-2. |
| 2026-06-22 | OpenAI | **gpt-image-1-mini** | ⚠️ DEPRECATED — June 2, 2026 notification; API shutdown December 1, 2026. Migrate to gpt-image-2. |
| 2026-06-22 | OpenAI | **chatgpt-image-latest** | ⚠️ DEPRECATED — June 2, 2026 notification; API shutdown December 1, 2026. Migrate to gpt-image-2. |
| 2026-06-22 | Mistral | **All active models** | ✅ VERIFIED — All active prices re-confirmed unchanged against mistral.ai/pricing. |
| 2026-06-15 | Anthropic | **Claude Sonnet 4** | ⚠️ RETIRED ❌ — `claude-sonnet-4-20250514` API calls now return errors. Migrate to Claude Sonnet 4.6. |
| 2026-06-15 | Anthropic | **Claude Opus 4** | ⚠️ RETIRED ❌ — `claude-opus-4-20250514` API calls now return errors. Migrate to Claude Opus 4.8. |
| 2026-06-15 | Mistral | **Voxtral Mini Transcribe 2** | ✏️ PRICE CORRECTED — $0.002/min → $0.003/min per official mistral.ai/pricing page. |
| 2026-06-15 | Mistral | **Leanstral v26.03** | ⚠️ MOVED TO LEGACY — `labs-leanstral-2603` now in legacy/deprecated table at docs.mistral.ai. |
| 2026-06-15 | Mistral | **Mistral Medium 3.1 v25.08** | ⚠️ FORMALLY DEPRECATED — `mistral-medium-2508` confirmed in legacy table at docs.mistral.ai. |
| 2026-06-09 | Anthropic | **Claude Fable 5** | 🚨 LAUNCHED — $10/$50 per MTok. *(Subsequently SUSPENDED June 12 by US gov't order.)* |
| 2026-06-09 | Anthropic | **Claude Mythos 5** | 🚨 LAUNCHED (limited) — Project Glasswing. *(Subsequently SUSPENDED June 12 by US gov't order.)* |
| 2026-06-09 | Mistral | **Voxtral Mini Transcribe 2** | 🆕 ADDED — v26.02 Premier transcription model, supersedes v25.07. |
| 2026-06-09 | Mistral | **Classifier API model 3B** | 🆕 ADDED — Training $1/MTok, Storage $2/mo/model, Input $0.10/MTok, Output $0.10/MTok. |
| 2026-06-09 | Mistral | **Classifier API model 8B** | 🆕 ADDED — Training $1/MTok, Storage $2/mo/model, Input $0.04/MTok, Output $0.04/MTok. |
| 2026-05-28 | Anthropic | **Claude Opus 4.8** | 🚨 LAUNCHED — $5/$25 per MTok. Fast Mode 2× ($10/$50). 1M context. |
| 2026-04-25 | OpenAI | **GPT-5.5 / GPT-5.5 Pro** | 🆕 LAUNCHED — $5/$30 and $30/$180 per MTok. |
| 2026-04-29 | Mistral | **Mistral Medium 3.5** | 🆕 LAUNCHED — $1.50/$7.50. 256K context. 128B dense. |

---

## ℹ️ Notes
- All prices are in **USD** per million tokens (MTok) unless stated otherwise.
- **Batch API discounts (50%)** apply at Anthropic, OpenAI, Mistral, and Google Gemini.
- **Prompt/context caching** discounts apply where noted. Mistral does **not** offer prompt caching.
- Enterprise/volume pricing available from all providers on request.
- **OpenAI GPT-5.4 and GPT-5.5** have short-context (<~270K) and long-context (>~270K) pricing tiers.
- **OpenAI service tiers:** Priority → Standard → Batch/Flex (50% off).
- **Google Gemini Pro** models double input cost for prompts >200K tokens.
- **Mistral** processes all API data in the EU by default — GDPR compliance advantage.
- **Anthropic** offers US-only inference at 1.1× pricing via `inference_geo: "us"` parameter.
- ⚠️ Models marked **RETIRED** return API errors. **DEPRECATED** = end-of-life published. **LEGACY** = still accessible but in provider's legacy section. **SUSPENDED** = access halted by external directive.
- 🚫 **Claude Fable 5 + Mythos 5 SUSPENDED June 12, 2026** — US government export control directive. All other Claude models unaffected. See [Anthropic's statement](https://www.anthropic.com/news/fable-mythos-access).
- ✅ **Claude Sonnet 4 + Opus 4 RETIRED June 15, 2026 ❌** — API calls now return errors.
- 🆕 **June 29, 2026:** Mistral OCR 4 launched ($4/1K pages); Mistral Small 4 price +50%/+100% to $0.15/$0.60; Voxtral Mini 3B deprecated; OpenAI Pro model batch pricing documented.
