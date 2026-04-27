# 🤖 LLM Pricing Tracker

Up-to-date pricing and specifications for large language models from **Anthropic**, **OpenAI**, **Google Gemini**, **Mistral AI**, and top **OpenRouter picks**.

> **Last updated:** 2026-04-27 (refresh #9)  
> **Sources:** Official provider pricing pages + third-party verification — scraped/verified on date above.

---

## 📋 Quick-Reference Index — Active Models

### 🟠 Tier 1 — Anthropic Claude

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Claude Opus 4.7** *(Current Flagship)* | $5.00 | $25.00 | **1M tokens** | API, AWS Bedrock (all regions), Vertex AI, MS Foundry, GitHub Copilot Pro+ |
| Claude Opus 4.6 *(prev flagship)* | $5.00 | $25.00 | **1M tokens** | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Sonnet 4.6** | $3.00 | $15.00 | **1M tokens** | API, AWS Bedrock, Vertex AI, MS Foundry |
| **Claude Haiku 4.5** | $1.00 | $5.00 | 200K tokens | API, AWS Bedrock (all regions), Vertex AI, MS Foundry |
| Claude Opus 4.5 | $5.00 | $25.00 | 200K tokens | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Sonnet 4.5 ⏰ | $3.00 | $15.00 | 200K tokens *(1M beta retiring Apr 30 — 3 days!)* | API, AWS Bedrock, Vertex AI, MS Foundry |
| Claude Haiku 3.5 *(prev-gen, still active)* | $0.80 | $4.00 | 128K tokens | API, AWS Bedrock, Vertex AI |

> 💡 Batch API: 50% off · Prompt caching: up to 90% off · Opus 4.7/4.6 Fast Mode: $30/$150 (6× base)  
> ⏰ **Claude Sonnet 4.5 1M context beta retires April 30, 2026 (3 days!)** — migrate to Sonnet 4.6  
> 🔒 Claude Mythos Preview (Project Glasswing) — restricted access only; no public API  

---

### 🟢 Tier 1 — OpenAI (Proprietary)

| Model | Input ($/MTok) | Cached Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|---|
| **GPT-5.5** 🆕 *(Current Flagship)* | $5.00 | $0.50 | $30.00 | 1M tokens | API |
| **GPT-5.5 Pro** 🆕 | $30.00 | — | $180.00 | 1M tokens | API |
| GPT-5.4 *(prev flagship)* | $2.50 / $5.00* | $0.25 / $0.50* | $15.00 / $22.50* | 1.05M tokens | API |
| GPT-5.4 Pro *(prev ultra-premium)* | $30.00 | — | $180.00 | 1.05M tokens | API |
| **GPT-5.4 mini** | $0.75 | $0.075 | $4.50 | 400K tokens | API |
| **GPT-5.4 nano** | $0.20 | $0.020 | $1.25 | 400K tokens | API |
| GPT-4.1 | $2.00 | $0.50 | $8.00 | 1.04M tokens | API |
| **GPT-4.1 mini** | $0.40 | $0.10 | $1.60 | 1.00M tokens | API |
| GPT-4.1 nano | $0.10 | — | $0.40 | 1M+ tokens | API |
| o3 *(reasoning)* | $2.00 | $0.50 | $8.00 | 200K tokens | API |
| o3-pro *(reasoning)* | $20.00 | — | $80.00 | 200K tokens | API |
| o4-mini *(reasoning)* | $1.10 | $0.275 | $4.40 | 200K tokens | API |

> 💡 Batch API: 50% off all models · Cached inputs: 50–90% off · Regional processing: +10% on GPT-5.5 and GPT-5.4 family  
> *GPT-5.4 tiered pricing: short ctx (<272K) / long ctx (>272K) — standard rates below 272K  
> 🆕 **GPT-5.5 released April 23-24, 2026** — new flagship; $5/$30 per MTok (2× GPT-5.4); first full retrain since GPT-4.5; AI Index #1 (score 60); Terminal-Bench 2.0 82.7%  
> 🔒 GPT-5.4-Cyber announced April 14 — limited vetted access only; no public API pricing

---

### 🔵 Tier 1 — Google Gemini

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Notes |
|---|---|---|---|---|
| **Gemini 3.1 Pro Preview** | $2.00 / $4.00* | $12.00 / $18.00* | **1M tokens** | *Tiered at >200K; Preview |
| **Gemini 3.1 Flash-Lite Preview** | $0.25 | $1.50 | **1M tokens** | Preview |
| **Gemini 2.5 Pro** | $1.25 / $2.50* | $10.00 / $15.00* | **1M tokens** | *Tiered at >200K; GA |
| **Gemini 2.5 Flash** | $0.30 | $2.50 | **1M tokens** | GA; optional thinking mode |
| **Gemini 2.5 Flash-Lite** | $0.10 | $0.40 | **1M tokens** | GA; cheapest Gemini |
| Gemini 2.0 Flash | $0.10 | $0.40 | 1M tokens | Active; prev-gen |

> 💡 Batch API: 50% off · Context caching: 90% off repeated prefixes · Free tier via AI Studio · Pro models: double input cost for prompts >200K

---

### 🟡 Tier 1 — Mistral AI

| Model | Input ($/MTok) | Output ($/MTok) | Context Window | Availability |
|---|---|---|---|---|
| **Mistral Large 3 (2512)** | $0.50 | $1.50 | 256K tokens | API (Mistral AI Studio) |
| **Magistral Medium 1.2** 🆕 | $2.00 | $5.00 | 128K tokens *(best <40K)* | API (Mistral AI Studio) |
| **Magistral Small 1.2** 🆕 | $0.50 | $1.50 | 128K tokens *(best <40K)* | API (Mistral AI Studio) |
| Mistral Medium 3.1 | $0.40 | $2.00 | 131K tokens | API (Mistral AI Studio) |
| **Mistral Small 4** *(Mar 2026)* | $0.15 | $0.60 | **256K tokens** | API (Mistral AI Studio) |
| Codestral 2508 | $0.30 | $0.90 | 256K tokens | API (Mistral AI Studio) |
| **Devstral 2 (2512)** ✏️ | $0.40 | $0.90 *(corrected from $2.00)* | 256K tokens *(corrected from 128K)* | API (Mistral AI Studio) |
| Devstral Small 1.1 | $0.07 | $0.28 | 128K tokens | API (Mistral AI Studio) |
| Mistral Small Creative 🆕 | $0.10 | $0.30 | 33K tokens | API (Mistral AI Studio) |
| Voxtral Small 24B | $0.10 | $0.30 | 128K tokens | API (Mistral AI Studio) |
| Voxtral TTS 🆕 | TBD | TBD | — | API (Mistral AI Studio) |
| Mistral Nemo | $0.15 | $0.15 | 128K tokens | API (Mistral AI Studio) |
| Ministral 14B | $0.20 | $0.20 | 256K tokens | API (Mistral AI Studio) |
| Ministral 8B | $0.10 | $0.10 | 256K tokens | API (Mistral AI Studio) |
| Ministral 3B | $0.10 | $0.10 | 556K tokens | API (Mistral AI Studio) |

> 💡 EU data residency by default · Free experimentation tier · Open-weight models (Apache 2.0) for self-hosting  
> 🆕 **Mistral Small Creative** added (Dec 2025) — experimental creative writing model, $0.10/$0.30, 33K context  
> ✏️ **Devstral 2 corrected:** output $2.00 → **$0.90/MTok**; context 128K → **256K** (per pricepertoken.com Apr 23 + Artificial Analysis)  
> ✏️ **Magistral Small/Medium context confirmed:** 128K tokens each (optimal performance below 40K)

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
| Anthropic | 1 | [anthropic.md](./anthropic.md) | Full model cards incl. caching, batch, fast mode, deprecation dates |
| OpenAI | 1 | [openai.md](./openai.md) | Full model cards incl. context tiers, reasoning models, batch pricing |
| Google Gemini | 1 | [gemini.md](./gemini.md) | Full model cards incl. context tiers, thinking tokens, free tier |
| Mistral AI | 1 | [mistral.md](./mistral.md) | Full model cards incl. Magistral reasoning, open-weight models, EU compliance |
| OpenRouter Picks | 2 | [openrouter-picks.md](./openrouter-picks.md) | One best-performing model per Tier 2 provider, all via OpenRouter |

---

## ⚠️ Legacy / Deprecated / Retired Models

> These models are no longer recommended for new deployments.

### 🟠 Anthropic — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ Claude Sonnet 4 | **DEPRECATED · Retiring Jun 15, 2026** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude Opus 4.1 | LEGACY | $15.00 | $75.00 | → Claude Opus 4.7 (67% cheaper) |
| ⚠️ Claude Opus 4 | **DEPRECATED · Retiring Jun 15, 2026** | $15.00 | $75.00 | → Claude Opus 4.7 |
| ⚠️ Claude Haiku 3 | **RETIRED April 19-20, 2026 ❌ API ERRORS** | $0.25 | $1.25 | → Claude Haiku 4.5 |
| ⚠️ Claude Sonnet 3.7 | **DEPRECATED** (API accessible; no new projects) | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 3 Opus | **DEPRECATED** (API accessible; phasing out) | $15.00 | $75.00 | → Claude Opus 4.7 |
| ⚠️ Claude 3.5 Sonnet | **RETIRED** | $3.00 | $15.00 | → Claude Sonnet 4.6 |
| ⚠️ Claude 2.x | **RETIRED** | ~$8.00 | ~$24.00 | → Claude Sonnet 4.6 |

### 🟢 OpenAI — Legacy

| Model | Status | Input ($/MTok) | Output ($/MTok) | Migration Target |
|---|---|---|---|---|
| ⚠️ GPT-5.4 Pro | LEGACY · Superseded by GPT-5.5 Pro | $30.00 | $180.00 | → GPT-5.5 Pro (same price, better performance) |
| ⚠️ GPT-5.3 / Codex | LEGACY · Phasing out Jun 2026 | $1.75 | $14.00 | → GPT-5.5 or GPT-5.4 |
| ⚠️ GPT-5.2 | LEGACY · Retiring Jun 2026 (Thinking: Jun 5) | $1.75 | $14.00 | → GPT-5.4 or GPT-5.5 |
| ⚠️ GPT-5.1 | **RETIRED March 11, 2026** | — | — | → GPT-5.5 |
| ⚠️ GPT-4o | LEGACY | $2.50 | $10.00 | → GPT-4.1 (cheaper, 1M ctx) |
| ⚠️ GPT-4o mini | LEGACY | $0.15 | $0.60 | → GPT-5.4 nano or GPT-4.1 nano |
| ⚠️ o1 | LEGACY (very expensive) | $15.00 | $60.00 | → o3 (87% cheaper) |
| ⚠️ GPT-4 Turbo | **RETIRED** | — | — | → GPT-4.1 |
| ⚠️ GPT-3.5 Turbo | **RETIRED** | — | — | → GPT-4.1 nano |

### 🔵 Google Gemini — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ Gemini 3 Pro Preview | **RETIRED** March 9, 2026 | → Gemini 3.1 Pro Preview |
| ⚠️ Gemini 2.0 Flash-Lite | **DEPRECATED · Shutdown June 1, 2026** | → Gemini 2.5 Flash-Lite |
| ⚠️ Gemini 1.5 Pro | LEGACY | → Gemini 2.5 Pro |
| ⚠️ Gemini 1.5 Flash | LEGACY | → Gemini 2.5 Flash |

### 🟡 Mistral AI — Legacy

| Model | Status | Migration Target |
|---|---|---|
| ⚠️ Devstral Medium | LEGACY · Superseded by Devstral 2 (Dec 2025) | → Devstral 2 ($0.40/$0.90 — same input, 55% cheaper output) |
| ⚠️ Mistral Small 3.2 24B | LEGACY · Superseded Mar 2026 | → Mistral Small 4 |
| ⚠️ Mistral Small 3.1 | LEGACY · Superseded Jun 2025 | → Mistral Small 4 |
| ⚠️ Mistral Large 2 (2407) | LEGACY | → Mistral Large 3 |
| ⚠️ Mistral Medium 3 (original) | LEGACY · Superseded Aug 2025 | → Mistral Medium 3.1 |
| ⚠️ Codestral 2501 | LEGACY · Superseded Aug 2025 | → Codestral 2508 |
| ⚠️ Mixtral 8×7B (API) | LEGACY (still self-hostable) | → Mistral Medium 3.1 (API) |

---

## 🏷️ Price Change Log

| Date | Provider | Model | Change |
|---|---|---|---|
| 2026-04-27 | Mistral | **Devstral 2 (2512)** | ✏️ CORRECTION — Output price updated $2.00 → **$0.90/MTok** (source: pricepertoken.com Apr 23, 2026; prior $2.00 was carried over from legacy Devstral Medium). Context window corrected 128K → **256K** (source: Artificial Analysis). |
| 2026-04-27 | Mistral | **Magistral Medium 1.2 & Small 1.2** | ✏️ Context window confirmed as **128K tokens** (optimal performance below 40K per OpenRouter). Model ID corrected to `magistral-medium-2509` (Sep 2025 release). |
| 2026-04-27 | Mistral | **Mistral Small Creative** | 🆕 ADDED — Experimental creative writing model; $0.10/$0.30 per MTok; 33K context; released Dec 16, 2025; confirmed on OpenRouter Apr 2026. Not a general-purpose model — use Mistral Small 4 for broad tasks. |
| 2026-04-27 | Anthropic | **Claude Sonnet 4.5 1M beta** | ⏰ Countdown updated — 1M context beta now retires in **3 days** (April 30, 2026). Migrate to Sonnet 4.6. |
| 2026-04-25 | OpenAI | **GPT-5.5** | 🆕 LAUNCHED April 23-24, 2026 — $5.00/$30.00 per MTok (2× GPT-5.4 price); 1M context; first fully retrained base since GPT-4.5; natively omnimodal; Terminal-Bench 2.0 82.7% (#1); AI Index score 60 (#1, +3 pts vs Opus 4.7 & Gemini 3.1 Pro); now available in API as of April 24. |
| 2026-04-25 | OpenAI | **GPT-5.5 Pro** | 🆕 LAUNCHED April 24, 2026 — $30.00/$180.00 per MTok; 1M context; same price as GPT-5.4 Pro with better benchmarks; BrowseComp 90.1%. |
| 2026-04-25 | OpenAI | **GPT-5.4** | Status updated to Previous Flagship (superseded by GPT-5.5). Still active and recommended for cost-sensitive workloads. |
| 2026-04-25 | OpenAI | **GPT-5.4 Pro** | ⚠️ Moved to legacy — superseded by GPT-5.5 Pro at identical pricing ($30/$180) with better benchmarks. |
| 2026-04-25 | OpenAI | **o3-pro** | ✅ ADDED — $20.00/$80.00 per MTok; maximum reasoning depth; 200K context. |
| 2026-04-25 | Anthropic | **Claude Haiku 3** | ⚠️ RETIRED April 19-20, 2026 — All API calls return errors. No automatic fallback. Migrate to Haiku 4.5. |
| 2026-04-25 | Anthropic | **Claude Sonnet 4.5** | ⏰ URGENT — 1M context beta (`context-1m-2025-08-07`) retires April 30, 2026. Migrate to Sonnet 4.6. |
| 2026-04-25 | Anthropic | **Managed Agents Memory** | 🆕 PLATFORM — Memory for Claude Managed Agents now in public beta (`managed-agents-2026-04-01`). Billed at standard token rates. |
| 2026-04-25 | Mistral | **Magistral Medium** | 🆕 ADDED — $2.00/$5.00 per MTok; 128K context (best <40K); Mistral's reasoning model comparable to o3; chain-of-thought; multilingual. |
| 2026-04-25 | Mistral | **Magistral Small 1.2** | 🆕 ADDED — $0.50/$1.50 per MTok; budget reasoning model; same pricing as Mistral Large 3. |
| 2026-04-25 | Mistral | **Mistral Small 4** | ✏️ CORRECTED context window: 128K → **262,144 tokens / 256K** (confirmed via OpenRouter listing Apr 2026). Output price confirmed at $0.60. |
| 2026-04-25 | Mistral | **Devstral Medium** | ⚠️ ADDED to legacy — July 2025 model superseded by Devstral 2. |
| 2026-04-16 | Anthropic | **Claude Opus 4.7** | 🆕 LAUNCHED — $5/$25 per MTok (same as Opus 4.6). New: xhigh effort level, task budgets (beta), /ultrareview (Claude Code, 3 free reviews at launch), 3.75MP vision (2,576px), new tokenizer (up to 35% more tokens/request vs Opus 4.6). SWE-bench Verified 87.6%, GPQA Diamond 94.2%. Available on API, Bedrock (all regions, self-serve), Vertex AI, MS Foundry, GitHub Copilot Pro+. |
| 2026-04-16 | Anthropic | **Claude Opus 4.6** | Status updated to Previous Flagship (superseded by Opus 4.7). Still active and available. |
| 2026-04-16 | Mistral | **Voxtral TTS** | 🆕 NOTED — First Mistral TTS model launched March 23, 2026. API pricing not yet published in per-MTok format. Added as awareness item in mistral.md. |
| 2026-04-15 | Anthropic | **Claude Sonnet 4** | ⚠️ DEPRECATED — Retirement scheduled June 15, 2026. Migrate to Sonnet 4.6. |
| 2026-04-15 | Anthropic | **Claude Opus 4** | ⚠️ DEPRECATED — Retirement scheduled June 15, 2026. Migrate to Opus 4.7. |
| 2026-04-15 | Anthropic | **Claude Mythos Preview** | 🔒 Announced April 7 — restricted access only (Project Glasswing cybersecurity initiative). No public API. |
| 2026-04-15 | OpenAI | **GPT-5.4-Cyber** | 🔒 Announced April 14 — limited vetted access only. Not available via public API. |
| 2026-04-15 | OpenAI | **GPT-5.1** | ⚠️ RETIRED March 11, 2026. Added to legacy section. |
| 2026-04-15 | Mistral | **Mistral Small 4** | ✅ ADDED — Released March 16, 2026; `mistral-small-latest` now routes here |
| 2026-04-15 | Mistral | **Codestral 2508** | ✅ UPDATED — Version 2508 (Aug 2025) at $0.30/$0.90; 70% cheaper than old Codestral 2501 ($1.00/$3.00) |
| 2026-04-13 | Anthropic | **Claude Haiku 3.5** | ✏️ CORRECTED — Restored to Active ($0.80/$4); was incorrectly marked RETIRED. |
| 2026-04-13 | Anthropic | **Claude Sonnet 3.7** | ✏️ CORRECTED — Status updated to DEPRECATED (not RETIRED). |
| 2026-04-13 | OpenAI | **GPT-4.1 mini** | ✅ ADDED — $0.40/$1.60 per MTok; 1M context. |
| 2026-04-12 | Google | **Gemini 3.1 Pro Preview** | ✅ Added — $2/$12 (≤200K), $4/$18 (>200K), 1M context |
| 2026-04-12 | Google | **Gemini 2.0 Flash-Lite** | ⚠️ DEPRECATED — shutting down June 1, 2026 |
| 2026-04-12 | OpenRouter | **gpt-oss-120b** | ✅ Added — $0.039/$0.19, 131K context |
| 2026-04-12 | OpenRouter | **DeepSeek V3.2** | ✅ Added — $0.26/$0.38, 163K context |
| 2026-04-12 | OpenRouter | **Qwen3.6 Plus** | ✅ Added — free preview (April 2026); paid pricing TBD |
| 2026-04-12 | OpenRouter | **Nemotron 3 Super 120B** | ✅ Added — $0.10/$0.50, 262K context |
| 2026-04-12 | OpenRouter | **MiniMax M2.7** | ✅ Added — $0.30/$1.20, 205K context |
| 2026-04-12 | OpenRouter | **Grok 4.1 Fast** | ✅ Added — $0.20/$0.50, 2M context |
| 2026-04-11 | Anthropic | **Claude Opus 4.6** | ✅ Confirmed $5/$25 · 1M context at standard pricing · Fast Mode $30/$150 |
| 2026-04-11 | Anthropic | **Claude Sonnet 4.6** | ✅ Confirmed $3/$15 · 1M context standard |
| 2026-04-11 | OpenAI | **GPT-5.4 family** | ✅ Confirmed launch Mar 5, 2026 · $2.50/$15 (short), $5/$22.50 (long ctx >272K) |
| 2026-04-11 | Mistral | **Mistral Large 3** | ✅ Confirmed $0.50/$1.50 at 256K context |

---

## ℹ️ Notes
- All prices are in **USD** and listed **per million tokens (MTok)**.
- **Batch API discounts (50%)** are available from Anthropic, OpenAI, and Google Gemini. Mistral does **not** currently offer a batch discount tier.
- **Prompt/context caching** discounts apply where noted. Mistral does **not** offer prompt caching.
- Enterprise/volume pricing is available from all providers on a negotiated basis.
- **OpenAI GPT-5.4** uses short context (<272K) and long context (>272K) pricing tiers. **GPT-5.5 is flat-rate** with no context tier surcharge.
- **Google Gemini Pro** models (2.5 Pro, 3.1 Pro) double input cost for prompts >200K tokens.
- **Mistral** processes all API data in the EU by default — key compliance advantage for GDPR workloads.
- **Anthropic** offers US-only inference (data residency) at 1.1× pricing for models released after February 1, 2026.
- **Tier 2 OpenRouter Picks** use OpenRouter prices which are typically at or near direct provider API rates.
- ⚠️ Models marked **RETIRED** return API errors. Models marked **DEPRECATED** have a known retirement date or are actively phasing out but may still be API-accessible.
- ✏️ **Correction policy:** When verified data from official pricing pages contradicts a prior entry, the old entry is corrected and logged in the Price Change Log above.
- 🔒 **Restricted models** (Mythos Preview, GPT-5.4-Cyber) are real models with no public API or general pricing — noted for awareness only.
- ⚠️ **Claude Opus 4.7 tokenizer change:** New tokenizer may produce up to 35% more tokens for the same text vs Opus 4.6. Per-token price is unchanged at $5/$25, but monitor per-request costs during migration.
- ⚠️ **GPT-5.5 price increase:** $5/$30 is 2× GPT-5.4 ($2.50/$15) per token. OpenAI claims ~40% token efficiency improvement for Codex tasks, netting ~20% higher effective cost. Measure on your own workloads before migrating.
- 🆕 **Mistral Magistral:** Mistral's reasoning model line (Medium 1.2 at $2/$5, Small 1.2 at $0.50/$1.50) is now tracked. These are comparable to OpenAI's o-series.
- ✏️ **Devstral 2 correction (Apr 27):** Output price corrected from $2.00 to $0.90/MTok; context corrected from 128K to 256K. The prior $2.00 figure was from the legacy Devstral Medium (Jul 2025), not Devstral 2 (Dec 2025).
