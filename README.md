# 🤖 LLM Pricing Tracker

Up-to-date pricing and specifications for large language models from **Anthropic**, **OpenAI**, **Google Gemini**, **Mistral AI**, and top **OpenRouter picks**.

> **Last updated:** 2026-08-03 (refresh #29)
> **Sources:** Official provider pricing pages — scraped/verified on date above.

---

## 📋 Quick-Reference Index — Active Models

### 🟠 Tier 1 — Anthropic Claude

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Max Output | Availability |
|---|---|---|---|---|---|
| 🔓 **Claude Fable 5** *(RESTORED July 1, 2026 — export controls lifted)* | $10.00 | $50.00 | **1M tokens** | 128k | Claude API, Claude.ai, Claude Code, Claude Cowork; AWS/Google Cloud/MS Foundry re-enabling |
| 🔒 **Claude Mythos 5** *(Restricted — Project Glasswing, restored June 26)* | $10.00 | $50.00 | **1M tokens** | 128k | Project Glasswing (approved orgs) |
| 🆕 **Claude Opus 5** *(New default on Max / strongest on Pro — July 24, 2026)* | $5.00 | $25.00 | **1M tokens** | 128k sync / 300k Batch | API, AWS Bedrock, Claude Platform on AWS, Google Cloud, MS Foundry |
| **Claude Opus 4.8** *(🔄 replaced by Opus 5 as default — still active)* | $5.00 | $25.00 | **1M tokens** | 128k sync / 300k Batch | API, AWS Bedrock (Messages API), Vertex AI, MS Foundry (200k ctx) |
| **Claude Sonnet 5** *(Default Sonnet-tier — intro pricing thru Aug 31)* | $2.00 → $3.00* | $10.00 → $15.00* | **1M tokens** | 128k sync / 300k Batch | API, Claude.ai, Claude Code, AWS Bedrock, Google Cloud, MS Foundry |
| **Claude Sonnet 4.6** *(🔄 replaced by Sonnet 5 as default)* | $3.00 | $15.00 | **1M tokens** | 64k sync / 300k Batch | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Haiku 4.5** | $1.00 | $5.00 | 200K tokens | 64k | API, AWS Bedrock (all regions), Vertex AI, MS Foundry |

> 💡 Batch API: 50% off · Prompt caching: up to 90% off
> 🆕 **Claude Opus 5 launched July 24, 2026** — replaces Opus 4.8 as the default model on Claude Max and the strongest model on Claude Pro, at **identical $5/$25 pricing**. Anthropic reports it approaches Fable 5-level performance on many benchmarks at half Fable 5's price; Opus 4.8 remains active and is still the safety-fallback target for flagged Fable 5 requests. Opus 5 also has the cheapest tool-use overhead of any active model (286/406 tokens).
> ✅ **Claude Fable 5 subscription cliff permanently resolved (July 20, 2026):** Max/Team Premium keep Fable 5 included at 50% of weekly usage limits indefinitely; Pro/Team Standard moved to metered usage credits at the $10/$50 API rate (with a one-time $100 credit).
> 🔓 **Claude Fable 5 + Mythos 5 RESTORED** — the US export control directive that suspended both models on June 12, 2026 was **lifted June 30, 2026**. Fable 5 is available globally starting July 1, 2026. Mythos 5 restored for approved Project Glasswing orgs since June 26, 2026.
> 🆕 **Claude Sonnet 5 launched June 30, 2026** — new default Sonnet-tier model, replacing Sonnet 4.6. *Intro pricing $2/$10 per MTok through Aug 31, 2026, then $3/$15 standard from Sept 1, 2026.
> ⚡ **Fast Mode:** Opus 5 and Opus 4.8 both run Fast Mode at $10/$50 per MTok (2× standard) — up to 2.5× faster. ✅ **Opus 4.7 Fast Mode is now confirmed REMOVED** (as of July 24, 2026 — the live pricing page states `speed: "fast"` requests against Opus 4.7 return an error), completing its previously scheduled deprecation.
> 🧠 **Thinking:** Fable 5/Mythos 5 = Adaptive only · Opus 5/Opus 4.8 = Adaptive only · Sonnet 5 = Adaptive only · Sonnet 4.6 = Adaptive + Extended · Haiku 4.5 = Extended only
> ✅ **Claude Sonnet 4 + Opus 4 RETIRED June 15, 2026 ❌** (Claude API; still on Bedrock/Google Cloud) — migrate to Sonnet 5/4.6 / Opus 5/4.8
> 🔧 **Tools & Agents pricing documented:** Web Search $10/1,000 searches · Code Execution free when paired with web search/fetch, else $0.05/hr per container (1,550 free org-hours/month) · Claude Managed Agents $0.08/session-hour runtime + standard tokens · per-model tool-use system-prompt overhead tabulated (Opus 5: 286–406 tokens vs Opus 4.8: 290–410 tokens vs Opus 4.7 (former): 675–804 tokens).
> ✅ **Re-verified August 3, 2026** directly against the live `platform.claude.com/docs/en/about-claude/pricing` page and `anthropic.com/news` — every price point above confirmed unchanged; no new model releases found since Opus 5 (checked news through July 30, 2026).

---

### 🟢 Tier 1 — OpenAI (Proprietary)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|---|
| 🆕 **GPT-5.6 Sol** *(GA July 9, 2026 — Current Flagship)* | $5.00 / $10.00* | $0.50 / $1.00* | $30.00 / $45.00* | **~1.05M tokens** | ChatGPT, Codex, API — self-serve |
| 📉 **GPT-5.6 Terra** *(Best price/performance — now cheaper)* | $2.00 / $4.00* | $0.20 / $0.40* | $12.00 / $18.00* | **~1.05M tokens** | ChatGPT, Codex, API — self-serve |
| 📉 **GPT-5.6 Luna** *(Fastest/cheapest tier — now ~80% cheaper)* | $0.20 / $0.40* | $0.02 / $0.04* | $1.20 / $1.80* | **~1.05M tokens** | ChatGPT, Codex, API — self-serve |
| **GPT-5.5** *(🔄 Replaced by Sol as flagship — still active)* | $5.00 / $10.00* | $0.50 / $1.00* | $30.00 / $45.00* | **1M tokens** | API |
| **GPT-5.5 Pro** | $30.00 / $60.00* | — | $180.00 / $270.00* | 1M tokens | API |
| GPT-5.4 *(prev flagship)* | $2.50 / $5.00† | $0.25 / $0.50† | $15.00 / $22.50† | 1M tokens | API |
| GPT-5.4 Pro | $30.00 / $60.00* | — | $180.00 / $270.00* | 1.05M tokens | API |
| **GPT-5.4 mini** | $0.75 | $0.075 | $4.50 | 400K tokens | API |
| **GPT-5.4 nano** | $0.20 | $0.020 | $1.25 | 400K tokens | API |
| GPT-4.1 | $2.00 | $0.50 | $8.00 | 1.04M tokens | API |
| **GPT-4.1 mini** | $0.40 | $0.10 | $1.60 | 1.00M tokens | API |
| GPT-4.1 nano | $0.10 | — | $0.40 | 1M+ tokens | API |
| o3 *(reasoning)* | $2.00 | $0.50 | $8.00 | 200K tokens | API |
| o3-pro *(reasoning)* | $20.00 | — | $80.00 | 200K tokens | API |
| o4-mini *(reasoning)* | $1.10 | $0.275 | $4.40 | 200K tokens | API |

> 💡 Batch/Flex API: 50% off all models · Cached inputs: 50–90% off · Regional processing: +10% on GPT-5.6/5.5/5.4 family
> 📉 **GPT-5.6 Terra and Luna got cheaper (Aug 3, 2026):** Terra's short-context price dropped $2.50/$15.00 → **$2.00/$12.00** per MTok; Luna's dropped $1.00/$6.00 → **$0.20/$1.20** per MTok (~80% cheaper). Sol, GPT-5.5, and the GPT-5.4 family are unchanged. Terra is now well under half GPT-5.5's price for GPT-5.5-class quality; Luna undercuts GPT-5.4 mini/nano dramatically for high-volume workloads.
> 🆕 **GPT-5.6 (Sol/Terra/Luna) reached General Availability on July 9, 2026** — after a 13-day limited preview from June 26, it is now self-serve across ChatGPT, Codex, and the API. New caching model: cache writes at 1.25× uncached input rate, 30-min minimum cache life, 90% discount on cache reads. New reasoning-effort ladder: `none/low/medium/high/xhigh/max`, plus a beta multi-agent `ultra` mode. Documented knowledge cutoff: February 16, 2026.
> 🔄 **GPT-5.5 replaced by GPT-5.6 Sol** as OpenAI's recommended flagship (same $5/$30 headline price) — GPT-5.5 remains fully active and is not deprecated.
> 🆕 **GPT-Live-1 / GPT-Live-1 mini** — OpenAI's new full-duplex voice models, launched July 8, 2026 into ChatGPT Voice. Bundled into ChatGPT plans only (no separate charge); **no API pricing published yet** ("coming soon"). This is distinct from the Realtime API (`gpt-realtime-2.1`/`2.1-mini`), which remains the only developer-facing voice API today.
> 🆕 **New transcription models discovered:** `gpt-transcribe` ($0.0045/min, high-accuracy) and `gpt-live-transcribe` ($0.017/min, low-latency realtime) now confirmed as distinct entries on the live models catalog and pricing page.
> *GPT-5.6 / GPT-5.5 / GPT-5.5 Pro / GPT-5.4 Pro long-context pricing (>~270K tokens): standard × 2 input / × 1.5 output (× 2 for Pro models)
> †GPT-5.4 tiered pricing: short ctx (<~270K) / long ctx (>~270K)
> 🔒 GPT-5.4-Cyber — limited vetted access only
> 📝 GPT-5.6 Priority tier (Aug 3, 2026): Sol $10/$1.00 cached/$60, Terra $4/$0.40/$24, Luna $0.40/$0.04/$2.40 (input/cached/output)
> 🔧 **Tools pricing confirmed unchanged:** Web Search $10/1K calls (all models + reasoning-preview) or $25/1K calls (non-reasoning preview, free content tokens) · Computer Use (`computer-use-preview`) $1.50/$6.00 · Containers $0.03–$1.92 per 20-min session · File Search $0.10/GB-day storage + $2.50/1K tool calls.
> ✅ Re-verified August 3, 2026 against the live `developers.openai.com/api/docs/pricing` and `developers.openai.com/api/docs/models` pages — GPT-5.6 Terra/Luna price cuts and two new transcription models confirmed; GPT-5.6 Sol, GPT-5.5, GPT-5.5 Pro, and the GPT-5.4 family confirmed unchanged.

**Multimodal / Specialized:**

| Model | Pricing |
|---|---|
| 🆕 GPT-Live-1 / GPT-Live-1 mini | ChatGPT-only (Free/Go $8/Plus $20/Pro $100+); no API pricing published yet |
| gpt-realtime-2.1 *(supersedes gpt-realtime-2)* | Audio $32/$64 · Text $4/$24 · Image $5 input (per MTok) |
| gpt-realtime-2.1-mini *(supersedes gpt-realtime-mini)* | Audio $10/$20 · Text $0.60/$2.40 · Image $0.80 input (per MTok) |
| gpt-realtime-translate | $0.034 / minute |
| gpt-realtime-whisper | $0.017 / minute |
| 🆕 **gpt-live-transcribe** | **$0.017 / minute** — low-latency realtime transcription |
| 🆕 **gpt-transcribe** | **$0.0045 / minute** — high-accuracy file/realtime transcription |
| gpt-image-2 | Image $8 input / $30 output · Text $5 input (per MTok) |
| ⚠️ gpt-image-1.5 | DEPRECATED — shutdown Dec 1, 2026 → migrate to gpt-image-2 |
| ⚠️ gpt-image-1-mini | DEPRECATED — shutdown Dec 1, 2026 → migrate to gpt-image-2 |
| ⚠️ gpt-4o-mini-tts | DEPRECATED — labeled "Deprecated" on live OpenAI models page |
| sora-2 | $0.10 / sec (720p) |
| sora-2-pro | $0.30–$0.70 / sec (720p–1080p) |
| o3-deep-research | $5.00 input / $20.00 output per MTok |
| o4-mini-deep-research | $1.00 input / $4.00 output per MTok |
| gpt-4o-transcribe | $2.50/$10.00 per MTok (~$0.006/min) |
| gpt-4o-mini-transcribe | $1.25/$5.00 per MTok (~$0.003/min) |
| **computer-use-preview** | $1.50 input / $6.00 output per MTok |

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
> ℹ️ Gemini pricing not re-verified in this update cycle (out of scope for this refresh — see `gemini.md` for last confirmed figures).

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
| **Leanstral 1.5** *(Jun 30, 2026)* [Labs] ⚠️ *(retiring Sep 30, 2026)* | Free | Free | 256K tokens | API (`leanstral-1-5`) |
| Voxtral Small 24B | $0.004/min (audio) | $0.40 | 128K tokens | API |
| **Voxtral Mini Transcribe 2** (v26.02, Premier) | $0.003/min | — | — | API |
| **Voxtral Mini Transcribe Realtime** (v26.02, Open) | $0.006/min | — | — | API |
| Voxtral TTS | $0.016/1K chars | — | — | API |
| **OCR 4** *(Jun 23, 2026)* | $4.00/1K pages | $2.00/1K pages (Batch) · $5.00/1K pages (DocAI) | — | API |
| **Classifier API 3B** | $0.10 + $1/MTok training | $0.10 | — | API |
| **Classifier API 8B** | $0.04 + $1/MTok training | $0.04 | — | API |
| **Codestral Embed** *(Premier)* | $0.15 (input only) | — | — | API |
| **Mistral Embed** | $0.10 (input only) | — | — | API |
| **Mistral Moderation 2** | $0.10 (input only) | — | — | API |
| Mistral Nemo | $0.15 | $0.15 | 128K tokens | API |
| Ministral 3 14B | $0.20 | $0.20 | 256K tokens | API |
| Ministral 3 8B | $0.15 | $0.15 | 256K tokens | API |
| Ministral 3 3B | $0.10 | $0.10 | 256K tokens | API |
| Mixtral 8x22B *(legacy API)* | $2.00 | $6.00 | 64K tokens | API |
| Mixtral 8x7B *(legacy API)* | $0.70 | $0.70 | 32K tokens | API |

> 💡 Batch API: 50% off · EU data residency by default
> 🆕 **Leanstral 1.5** has a published retirement date: September 30, 2026 (per docs.mistral.ai changelog) — still free until then; no successor announced yet.
> 🔭 **Discovery-only (not priced, not tracked as a full model):** Mistral published **Robostral Navigate** (July 8, 2026), an 8B embodied-navigation robotics model (single RGB camera, no LiDAR/depth sensors). It has **no published API pricing** and does not appear on `mistral.ai/pricing/api` — noted for awareness only, per this tracker's verification-before-tracking policy.
> 🔧 **Agent API tool pricing confirmed:** Libraries OCR $3/1K pages, Indexing $1/MTok, Call $0.01/call · Code execution $30/1K calls · Web search $30/1K calls · Image generation $100/1K images · Premium news $50/1K calls · Data capture $0.04/MTok.
> ⚠️ **Marketing-page discrepancy:** the general `mistral.ai/pricing` FAQ still shows a stale "$2/$6" Mistral Large example from an earlier generation. The authoritative `mistral.ai/pricing/api` product table confirms **Mistral Large 3 remains $0.50/$1.50** — no price change.
> 📈 **Mistral Small 4** price increased to $0.15/$0.60 (was $0.10/$0.30) — verified June 29, 2026
> 🆕 **OCR 4** launched June 23, 2026 — supersedes OCR 3; adds bounding boxes, 170-language support
> ⚠️ **Voxtral Mini 3B** (`voxtral-mini-2507`) moved to legacy; `voxtral-mini-latest` now points to Voxtral Mini Transcribe 2
> ✅ Re-verified August 3, 2026 against the live `mistral.ai/pricing/api` page — no price changes or new priced releases detected since July 27.

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
> ℹ️ OpenRouter picks not re-verified in this update cycle (out of scope) — see `openrouter-picks.md` for last confirmed figures.

---

## 📁 Model Card Files

| Provider | Tier | File | Description |
|---|---|---|---|
| Anthropic | 1 | [anthropic.md](./anthropic.md) | Full model cards — Claude Opus 5 ($5/$25, replaces Opus 4.8 as default) · 🔓 Fable 5 + Mythos 5 restored · Claude Sonnet 5 (new default) · ✅ **Opus 4.7 Fast Mode removal now confirmed** · 🔧 Tools & Agents pricing · re-verified Aug 3 |
| OpenAI | 1 | [openai.md](./openai.md) | Full model cards — 📉 **GPT-5.6 Terra & Luna price cuts (Aug 3)** · 🆕 gpt-transcribe & gpt-live-transcribe added · GPT-5.6 GA since July 9, current flagship family · 🆕 GPT-Live-1/mini voice (ChatGPT-only, unpriced API) · re-verified Aug 3 |
| Google Gemini | 1 | [gemini.md](./gemini.md) | Full model cards incl. Gemini 3.5 Flash (new flagship), 3.1 Flash-Lite stable GA, 2.0 Flash deprecation |
| Mistral AI | 1 | [mistral.md](./mistral.md) | Full model cards — ✅ re-verified Aug 3, no pricing changes · 🔭 Robostral Navigate (robotics, unpriced) flagged as discovery-only · Leanstral 1.5 retirement Sep 30 · OCR 4 (Jun 23) · Small 4 price +50%/+100% |
| OpenRouter Picks | 2 | [openrouter-picks.md](./openrouter-picks.md) | One best-performing model per Tier 2 provider, all via OpenRouter |

---

## ⚠️ Legacy / Deprecated / Retired Models

### 🟠 Anthropic — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| 🔓 Claude Fable 5 | **RESTORED ✅ July 1, 2026** — subscription cliff permanently resolved July 20, 2026 | $10.00 | $50.00 | Active — no migration needed |
| 🔓 Claude Mythos 5 | **RESTORED ✅ June 26, 2026** for approved Project Glasswing orgs; no longer suspended | $10.00 | $50.00 | Active (restricted) — no migration needed |
| ⚠️ Claude Mythos Preview | **LEGACY** · Superseded by Claude Mythos 5 (June 9, 2026) | $25.00 | $125.00 | → Claude Mythos 5 |
| 🔄 Claude Opus 4.8 | **REPLACED** as default by Claude Opus 5 (July 24, 2026) — still fully active, same $5/$25 price, not deprecated; remains Fable 5's safety-fallback target | $5.00 | $25.00 | → Claude Opus 5 (same price) |
| 🔄 Claude Sonnet 4.6 | **REPLACED** as default by Claude Sonnet 5 (June 30, 2026) — still fully active, not deprecated | $3.00 | $15.00 | → Claude Sonnet 5 (intro $2/$10 thru Aug 31) |
| ⚠️ Claude Opus 4.7 | **LEGACY** · Fast Mode ❌ **REMOVED July 24, 2026** (confirmed on live pricing page — was $30/$150, 6×) | $5.00 | $25.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude Opus 4.6 | **LEGACY** · Fast Mode ❌ REMOVED June 29, 2026 | $5.00 | $25.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude Sonnet 4.5 | **LEGACY** · 1M beta RETIRED Apr 30, 2026 | $3.00 | $15.00 | → Claude Sonnet 5 or Sonnet 4.6 |
| ⚠️ Claude Opus 4.5 | **LEGACY** | $5.00 | $25.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude Opus 4.1 | **LEGACY** (deprecated) | $15.00 | $75.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude Sonnet 4 | **RETIRED ❌ June 15, 2026** on Claude API (still on Bedrock/Google Cloud) | $3.00 | $15.00 | → Claude Sonnet 5 or Sonnet 4.6 |
| ⚠️ Claude Opus 4 | **RETIRED ❌ June 15, 2026** on Claude API (still on Google Cloud) | $15.00 | $75.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude Haiku 3.5 | **RETIRED Feb 19, 2026 ❌ (Claude API)** | $0.80 | $4.00 | → Claude Haiku 4.5 |
| ⚠️ Claude Haiku 3 | **RETIRED Feb 19, 2026 ❌** | $0.25 | $1.25 | → Claude Haiku 4.5 |
| ⚠️ Claude Sonnet 3.7 | **RETIRED Oct 28, 2025 ❌** | $3.00 | $15.00 | → Claude Sonnet 5 or Sonnet 4.6 |
| ⚠️ Claude 3 Opus | **DEPRECATED** Jan 2026 | $15.00 | $75.00 | → Claude Opus 5 or 4.8 |
| ⚠️ Claude 3.5 Sonnet | **RETIRED Jan 5, 2026** | $3.00 | $15.00 | → Claude Sonnet 5 or Sonnet 4.6 |
| ⚠️ Claude 2.x | **RETIRED** | ~$8.00 | ~$24.00 | → Claude Sonnet 5 or Sonnet 4.6 |

### 🟢 OpenAI — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| 🔄 GPT-5.5 | **REPLACED** as flagship by GPT-5.6 Sol (July 9, 2026) — still fully active, same $5/$30 price, not deprecated | $5.00 | $30.00 | → GPT-5.6 Sol (same price) or Terra (now $2.00/$12.00, well under half price) |
| ⚠️ GPT-Realtime-2 | **LEGACY** · Superseded by `gpt-realtime-2.1` (July 9, 2026 refresh) — identical pricing | $4.00 (text) / $32.00 (audio) | $24.00 (text) / $64.00 (audio) | → gpt-realtime-2.1 |
| ⚠️ GPT-Realtime-1.5 | **LEGACY** · Superseded first by gpt-realtime-2, now by gpt-realtime-2.1 | $4.00 (text) / $32.00 (audio) | $16.00 (text) / $64.00 (audio) | → gpt-realtime-2.1 |
| ⚠️ GPT-Realtime-Mini | **LEGACY** · Superseded by `gpt-realtime-2.1-mini` — identical pricing | $0.60 (text) / $10.00 (audio) | $2.40 (text) / $20.00 (audio) | → gpt-realtime-2.1-mini |
| ⚠️ GPT-4o mini TTS | **DEPRECATED** · Explicitly labeled "Deprecated" on live OpenAI models page | — | — | → gpt-realtime-2.1 or current TTS models |
| ⚠️ GPT-Image-1.5 | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | $8.00 | $32.00 | → gpt-image-2 |
| ⚠️ GPT-Image-1-mini | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | $2.50 | $8.00 | → gpt-image-2 |
| ⚠️ chatgpt-image-latest | **DEPRECATED ❌ June 2, 2026 — Shutdown Dec 1, 2026** | — | — | → gpt-image-2 |
| ⚠️ GPT-5.4 Pro | LEGACY · Superseded by GPT-5.5 Pro (same std price, better perf) | $30.00 | $180.00 | → GPT-5.5 Pro |
| ⚠️ GPT-5.3 / Codex | LEGACY · Phasing out (still available as gpt-5.3-codex) | $1.75 | $14.00 | → GPT-5.6 Terra or GPT-5.5 |
| ⚠️ GPT-5.2 | LEGACY · **All GPT-5.2 retired from ChatGPT June 12, 2026 ❌** | $1.75 | $14.00 | → GPT-5.4 or GPT-5.6 Terra |
| ⚠️ GPT-5.1 | **RETIRED March 11, 2026** | — | — | → GPT-5.6 family |
| ⚠️ GPT-4o | LEGACY | $2.50 | $10.00 | → GPT-4.1 |
| ⚠️ GPT-4o mini | LEGACY | $0.15 | $0.60 | → GPT-5.6 Luna (now $0.20/$1.20) or GPT-4.1 nano |
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
| 🔄 Leanstral v26.03 | **REPLACED** by Leanstral 1.5 (June 30, 2026); was already in legacy table since June 15, 2026 | → Leanstral 1.5 (`leanstral-1-5`) — ⚠️ itself scheduled for retirement Sep 30, 2026 |
| ⚠️ OCR 3 v25.12 | **LEGACY** · Superseded by OCR 4 (June 23, 2026); available for existing integrations | → OCR 4 ($4/1K pages std, $2/1K batch) |
| ⚠️ Voxtral Mini 3B v25.07 | **LEGACY** · `voxtral-mini-2507` in legacy table; `voxtral-mini-latest` alias reassigned | → Voxtral Mini Transcribe 2 ($0.003/min) |
| ⚠️ Devstral 2 v25.12 | **LEGACY** · `devstral-2512` in legacy table at docs.mistral.ai; `devstral-medium-latest` still active | Use `devstral-medium-latest` |
| ⚠️ Devstral Small 2 v25.12 | **LEGACY** · `labs-devstral-small-2512` in legacy table; `devstral-small-latest` still active | Use `devstral-small-latest` |
| ⚠️ Magistral Medium 1.2 v2509 | **LEGACY** · `magistral-medium-2509` in legacy table; `magistral-medium-latest` still active | Use `magistral-medium-latest` |
| ⚠️ Magistral Medium 1.1 v2507 | **LEGACY** · `magistral-medium-2507` cross-checked in legacy table at docs.mistral.ai | Use `magistral-medium-latest` |
| ⚠️ Magistral Small 1.2 (v2509) | **LEGACY** · Specific version; `magistral-small-latest` still active | → Mistral Small 4 with `reasoning_effort=high` |
| ⚠️ Mistral Medium 3.1 v25.08 | **LEGACY** · Confirmed in legacy table at docs.mistral.ai | → Mistral Medium 3.5 or Mistral Large 3 |
| ⚠️ Mistral Medium 3 v25.05 | **LEGACY** · Confirmed in legacy table at docs.mistral.ai | → Mistral Medium 3.5 |
| ⚠️ Voxtral Mini Transcribe v25.07 | **LEGACY** · Superseded by v26.02 (June 2026) | → Voxtral Mini Transcribe 2 (v26.02, $0.003/min) or Realtime ($0.006/min) |
| ⚠️ Mistral Small Creative v25.12 | **LEGACY** · Now in legacy per docs.mistral.ai | → Verify on console.mistral.ai |
| ⚠️ Pixtral Large | **LEGACY** · Deprecated May 2026 | → Mistral Medium 3.5 or Mistral Small 4 |
| ⚠️ Devstral Small 1.1 / 1.0 | LEGACY | → Devstral Small 2 |
| ⚠️ Devstral Medium 1.0 | LEGACY | → Devstral 2 or Medium 3.5 |
| ⚠️ Mistral Small 3.2 24B | LEGACY | → Mistral Small 4 |
| ⚠️ Mistral Small 3.1/3.0 | LEGACY | → Mistral Small 4 |
| ⚠️ Mistral Large 2.x | LEGACY | → Mistral Large 3 |
| ⚠️ Codestral 2501 / 24.05 | LEGACY | → Codestral 2508 |
| ⚠️ Mistral Saba, Pixtral 12B, Ministral 3B/8B (24.10), Mistral Nemo 12B, Codestral Mamba, Mathstral, Mistral 7B, Mistral Large/Small/Medium 1.0, original Mixtral 8x7B/8x22B | LEGACY | → Current generation equivalents (see mistral.md) |

---

## 🏷️ Price Change Log

| Date | Provider | Model | Change |
|---|---|---|---|
| 2026-08-03 | OpenAI | **GPT-5.6 Terra** | 📉 **PRICE CUT** — Short-context input $2.50 → **$2.00**/MTok, output $15.00 → **$12.00**/MTok. Long-context, cached, cache-write, priority, and batch/flex rows recalculated proportionally from the new base price. |
| 2026-08-03 | OpenAI | **GPT-5.6 Luna** | 📉 **PRICE CUT (~80%)** — Short-context input $1.00 → **$0.20**/MTok, output $6.00 → **$1.20**/MTok. All derived pricing tiers (long-context, cached, priority, batch/flex) recalculated proportionally. |
| 2026-08-03 | OpenAI | **gpt-transcribe** | 🆕 **NEW MODEL** — High-accuracy speech-to-text for file and Realtime input transcription, $0.0045/minute. Newly visible on the live models catalog and pricing page. |
| 2026-08-03 | OpenAI | **gpt-live-transcribe** | 🆕 **NEW MODEL** — Low-latency speech-to-text for realtime transcription, $0.017/minute. Now listed as its own catalog entry alongside `gpt-realtime-whisper`. |
| 2026-08-03 | OpenAI | **GPT-5.6 Sol, GPT-5.5, GPT-5.5 Pro, GPT-5.4 family** | ✅ RE-VERIFIED — Confirmed unchanged against the live pricing page. GPT-5.6 family's documented knowledge cutoff is now Feb 16, 2026. |
| 2026-08-03 | Anthropic | **Claude Opus 4.7 Fast Mode** | ✅ **REMOVAL CONFIRMED** — Previously flagged as "deprecated, scheduled removal July 24, 2026"; the live pricing page now explicitly states `speed: "fast"` requests against Opus 4.7 return an error, confirming the removal took effect on schedule. |
| 2026-08-03 | Anthropic | **Claude Opus 5** | 🆕 NEWLY CAPTURED — Tool-use system-prompt overhead (286/406 tokens, `auto`/`none` vs. `any`/`tool`), now the cheapest of any active Claude model, confirmed from the live pricing page's tool-use pricing table. |
| 2026-08-03 | Anthropic | **All other active + legacy models** | ✅ RE-VERIFIED — Independently re-checked the live `platform.claude.com/docs/en/about-claude/pricing` page and `anthropic.com/news` (through July 30, 2026) — no new model releases or price changes found since Claude Opus 5 (July 24, 2026). |
| 2026-08-03 | Mistral | **Robostral Navigate** | 🔭 **DISCOVERY NOTED (not priced, not tracked)** — Mistral published "Introducing Robostral Navigate" (July 8, 2026), an 8B embodied-navigation robotics model. No API pricing published; does not appear on `mistral.ai/pricing/api`. Flagged for awareness only per this tracker's verification-before-tracking policy. |
| 2026-08-03 | Mistral | **All active models + legacy table** | ✅ RE-VERIFIED — Independently checked every price point against `mistral.ai/pricing/api`; no price changes or new priced releases detected since the July 27, 2026 refresh. |
| 2026-07-27 | Anthropic | **Claude Opus 5** | 🆕 **NEW MODEL** — Launched July 24, 2026 at $5.00/$25.00 per MTok, identical pricing to the Opus 4.8 model it replaces. Becomes the new default on Claude Max and the strongest model available on Claude Pro. Anthropic reports it approaches Fable 5-level performance on several benchmarks (Frontier-Bench v0.1: 43.3% vs. Fable 5's 33.7%) at half Fable 5's price. No mandatory data retention (unlike Fable 5's 30-day requirement). Fast Mode: $10/$50 (2×). Model ID `claude-opus-5`. |
| 2026-07-27 | Anthropic | **Claude Opus 4.8** | 🔄 **REPLACED** as default by Claude Opus 5 — same headline price ($5/$25), remains fully active, not deprecated, and continues as the safety-fallback target for flagged Fable 5 requests. |
| 2026-07-27 | Anthropic | **Claude Fable 5 subscription access** | ✅ **PERMANENTLY RESOLVED** — After three extensions (July 7 → 12 → 19), Anthropic split subscription access on July 20, 2026: Max/Team Premium keep Fable 5 included at 50% of weekly usage limits indefinitely; Pro/Team Standard moved to metered usage credits at the standard $10/$50 API rate, softened by a one-time $100 credit. |
| 2026-07-27 | OpenAI | **GPT-Live-1 / GPT-Live-1 mini** | 🆕 **NEW MODEL (ChatGPT-only, unpriced API)** — Full-duplex voice models launched July 8, 2026 into ChatGPT Voice. Bundled into ChatGPT plans (Free gets mini; Go/Plus/Pro get the full model) with no separate charge. No API token/per-minute pricing published yet ("coming soon") — distinct from the Realtime API, which remains the only priced developer voice API. |
| 2026-07-27 | OpenAI | **All active models, Tools, Computer Use** | ✅ RE-VERIFIED — Independently re-checked the live `developers.openai.com/api/docs/pricing` page; GPT-5.6 Sol/Terra/Luna, GPT-5.5, GPT-5.5 Pro, GPT-5.4 family, Realtime, Image, Video, Transcription, Deep Research, Computer Use, and Tools pricing all confirmed unchanged since July 20. |
| 2026-07-27 | Mistral | **Leanstral 1.5** | 🆕 **RETIREMENT DATE PUBLISHED** — `docs.mistral.ai/resources/changelogs` confirms `leanstral-1-5` is scheduled for retirement on **September 30, 2026**. Still free and fully available until then; no successor announced yet. |
| 2026-07-27 | Mistral | **Watch item — new open-weight model** | 🔭 NOTED (not yet tracked) — CEO Arthur Mensch confirmed a new, larger open-weight MoE model family entering early access in July 2026, broader release expected later in the summer. No pricing, benchmarks, or license published — will be added once Mistral publishes official details. |
| 2026-07-27 | Mistral | **All other active models + legacy table** | ✅ RE-VERIFIED — Independently checked every price point against `mistral.ai/pricing/api` and three independent third-party trackers (benchlm.ai, cloudzero.com, spheron.network); no price changes or new priced releases detected since July 20. |
| 2026-07-20 | Anthropic | **Tools & Agents pricing** | 🔧 **NEWLY DOCUMENTED** — Added a dedicated section covering Web Search ($10/1,000 searches), Web Fetch (free), Code Execution (free when paired with `web_search_20260209`+/`web_fetch_20260209`+, else $0.05/hr per container after 1,550 free org-hours/month), per-model tool-use system-prompt token overhead (e.g., Opus 4.8: 290–410 tokens vs. Opus 4.7: 675–804 tokens), and Claude Managed Agents' $0.08/session-hour runtime billing. Sourced directly from the live pricing page's "Feature-specific pricing" and "Claude Managed Agents pricing" sections — no price changes, purely new documentation. |
| 2026-07-20 | Anthropic | **All active + legacy models** | ✅ RE-VERIFIED — Independently re-fetched the live `platform.claude.com/docs/en/about-claude/pricing` page; every price point (Fable 5, Mythos 5, Opus 4.8, Sonnet 5, Sonnet 4.6, Haiku 4.5), including exact cache-write/cache-read/batch figures, and all legacy/retirement statuses confirmed unchanged. |
| 2026-07-20 | OpenAI | **All active models, Tools, Computer Use** | ✅ RE-VERIFIED line-by-line — Independently re-fetched the live `developers.openai.com/api/docs/pricing` page in full, including the Standard/Batch/Flex/Priority matrices for GPT-5.6 Sol/Terra/Luna, GPT-5.5, GPT-5.5 Pro, and GPT-5.4 family, plus Realtime, Image, Video, Transcription, Deep Research, Computer Use (`computer-use-preview` $1.50/$6.00), Codex, and Tools (Web Search, Containers, File Search, Agent Kit) pricing. **Zero changes detected.** |
| 2026-07-20 | Mistral | **Agent API tool pricing** | 🔧 Cross-verified the live `mistral.ai/pricing/api` "Agent API" section against this repo's existing Platform Tool Pricing table — Libraries OCR $3/1K pages, Indexing $1/MTok, Call $0.01/call, Code execution $30/1K calls, Web search $30/1K calls, Image generation $100/1K images, Premium news $50/1K calls, Data capture $0.04/MTok all confirmed unchanged. |
| 2026-07-20 | Mistral | **Mistral Large 3 — marketing FAQ discrepancy flagged** | ⚠️ NOTED — The general `mistral.ai/pricing` (non-API) FAQ page contains a stale illustrative example ("Mistral Large costs $2/M in, $6/M out") left over from an earlier Large generation. The authoritative `mistral.ai/pricing/api` product table was independently re-verified and confirms **Mistral Large 3 remains unchanged at $0.50/$1.50**. Flagging this here so future refreshes don't mistake the stale FAQ copy for a real price change. |
| 2026-07-20 | Mistral | **All other active models + legacy table** | ✅ RE-VERIFIED — Independently checked every price point against `mistral.ai/pricing/api`; legacy table cross-checked against `docs.mistral.ai/models/overview`. No price changes or new releases detected since the July 14, 2026 refresh. |
| 2026-07-14 | OpenAI | **GPT-5.6 (Sol/Terra/Luna)** | 🆕 **REACHED GENERAL AVAILABILITY — July 9, 2026.** After a 13-day limited preview (announced June 26, 2026, restricted to ~20 trusted partners), GPT-5.6 is now live across ChatGPT, Codex, and the API. Pricing unchanged from preview: Sol $5/$30, Terra $2.50/$15, Luna $1/$6 per MTok (short context); 2×/1.5× long-context surcharge above ~270K tokens. New caching model (cache writes 1.25× uncached rate, 90% discount on reads, 30-min minimum cache life). Now documented as OpenAI's "Flagship models." |
| 2026-07-14 | OpenAI | **GPT-5.5** | 🔄 **REPLACED** as current flagship by GPT-5.6 Sol — same headline price ($5/$30), remains fully active and not deprecated. |
| 2026-07-14 | OpenAI | **Realtime models** | 🆕 REFRESHED — `gpt-realtime-2.1` and `gpt-realtime-2.1-mini` now appear on the live pricing page at identical pricing to the prior `gpt-realtime-2` / `gpt-realtime-mini`; older IDs moved to legacy. |
| 2026-07-14 | Anthropic | **Claude Fable 5 subscription window** | 📝 NOTED — The July 1 restoration's subscription-included usage window (originally through July 7) has been **extended twice**, now reported as **July 19, 2026**, per third-party trackers. Underlying API rate ($10/$50) unchanged. *(Superseded by the July 20 permanent resolution above.)* |
| 2026-07-14 | Anthropic | **Consumer pricing (India)** | 🌐 NOTED — Anthropic began localizing Claude.ai consumer plans in INR (Pro ₹2,000/mo, Max ₹11,999/mo, Team ₹2,399/seat/mo) starting July 13, 2026. Consumer subscriptions only — no impact on Claude API/developer pricing. |
| 2026-07-14 | Anthropic | **All active + legacy models** | ✅ RE-VERIFIED — Independently re-fetched the live `platform.claude.com/docs/en/about-claude/pricing` page; every price point (Fable 5, Mythos 5, Opus 4.8, Sonnet 5, Sonnet 4.6, Haiku 4.5) and legacy/retirement status confirmed unchanged. |
| 2026-07-14 | Mistral | **Leanstral 1.5** | 🛠️ **MODEL ID CORRECTED** — Confirmed API endpoint is `leanstral-1-5` (not `labs-leanstral-1-5` as previously documented), verified against docs.mistral.ai and Mistral's official July 2, 2026 announcement post. Benchmark detail added (miniF2F saturated, 587/672 PutnamBench, FATE-H/X SOTA, FLTEval surpassing Claude Opus 4.6 at ~1/7th cost). Pricing unchanged (free). |
| 2026-07-14 | Mistral | **All active models + legacy table** | ✅ RE-VERIFIED — Independently checked every price point against `mistral.ai/pricing/api`; legacy table cross-checked against `docs.mistral.ai/models/overview` — added Magistral Medium 1.1 (v25.07) as a newly-confirmed legacy entry. No price changes detected. |
| 2026-07-06 | Anthropic | **All active + legacy models** | ✅ RE-VERIFIED — Independently re-fetched the live `platform.claude.com/docs/en/about-claude/pricing` page; every price point (Fable 5, Mythos 5, Opus 4.8, Sonnet 5, Sonnet 4.6, Haiku 4.5) and legacy/retirement status confirmed unchanged since July 1, 2026. |
| 2026-07-06 | OpenAI | **All active models** | ✅ RE-VERIFIED — Independently checked every price point against the live `developers.openai.com/api/docs/pricing` and `developers.openai.com/api/docs/models` pages; no changes detected. The models page explicitly confirms GPT-5.6 remains "available to select trusted partners in preview" with broad availability still "coming soon" and no GA date set. |
| 2026-07-06 | Mistral | **All active models + legacy table** | ✅ RE-VERIFIED — Independently checked every price point against `mistral.ai/pricing/api` and the legacy table against `docs.mistral.ai/getting-started/models/models_overview/`; no changes or new releases detected since June 30, 2026. |
| 2026-07-01 | Anthropic | **Claude Fable 5 + Mythos 5** | 🔓 **RESTORED** — US export control directive (issued June 12, 2026) lifted June 30, 2026. Fable 5 available globally starting July 1, 2026 (Claude Platform, Claude.ai, Claude Code, Claude Cowork; AWS/Google Cloud/MS Foundry re-enabling). Mythos 5 restored June 26, 2026 for approved Project Glasswing orgs. New safety classifier blocks the reported jailbreak technique in >99% of cases. Subscription plans (Pro/Max/Team/select Enterprise): Fable 5 included for up to 50% of weekly usage limits through July 7, 2026, then usage-credits billing. Pricing unchanged at $10/$50 per MTok. |
| 2026-07-01 | Anthropic | **US government collaboration** | 🤝 Anthropic committed to expanded pre-release government access/evaluation, rapid jailbreak information sharing, dedicated joint security research, and a common industry security standard. Partnering with Amazon, Microsoft, Google on a shared jailbreak-severity scoring framework. |
| 2026-07-01 | OpenAI | **All active models** | ✅ RE-VERIFIED — Independently checked every price point against the live `developers.openai.com/api/docs/pricing` page; no changes detected. GPT-5.6 remains restricted-preview only. |
| 2026-07-01 | Mistral | **All active models + legacy table** | ✅ RE-VERIFIED — Independently checked every price point against `mistral.ai/pricing` and the legacy table against `docs.mistral.ai/models/overview`; no changes or new releases detected since June 30, 2026. |
| 2026-06-30 | Anthropic | **Claude Sonnet 5** | 🆕 NEW MODEL — Launched June 30, 2026. New default Sonnet-tier model, replacing Sonnet 4.6. Introductory pricing $2/$10 per MTok through Aug 31, 2026, then $3/$15 standard from Sept 1, 2026. Model ID `claude-sonnet-5`. Newer tokenizer produces ~30% more tokens vs Sonnet 4.6-and-earlier tokenizer. 1M context, 128k max output, adaptive thinking (no extended thinking). |
| 2026-06-30 | Anthropic | **Claude Sonnet 4.6** | 🔄 REPLACED as default by Claude Sonnet 5 (June 30, 2026). Still fully active and not deprecated — pricing unchanged at $3/$15. |
| 2026-07-01 | Anthropic | **Claude Opus 4.7 Fast Mode** | ⚠️ DEPRECATED — Removal scheduled for July 24, 2026. Still billable at $30/$150 (6×) until then. *(Confirmed removed on schedule — see Aug 3, 2026 entry above.)* |
| 2026-07-01 | Anthropic | **Claude Opus 4.6 Fast Mode** | ❌ REMOVED — As of June 29, 2026, `speed: "fast"` requests to Opus 4.6 now run at standard speed/pricing. |
| 2026-07-01 | OpenAI | **GPT-5.6 (Sol/Terra/Luna)** | 🆕 NEW MODEL FAMILY (Restricted Preview) — Announced June 26, 2026. Limited to ~20 trusted partners pending US government review (per June 2, 2026 executive order). Pricing: Sol $5/$30, Terra $2.50/$15, Luna $1/$6 per MTok. New caching model: cache writes at 1.25× uncached input rate, 30-min minimum cache life. *(Superseded by the July 9, 2026 GA entry above, and the Aug 3, 2026 Terra/Luna price cut.)* |
| 2026-06-29 | Mistral | **OCR 4** | 🆕 NEW MODEL — Launched June 23, 2026. $4/1K pages (standard), $2/1K pages (Batch-API 50% off), $5/1K pages (Document AI). `mistral-ocr-latest` alias now points to OCR 4. Adds bounding boxes, block classification, confidence scores, 170-language support. OCR 3 moved to legacy. Source: mistral.ai/news/ocr-4/ |
| 2026-07-01 | Mistral | **Leanstral 1.5** | 🆕 NEW MODEL — Launched June 30, 2026 (Labs, free, 256K context, 119B/6B active MoE). Supersedes original Leanstral (v26.03), which was already in the legacy table since June 15, 2026. |
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
| 2026-06-22 | Anthropic | **Claude Fable 5 + Mythos 5** | 🚫 SUSPENDED — US government issued export control directive June 12, 2026 suspending all access. *(Superseded by the July 1, 2026 restoration above.)* |
| 2026-06-22 | OpenAI | **gpt-realtime-whisper** | 🆕 NEW — Real-time speech recognition model at $0.017/min added to live pricing page. |
| 2026-06-22 | OpenAI | **gpt-realtime-1.5** | ⚠️ MOVED TO LEGACY — No longer listed on live pricing page as of June 2026; still listed as a specialized model on the models page. |
| 2026-06-22 | OpenAI | **gpt-realtime-mini** | ⚠️ MOVED TO LEGACY — No longer listed on live pricing page as of June 2026; still listed as a specialized model on the models page. |
| 2026-06-22 | OpenAI | **gpt-image-1.5** | ⚠️ DEPRECATED — June 2, 2026 notification; API shutdown December 1, 2026. Migrate to gpt-image-2. |
| 2026-06-22 | OpenAI | **gpt-image-1-mini** | ⚠️ DEPRECATED — June 2, 2026 notification; API shutdown December 1, 2026. Migrate to gpt-image-2. |
| 2026-06-22 | OpenAI | **chatgpt-image-latest** | ⚠️ DEPRECATED — June 2, 2026 notification; API shutdown December 1, 2026. Migrate to gpt-image-2. |
| 2026-06-22 | Mistral | **All active models** | ✅ VERIFIED — All active prices re-confirmed unchanged against mistral.ai/pricing. |
| 2026-06-15 | Anthropic | **Claude Sonnet 4** | ⚠️ RETIRED ❌ — `claude-sonnet-4-20250514` API calls now return errors. Migrate to Claude Sonnet 4.6. |
| 2026-06-15 | Anthropic | **Claude Opus 4** | ⚠️ RETIRED ❌ — `claude-opus-4-20250514` API calls now return errors. Migrate to Claude Opus 4.8. |
| 2026-06-15 | Mistral | **Voxtral Mini Transcribe 2** | ✏️ PRICE CORRECTED — $0.002/min → $0.003/min per official mistral.ai/pricing page. |
| 2026-06-15 | Mistral | **Leanstral v26.03** | ⚠️ MOVED TO LEGACY — `labs-leanstral-2603` now in legacy/deprecated table at docs.mistral.ai. |
| 2026-06-15 | Mistral | **Mistral Medium 3.1 v25.08** | ⚠️ FORMALLY DEPRECATED — `mistral-medium-2508` confirmed in legacy table at docs.mistral.ai. |
| 2026-06-09 | Anthropic | **Claude Fable 5** | 🚨 LAUNCHED — $10/$50 per MTok. |
| 2026-06-09 | Anthropic | **Claude Mythos 5** | 🚨 LAUNCHED (limited) — Project Glasswing. |
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
- **Prompt/context caching** discounts apply where noted. Mistral does **not** offer prompt caching. OpenAI's GPT-5.6 generation introduces a new caching model (cache writes at 1.25× uncached input rate).
- Enterprise/volume pricing available from all providers on request.
- **OpenAI GPT-5.6, GPT-5.5, and GPT-5.4** have short-context (<~270K) and long-context (>~270K) pricing tiers.
- **OpenAI service tiers:** Priority → Standard → Batch/Flex (50% off).
- **Google Gemini Pro** models double input cost for prompts >200K tokens.
- **Mistral** processes all API data in the EU by default — GDPR compliance advantage.
- **Anthropic** offers US-only inference at 1.1× pricing via `inference_geo: "us"` parameter.
- **Tool/agent pricing is additive:** Anthropic Web Search ($10/1K searches), Code Execution, and Claude Managed Agents ($0.08/session-hour); OpenAI Web Search ($10–25/1K calls), Computer Use, Containers, and File Search; Mistral Agent API (Web Search/Code Execution at $30/1K calls, Libraries, Image Generation) all bill on top of standard per-model token rates — see each provider's model card for the full tool-pricing tables.
- ⚠️ Models marked **RETIRED** return API errors. **DEPRECATED** = end-of-life published. **LEGACY** = still accessible but in provider's legacy section. **SUSPENDED** = access halted by external directive. **🔄 REPLACED** = superseded by a newer default/recommended model but still active and not deprecated. **🔓 RESTORED** = a previously suspended model has regained access. **📉 PRICE CUT** = confirmed price decrease on an active model.
- 🆕 **Unpriced/discovery-only items** (e.g., OpenAI's GPT-Live voice models, Mistral's Robostral Navigate and upcoming open-weight model family) are noted for awareness but are **not** given a full tracked model card until the provider publishes official pricing/specs, per this tracker's verification-before-tracking policy.
- 🔓 **Claude Fable 5 + Mythos 5 RESTORED July 1 / June 26, 2026** — the US government export control directive from June 12, 2026 was lifted June 30, 2026 after Anthropic deployed an improved safety classifier. See [Anthropic's "Redeploying Fable 5" post](https://www.anthropic.com/news/redeploying-fable-5).
- ✅ **Claude Sonnet 4 + Opus 4 RETIRED June 15, 2026 ❌** on the Claude API (still available on Bedrock/Google Cloud per Anthropic's deprecation policy).
- 🆕 **July 24, 2026:** Claude Opus 5 launched, replacing Opus 4.8 as the default on Claude Max/strongest on Pro at identical $5/$25 pricing.
- ✅ **July 20, 2026:** Claude Fable 5's subscription-tier cliff permanently resolved — Max/Team Premium keep 50%-of-limits included access; Pro/Team Standard moved to metered usage credits.
- ✅ **July 24, 2026 (confirmed Aug 3):** Claude Opus 4.7's Fast Mode removal took effect as scheduled — `speed: "fast"` requests now return an error.
- 🆕 **July 9, 2026:** GPT-5.6 (Sol/Terra/Luna) reached General Availability — now OpenAI's current flagship family, replacing GPT-5.5 as the recommended top-tier model (GPT-5.5 remains active/not deprecated at the same price).
- 🆕 **July 8, 2026:** OpenAI launched GPT-Live-1/GPT-Live-1 mini, full-duplex voice models bundled into ChatGPT plans (no API pricing yet). Mistral published Robostral Navigate, an unpriced embodied-navigation robotics model.
- 📉 **August 3, 2026:** GPT-5.6 Terra and Luna both got significantly cheaper (Terra: $2.50/$15.00 → $2.00/$12.00; Luna: $1.00/$6.00 → $0.20/$1.20, ~80% off). Two new OpenAI transcription models discovered (`gpt-transcribe`, `gpt-live-transcribe`).
- 🆕 **June 30, 2026:** Claude Sonnet 5 launched, replacing Sonnet 4.6 as Anthropic's default Sonnet-tier model (intro pricing $2/$10 thru Aug 31, 2026). Mistral Leanstral 1.5 launched, replacing v26.03. US export controls on Fable 5/Mythos 5 lifted.
- 🆕 **July 1, 2026:** Claude Fable 5 restored globally.
- 🆕 **June 26, 2026:** OpenAI previewed GPT-5.6 (Sol/Terra/Luna) in restricted preview (~20 trusted partners, US government coordination) — later reached GA on July 9, 2026 (see above).
- 🆕 **June 29, 2026:** Mistral OCR 4 launched ($4/1K pages); Mistral Small 4 price +50%/+100% to $0.15/$0.60; Voxtral Mini 3B deprecated; OpenAI Pro model batch pricing documented.
- 📝 **July 14, 2026:** Independently re-verified Anthropic, OpenAI, and Mistral pricing directly against each provider's live pricing/docs pages. Key changes: **GPT-5.6 reached GA** (July 9) and is now the flagship OpenAI family; OpenAI Realtime models refreshed to `gpt-realtime-2.1`/`2.1-mini`; Mistral's **Leanstral 1.5 model ID corrected** to `leanstral-1-5`; Anthropic's Fable 5 subscription-included window has been extended twice (now reported as July 19) and Anthropic began localizing consumer (not API) pricing for India.
- 📝 **July 20, 2026:** This refresh independently re-verified Anthropic, OpenAI, and Mistral pricing line-by-line against each provider's live pricing/docs pages — **no price changes detected on any of the three Tier 1 providers covered this cycle.** Newly documented: Anthropic's full Tools & Agents pricing (Web Search, Code Execution, Claude Managed Agents, tool-use system-prompt overhead); Mistral's Agent API tool pricing was cross-verified and a stale marketing-FAQ example (an outdated "$2/$6" Mistral Large figure) was flagged and resolved against the authoritative product pricing table (Large 3 confirmed unchanged at $0.50/$1.50). Google Gemini and OpenRouter Picks tables reflect the last confirmed figures from a prior refresh and were not re-verified this cycle.
- 📝 **July 27, 2026:** This refresh independently re-verified Anthropic, OpenAI, and Mistral pricing against each provider's live pricing/docs pages and independent reporting. **Key changes:** Anthropic launched **Claude Opus 5** (July 24, 2026, $5/$25, replaces Opus 4.8 as the Max default/strongest-on-Pro model) and **permanently resolved** the Fable 5 subscription-tier cliff (July 20, 2026 — Max/Team Premium keep 50%-of-limits included access; Pro/Team Standard moved to metered usage credits with a one-time $100 credit). OpenAI launched **GPT-Live-1/GPT-Live-1 mini** (July 8, 2026), full-duplex ChatGPT voice models with no API pricing published yet — flagged as discovery-only. Mistral's **Leanstral 1.5 now has a published retirement date (September 30, 2026)**, and a new, larger open-weight MoE model family was flagged as a watch item (early access starting July 2026, no pricing/specs published — not yet added as a tracked model). No pricing changes detected on any existing Tier 1 model this cycle. Google Gemini and OpenRouter Picks tables reflect the last confirmed figures from a prior refresh and were not re-verified this cycle.
- 📝 **August 3, 2026:** This refresh independently re-verified Anthropic, OpenAI, and Mistral pricing against each provider's live pricing/docs pages and news feeds. **Key changes:** OpenAI cut prices on **GPT-5.6 Terra** ($2.50/$15.00 → $2.00/$12.00) and **GPT-5.6 Luna** ($1.00/$6.00 → $0.20/$1.20, ~80% off), and two new transcription models were discovered (`gpt-transcribe` at $0.0045/min, `gpt-live-transcribe` at $0.017/min); GPT-5.6 Sol, GPT-5.5, GPT-5.5 Pro, and the GPT-5.4 family remain unchanged. Anthropic confirmed that **Claude Opus 4.7's Fast Mode removal**, previously scheduled for July 24, 2026, has taken effect (the live pricing page now returns an error for `speed: "fast"` requests against Opus 4.7); Claude Opus 5's tool-use overhead (286/406 tokens, the cheapest of any active model) was also newly captured. No new Anthropic model releases were found since Claude Opus 5. Mistral's pricing was fully re-confirmed unchanged; a new robotics release, **Robostral Navigate** (July 8, 2026, 8B embodied-navigation model), was flagged as a discovery-only item since it has no published API pricing. Google Gemini and OpenRouter Picks tables reflect the last confirmed figures from a prior refresh and were not re-verified this cycle.
