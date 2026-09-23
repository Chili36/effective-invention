# 🔵 Mistral AI — Model Cards

> **Last updated:** 2026-09-23
> **Source:** https://mistral.ai/pricing · https://docs.mistral.ai/inference/pricing · https://docs.mistral.ai/getting-started/models/models_overview/ · https://docs.mistral.ai/inference/model-lifecycle · https://mistral.ai/news · https://docs.mistral.ai/resources/changelogs
> **Scraped / verified:** 2026-09-23 — ✅ **Re-verified against the live `mistral.ai/pricing/api`, `docs.mistral.ai/inference/pricing`, and `mistral.ai/news` pages through September 23, 2026.** Every active model price (Mistral Large 3 $0.50/$1.50, Medium 3.5 $1.50/$7.50, Small 4 $0.15/$0.60, Ministral 3 tiers, Codestral, Codestral Embed, OCR 4.1/4.0, Voxtral TTS/Transcribe 2, Moderation 2 Free, Z.ai GLM-5.2/5.3, Leanstral 1.5 Free) matches the September 22 refresh byte-for-byte. Checked `mistral.ai/news` — **no new posts since the Sept 16 Mozilla partnership**; no new priced model releases, retirements, or price changes found this cycle.

> 🆕 **September 21, 2026 refresh — key findings (still current):**
> 1. ⚠️ **CORRECTION: Devstral 2, Devstral Small 2, and the entire Magistral family (Medium 1.0/1.1/1.2, Small 1.0/1.1/1.2) are RETIRED, not active.** Official confirmation via `docs.mistral.ai/getting-started/models/models_overview` "Deprecated & retired models" table plus third-party lifecycle tracking: these models — along with **Mistral Small 3.2** and **Mistral NeMo 12B** — were retired **July 31, 2026**, superseded by **Mistral Small 4** (`reasoning_effort: high` covers Magistral Small / Devstral Small use cases) and **Mistral Medium 3.5** (covers Magistral Medium / Devstral use cases). Prior refreshes of this tracker incorrectly carried these as "Active via `-latest` alias" — this was stale; the `-latest` aliases for these families no longer resolve to a supported model. **All moved to the Legacy/Retired section below.**
> 2. ⚠️ **CORRECTION: Mistral Medium 3 and Medium 3.1 are RETIRED (August 31, 2026)**, not merely "Legacy" — both fully retired in favor of Mistral Medium 3.5.
> 3. 🆕 **Z.ai GLM-5.3 added to Mistral's platform (~September 15, 2026)** — Mistral's **second** third-party hosted open model, public preview, same pricing as GLM-5.2 ($1.40/$4.40 per MTok, 1M context). New aliases `zai-glm-5` and `zai-glm-latest` now point to GLM-5.3; GLM-5.2 remains available side-by-side (not deprecated).
> 4. 🆕 **Cached-input pricing now published for Mistral's own native models** — a first. The live pricing page now shows a **90%-off cached-input rate (0.1× multiplier)** across Mistral Large 3 ($0.05/MTok cached), Mistral Medium 3.5 ($0.15/MTok cached), Mistral Small 4 ($0.015/MTok cached), all three Ministral 3 tiers, Codestral, Codestral Embed, OCR 4.1/4.0 ($0.40/1,000 pages cached), and Voxtral Mini Transcribe 2 ($0.0003/min cached). This corrects prior refreshes' statement that "Mistral's own models do NOT offer prompt caching" — that is no longer accurate.
> 5. 📉 **Mistral Moderation 2 is listed as Free** on the live pricing page (previously tracked at $0.10/MTok — correcting to Free).
> 6. ℹ️ Checked `mistral.ai/news` through September 21, 2026: **Sept 16** — "Mistral and Mozilla are bringing open, private and multilingual AI to your web browser" (Firefox Smart Window partnership — product integration, non-pricing). No new priced LLM releases beyond GLM-5.3 found this cycle.

All prices are **USD per million tokens (MTok)** unless noted. Mistral offers a **free experimentation tier** (rate-limited) — no credit card required to start. API and consumer (Vibe) subscriptions are billed **separately**. Batch API gives a flat **50% discount**; cached input tokens are now broadly available at **90% off** across both native and third-party-hosted models.

> **Mistral's key differentiators:** Native EU data residency (GDPR by default) paired with GA'd regional endpoint choice (EU or US), competitive mid-tier pricing, Apache 2.0 / Modified MIT open-weight models, dedicated reasoning and coding capability now folded into Small 4 / Medium 3.5, a growing **third-party open-model marketplace** (GLM-5.2, GLM-5.3), and a 50% batch processing discount.

---

## ✅ Active / Recommended Models

### 🆕 Z.ai GLM-5.3 *(Third-Party Open Model — Added to Mistral's Platform ~September 15, 2026)*

> Mistral's **second** third-party hosted open model after GLM-5.2, running unmodified on Mistral's infrastructure under the same regional controls and SLA commitments as native Mistral models. Public preview.

| Field | Value |
|---|---|
| **Provider** | Z.ai *(hosted on Mistral AI Studio)* |
| **Model ID** | `zai-glm-5-3` — aliases `zai-glm-5` and `zai-glm-latest` now point to it |
| **Added to Mistral** | ~September 15, 2026 |
| **Status** | ✅ Active — Public Preview — **Second third-party open model on Mistral's platform** |
| **Input price** | $1.40 / MTok |
| **Cached input price** | $0.14 / MTok *(90% off)* |
| **Output price** | $4.40 / MTok |
| **Context window** | 1,000,000 tokens |
| **License** | Open |
| **Availability** | Mistral AI Studio / La Plateforme, with EU/US Regional Endpoint choice and Priority Tier support |
| **Notable** | Same pricing as GLM-5.2; GLM-5.2 remains available and is not deprecated. `zai-glm-latest` now resolves to 5.3 — pin `zai-glm-5-2` explicitly if you need the older snapshot |

---

### Z.ai GLM-5.2 *(Third-Party Open Model — still active alongside GLM-5.3)*

| Field | Value |
|---|---|
| **Provider** | Z.ai *(hosted on Mistral AI Studio)* |
| **Model ID** | `zai-glm-5-2` |
| **Added to Mistral** | August 11, 2026 |
| **Status** | ✅ Active — first third-party open model on Mistral's platform; not deprecated by GLM-5.3 |
| **Input price** | $1.40 / MTok |
| **Cached input price** | $0.14 / MTok *(90% off)* |
| **Output price** | $4.40 / MTok |
| **Context window** | 1,000,000 tokens |
| **Notable** | Specializes in long-context agentic workflows and coding. Note: the `zai-glm-latest` alias now points to GLM-5.3, not 5.2 — pin `zai-glm-5-2` if you need this exact version |

---

### Mistral Medium 3.5 *(Flagship — Released April 29, 2026)*

> Now Mistral's unified flagship for reasoning, agentic coding, and vision — absorbing the use cases previously split across Magistral Medium (reasoning) and Devstral 2 (agentic coding), both now retired (see Legacy section).

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-medium-latest` |
| **Released** | April 29, 2026 |
| **Status** | ✅ Active — **Flagship** |
| **Input price** | $1.50 / MTok |
| **Cached input price** | 🆕 $0.15 / MTok *(90% off — newly published)* |
| **Output price** | $7.50 / MTok |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio / La Plateforme); NVIDIA NIM; open weights on HuggingFace (modified MIT license) |
| **Capabilities** | Text, Vision, Function Calling, JSON mode, Configurable reasoning effort (`reasoning_effort`), Agentic coding, 24-language support |
| **Notable** | First Mistral flagship merged model; 128B dense; SWE-Bench Verified 77.6%; default model for Mistral Vibe CLI and Le Chat Work Mode. Use `reasoning_effort=high` for Magistral Medium-class reasoning depth, and for Devstral/agentic-coding-class workloads |

---

### Mistral Large 3 (2512)

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-large-latest` |
| **Status** | ✅ Active — General Reasoning Flagship, Open-weight |
| **Input price** | $0.50 / MTok |
| **Cached input price** | 🆕 $0.05 / MTok *(90% off — newly published)* |
| **Output price** | $1.50 / MTok |
| **Context window** | 262,144 tokens (256K) |
| **Notable** | Cheapest output pricing vs peers; GDPR-compliant EU hosting; open-weight, general-purpose multimodal model. Do not confuse with the stale "$2/$6" example still floating on the general `mistral.ai/pricing` FAQ page — always price off the `mistral.ai/pricing/api` product table |

---

### Mistral Small 4 *(Released March 16, 2026)*

> Now Mistral's unified budget model for reasoning, coding, and vision — absorbing the use cases previously split across Magistral Small (reasoning) and Devstral Small 2 (agentic coding), both now retired (see Legacy section).

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-small-latest` |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.15 / MTok |
| **Cached input price** | 🆕 $0.015 / MTok *(90% off — newly published)* |
| **Output price** | $0.60 / MTok |
| **Context window** | 262,144 tokens (256K) |
| **Capabilities** | Text, Vision, Function Calling, Reasoning (`reasoning_effort`), Agentic, Coding |
| **Notable** | Hybrid model unifying instruct, reasoning, and coding in a single efficient model; multimodal reasoning; configurable `reasoning_effort` (none → high) now the recommended replacement for both Magistral Small and Devstral Small 2 |

---

### Codestral 2508 *(Updated August 2025)*

| Field | Value |
|---|---|
| **Model ID** | `codestral-latest` |
| **Status** | ✅ Active — Specialized (Code), Premier |
| **Input price** | $0.30 / MTok |
| **Cached input price** | 🆕 $0.03 / MTok *(90% off — newly published)* |
| **Output price** | $0.90 / MTok |
| **Context window** | 256,000 tokens |
| **Notable** | Purpose-built code model; fill-in-the-middle (FIM); low-latency completion, chat-based code generation |

---

### Leanstral 1.5 *(Labs — ⚠️ scheduled retirement Sept 30, 2026)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `leanstral-1-5` |
| **Released** | June 30, 2026 |
| **Scheduled retirement** | September 30, 2026 (per docs.mistral.ai changelog) — now just over a week out from this refresh |
| **Status** | ✅ Active — Labs — retirement date published |
| **Pricing** | **Free** *(API endpoint kept highly accessible for a limited period to gather feedback)* |
| **Context window** | 256,000 tokens |
| **Parameters** | 119B total, 6B active (MoE — same family as Mistral Small 4) |
| **License** | Apache 2.0 |
| **Notable** | First-of-kind open-source code agent purpose-built for Lean 4 formal proof engineering; ⚠️ scheduled for retirement September 30, 2026 — no successor announced yet |

---

### Voxtral Small 24B *(Audio / Speech)*

| Field | Value |
|---|---|
| **Model ID** | `voxtral-small-latest` |
| **Status** | ✅ Active — Specialized (Audio), Open |
| **Input price (audio)** | $0.004 / min |
| **Input price (text)** | $0.10 / MTok |
| **Output price** | $0.40 / MTok |
| **Context window** | 128,000 tokens |

---

### Voxtral Mini Transcribe 2 *(Premier — v26.02)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-mini-latest` |
| **Status** | ✅ Active — Specialized (Transcription) — Premier |
| **Pricing** | $0.003 / min |
| **Cached pricing** | 🆕 $0.0003 / min *(90% off — newly published)* |
| **Availability** | API (`/v1/audio/transcriptions`) |

---

### Voxtral Mini Transcribe Realtime *(Open — v26.02)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-mini-transcribe-realtime-2602` |
| **Status** | ✅ Active — Specialized (Real-time Transcription) — Open (Apache 2.0) |
| **Pricing** | $0.006 / min audio input |
| **Availability** | API (`/v1/audio/transcriptions`) |

---

### Voxtral TTS *(Text-to-Speech)*

| Field | Value |
|---|---|
| **Model ID** | `voxtral-mini-tts-latest` |
| **Status** | ✅ Active — Specialized (Text-to-Speech), Open |
| **Pricing** | $0.016 per 1,000 characters ($16/M characters) |
| **Notable** | State-of-the-art TTS with zero-shot voice cloning and multilingual support; 4B params; CC BY-NC 4.0 (non-commercial) |

---

### OCR 4.1 *(Flagship OCR, supersedes OCR 4.0)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-ocr-latest` *(alias — points to OCR 4.1)* / docs card `ocr-4-1` |
| **Status** | ✅ Active — **Flagship OCR** — Premier |
| **OCR price (standard)** | $4.00 / 1,000 pages |
| **Cached price** | 🆕 $0.40 / 1,000 pages *(90% off — newly published)* |
| **OCR price (Batch-API)** | $2.00 / 1,000 pages *(50% off)* |
| **Document AI price** | $5.00 / 1,000 pages |
| **Availability** | API (Mistral Studio), Amazon SageMaker, Microsoft Foundry, self-hosted (enterprise) |
| **Notable** | "The world's best document extraction and understanding model" per Mistral; OCR 4.0 remains available for existing integrations |

---

### ⚠️ LEGACY — OCR 4.0 *(Superseded by OCR 4.1)*

| Field | Value |
|---|---|
| **Model ID** | `ocr-4-0` |
| **Status** | ⚠️ LEGACY — Superseded by OCR 4.1; available for existing integrations |
| **Last price** | $4.00/1K pages (standard) · $0.40/1K cached · $2.00/1K (Batch) · $5.00/1K (Document AI) — identical to 4.1 |
| **Migration** | → **OCR 4.1** (`mistral-ocr-latest`) for confidence-score support; same price |

---

### Codestral Embed *(Premier — Code Embeddings)*

| Field | Value |
|---|---|
| **Model ID** | `codestral-embed` |
| **Status** | ✅ Active — Specialized (Code Embeddings) |
| **Input price** | $0.15 / MTok |
| **Cached input price** | 🆕 $0.015 / MTok *(90% off — newly published)* |

---

### Mistral Embed *(General Embeddings)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-embed` |
| **Status** | ✅ Active — Specialized (General Embeddings) |
| **Input price** | $0.10 / MTok |

---

### Mistral Moderation 2 *(Content Classifier)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-moderation-2603` |
| **Status** | ✅ Active — Specialized (Content Moderation), Premier |
| **Pricing** | 📉 **Free** *(corrected this refresh — previously tracked at $0.10/MTok; the live `docs.mistral.ai/inference/pricing` page lists Input/Cached input/Output all as "Free")* |
| **Notable** | 128K context window; jailbreaking detection; distinct product from the open-weight Shieldstral classifier (see Discovery-Only section) |

---

### Classifier API model 3B *(Fine-tunable Classifier)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Status** | ✅ Active — Specialized (Classification) |
| **Training cost** | $1.00 / MTok *(one-off fine-tuning)* |
| **Storage cost** | $2.00 / month per model |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.10 / MTok |
| **Notable** | Fine-tunes Ministral 3B |

---

### Classifier API model 8B *(Fine-tunable Classifier — Larger)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Status** | ✅ Active — Specialized (Classification) |
| **Training cost** | $1.00 / MTok *(one-off fine-tuning)* |
| **Storage cost** | $2.00 / month per model |
| **Input price** | $0.04 / MTok |
| **Output price** | $0.04 / MTok |
| **Notable** | Fine-tunes Ministral 8B; lower inference cost than 3B variant |

---

### Ministral 3 - 14B

| Field | Value |
|---|---|
| **Model ID** | `ministral-14b-latest` |
| **Status** | ✅ Active — Open |
| **Input price** | $0.20 / MTok |
| **Cached input price** | 🆕 $0.02 / MTok *(90% off — newly published)* |
| **Output price** | $0.20 / MTok |
| **Context window** | 256,000 tokens |

---

### Ministral 3 - 8B

| Field | Value |
|---|---|
| **Model ID** | `ministral-8b-latest` |
| **Status** | ✅ Active — Open |
| **Input price** | $0.15 / MTok |
| **Cached input price** | 🆕 $0.015 / MTok *(90% off — newly published)* |
| **Output price** | $0.15 / MTok |
| **Context window** | 256,000 tokens |

---

### Ministral 3 - 3B

| Field | Value |
|---|---|
| **Model ID** | `ministral-3b-latest` |
| **Status** | ✅ Active — Open |
| **Input price** | $0.10 / MTok |
| **Cached input price** | 🆕 $0.01 / MTok *(90% off — newly published)* |
| **Output price** | $0.10 / MTok |
| **Context window** | 256,000 tokens (up to 556K on some deployments) |

---

### Mixtral 8x22B *(API — Legacy Open-Weight)*

| Field | Value |
|---|---|
| **Model ID** | `open-mixtral-8x22b` |
| **Status** | ✅ Active (API) — Legacy open-weight |
| **Input price** | $2.00 / MTok |
| **Output price** | $6.00 / MTok |
| **Context window** | 65,536 tokens |

---

### Mixtral 8x7B *(API — Legacy Open-Weight)*

| Field | Value |
|---|---|
| **Model ID** | `open-mixtral-8x7b` |
| **Status** | ✅ Active (API) — Legacy open-weight |
| **Input price** | $0.70 / MTok |
| **Output price** | $0.70 / MTok |
| **Context window** | 32,768 tokens |

---

## 🌐 Regional Endpoints & Priority Tier *(GA / Public Preview — confirmed unchanged Sept 21, 2026)*

| Feature | Status | Details |
|---|---|---|
| **Mistral Regional Endpoints** | ✅ **General Availability** | Choose EU or US inference region for supported models (including third-party models like GLM-5.2/5.3). **+10% surcharge.** |
| **Mistral Priority Tier** | 🆕 **Public Preview** | Committed service levels for mission-critical workloads: custom rate limits, uptime SLA. |
| **Cached input tokens** | 🆕 **Now broadly available** | -90% on input tokens for repeated prompts — now published for native Mistral models (Large 3, Medium 3.5, Small 4, Ministral tiers, Codestral, Codestral Embed, OCR 4.1/4.0, Voxtral Mini Transcribe 2) in addition to GLM-5.2/5.3 |

---

## 🏦 Company Milestone: €3B Series D *(September 8, 2026 — non-pricing)*

> Mistral announced it raised **€3 billion in a Series D funding round** at a post-money valuation of more than **€21 billion**. Led by Samsung Electronics together with the Scaleup Europe Fund (managed by EQT) and existing investor PSG Equity, per third-party reporting. This is a **corporate funding milestone with no direct impact on API or subscription pricing**.

## 🤝 Mistral x Mozilla *(September 16, 2026 — non-pricing)*

> Mozilla and Mistral AI announced a partnership to bring open, private, and multilingual AI to Firefox's "Smart Window" feature. This is a **browser product integration, not a new priced API model or pricing change**.

---

## 🤖 Discovery-Only: Non-LLM / Unpriced Model Releases *(not priced, not tracked as full cards)*

> Per this tracker's verification-before-tracking policy, releases without published API/token pricing are noted here for awareness only and are not given a full model card.

### Shieldstral 1.0 *(Open-Weight Multimodal Safety Classifier — Released August 4, 2026)*

> A 3B-class (3.8B total/active parameters) open-weights, policy-adaptive multimodal safety classifier for text and images. Built on a Ministral-3-3B backbone with a Pixtral vision encoder. Released under Apache 2.0 (`mistralai/Shieldstral-1.0`). **No hosted API model ID or per-token rate published** — self-host only (single 16GB GPU). Source: https://mistral.ai/news/shieldstral/

### Robostral Navigate *(Embodied Navigation — Released July 8, 2026)*

> An 8B parameter model for embodied robot navigation using a single RGB camera. **Has no listing or pricing on `mistral.ai/pricing/api`** — a robotics research release, not a text/chat model. Source: https://mistral.ai/news/robostral-navigate/

---

## 🔧 Platform Tool Pricing (Mistral AI Studio — Agent API)

| Tool | Pricing |
|---|---|
| **Agent API** | Model cost per MTok + tool call |
| **Libraries (OCR)** | $3 / 1K pages |
| **Libraries (Indexing)** | $1 / MTok |
| **Libraries (Call)** | $0.01 / call |
| **Code execution** | $30 / 1K calls |
| **Web search** | $30 / 1K calls |
| **Image generation** | $100 / 1K images |
| **Premium news** | $50 / 1K calls |
| **Data capture** | $0.04 / MTok |

---

## 🔓 Open-Weight / Self-Hosted Models

| Model | Parameters | License | Best For |
|---|---|---|---|
| **Mistral Medium 3.5** | 128B (dense) | Modified MIT | Self-hosted flagship: coding + reasoning + vision |
| **Mistral Small 4** | 119B (MoE, 6B active) | Apache 2.0 | Self-hosted multimodal reasoning + coding |
| **Mistral Large 3 (2512)** | 675B (MoE) | Apache 2.0 | Self-hosted flagship general reasoning |
| **Leanstral 1.5** | 119B (MoE, 6B active) | Apache 2.0 | Self-hosted Lean 4 formal proof engineering *(retiring Sept 30, 2026)* |
| **Shieldstral 1.0** | 3.8B | Apache 2.0 | Self-hosted policy-adaptive text/image safety classification *(no hosted API yet)* |
| **Voxtral Small 24B** | 24B | Apache 2.0 | Self-hosted audio understanding |
| **Voxtral Mini Transcribe Realtime** | — | Apache 2.0 | Self-hosted real-time transcription |
| **Voxtral TTS** | 4B | CC BY-NC 4.0 | Self-hosted TTS (non-commercial only) |
| **OCR 4.1** | — | Premier (API) | Self-hosted document OCR (enterprise, single container) |
| **Z.ai GLM-5.2 / GLM-5.3** | — | Open | Hosted on Mistral's platform (not self-hosted, but open-weight) — long-context agentic/coding |
| **Mixtral 8×22B** | 141B (MoE) | Apache 2.0 | Self-hosted complex reasoning |
| **Mixtral 8×7B** | 46.7B (MoE) | Apache 2.0 | General-purpose self-hosted |
| **Mistral 7B** | 7B | Apache 2.0 | Edge / on-device |

> ⚠️ **Devstral 2, Devstral Small 2, and all Magistral (Medium/Small) versions are RETIRED from the hosted API (July 31, 2026)** — their open weights remain downloadable on HuggingFace for self-hosting, but Mistral itself recommends Mistral Medium 3.5 / Small 4 for hosted use going forward.

---

## ⚠️ Legacy / Deprecated / Retired Models

### ⚠️ RETIRED — Devstral 2 *(123B — API retired July 31, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `devstral-medium-latest` / `devstral-2512` |
| **Status** | ⚠️ **RETIRED from the hosted API July 31, 2026** — superseded by Mistral Medium 3.5 |
| **Last price** | $0.40 / MTok input · $2.00 / MTok output |
| **Migration** | → **Mistral Medium 3.5** (`mistral-medium-latest`, $1.50/$7.50) — a ~275% increase on both input and output tokens per third-party migration trackers, offset by unified reasoning+coding+vision capability |
| **Note** | Open weights remain downloadable (Modified MIT) for self-hosting |

---

### ⚠️ RETIRED — Devstral Small 2 *(24B — API retired July 31, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `devstral-small-latest` / `labs-devstral-small-2512` |
| **Status** | ⚠️ **RETIRED from the hosted API July 31, 2026** — superseded by Mistral Small 4 |
| **Last price** | $0.10 / MTok input · $0.30 / MTok output |
| **Migration** | → **Mistral Small 4** (`mistral-small-latest`, $0.15/$0.60) |
| **Note** | Open weights remain downloadable (Apache 2.0) for self-hosting; runs on a single RTX 4090/32GB Mac at Q4 |

---

### ⚠️ RETIRED — Magistral Medium (all versions: 1.0 / 1.1 / 1.2) *(API retired July 31, 2026)*

| Field | Value |
|---|---|
| **Model IDs** | `magistral-medium-2506` (1.0) · `magistral-medium-2507` (1.1) · `magistral-medium-2509` (1.2) — `magistral-medium-latest` alias no longer resolves to a supported dedicated model |
| **Status** | ⚠️ **RETIRED from the hosted API July 31, 2026** — reasoning capability now lives in Mistral Medium 3.5 |
| **Last price** | $2.00 / MTok input · $5.00 / MTok output |
| **Migration** | → **Mistral Medium 3.5** with `reasoning_effort=high` |

---

### ⚠️ RETIRED — Magistral Small (all versions: 1.0 / 1.1 / 1.2) *(API retired July 31, 2026)*

| Field | Value |
|---|---|
| **Model IDs** | `magistral-small-2506` (1.0) · `magistral-small-2507` (1.1) · `magistral-small-2509` (1.2) — `magistral-small-latest` alias now resolves to Mistral Small 4 |
| **Status** | ⚠️ **RETIRED from the hosted API July 31, 2026** — reasoning capability now lives in Mistral Small 4 |
| **Last price** | $0.50 / MTok input · $1.50 / MTok output |
| **Migration** | → **Mistral Small 4** (`mistral-small-latest`) with `reasoning_effort=high` — a ~70%/60% price *decrease* vs. the old Magistral Small rate |

---

### ⚠️ RETIRED — Mistral Small 3.2 24B *(API retired July 31, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-small-2506` |
| **Status** | ⚠️ RETIRED July 31, 2026 |
| **Migration** | → **Mistral Small 4** (`mistral-small-latest`) |

---

### ⚠️ RETIRED — Mistral NeMo 12B *(API retired July 31, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `open-mistral-nemo` |
| **Status** | ⚠️ **RETIRED July 31, 2026** *(corrected this refresh — prior tracking listed this as still active on the API)* |
| **Last price** | $0.15 / MTok input · $0.15 / MTok output |
| **Migration** | → **Ministral 3 8B/14B** or **Mistral Small 4** |
| **Note** | The `mistral-tiny-latest` alias is reported by some third parties to still resolve to `open-mistral-nemo` in certain SDK versions — verify directly against your account before relying on this |

---

### ⚠️ RETIRED — Mistral Medium 3.1 *(API retired August 31, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-medium-2508` |
| **Status** | ⚠️ **RETIRED August 31, 2026** *(corrected this refresh — prior tracking listed this only as "Legacy")* |
| **Migration** | → **Mistral Medium 3.5** ($1.50/$7.50) |

---

### ⚠️ RETIRED — Mistral Medium 3 *(API retired August 31, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-medium-2505` |
| **Status** | ⚠️ **RETIRED August 31, 2026** *(corrected this refresh — prior tracking listed this only as "Legacy")* |
| **Last price** | $1.00 / MTok input (per third-party trackers) |
| **Migration** | → **Mistral Medium 3.5** — note this is also a price increase from Medium 3's ~$1/MTok input rate |

---

### ⚠️ LEGACY — OCR 3 v25.12 *(Superseded by OCR 4 line)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-ocr-2512` |
| **Status** | ⚠️ LEGACY — Superseded by the OCR 4 line (OCR 4.0, then 4.1); available for existing integrations |
| **Last price** | $2.00 / 1,000 pages · $3.00 / 1,000 pages (annotations) |
| **Migration** | → **OCR 4.1** (`mistral-ocr-latest`) |

---

### ⚠️ LEGACY — Voxtral Mini 3B v25.07

| Field | Value |
|---|---|
| **Model ID** | `voxtral-mini-2507` |
| **Status** | ⚠️ LEGACY — In legacy table at docs.mistral.ai |
| **Migration** | → **Voxtral Mini Transcribe 2** ($0.003/min) or **Voxtral Mini Transcribe Realtime** ($0.006/min) |

---

### ⚠️ LEGACY — Leanstral v26.03 *(🔄 Replaced by Leanstral 1.5)*

| Field | Value |
|---|---|
| **Model ID** | `labs-leanstral-2603` |
| **Status** | ⚠️ LEGACY — 🔄 Replaced by Leanstral 1.5; still free while accessible |
| **Migration** | → **Leanstral 1.5** (`leanstral-1-5`) — note: also scheduled for retirement Sept 30, 2026 |

---

### ⚠️ LEGACY — Pixtral Large

| Field | Value |
|---|---|
| **Model ID** | `pixtral-large-2411` |
| **Status** | ⚠️ LEGACY |
| **Migration** | → **Mistral Medium 3.5** or **Mistral Small 4** |

---

### ⚠️ LEGACY — Older Generations

| Model | Status | Migration |
|---|---|---|
| Devstral Small 1.1 / 1.0 | ⚠️ RETIRED | → Mistral Small 4 |
| Devstral Medium 1.0 | ⚠️ RETIRED | → Mistral Medium 3.5 |
| Mistral Small 3.1 / 3.0 | ⚠️ LEGACY | → Mistral Small 4 |
| Mistral Large 2.1 / 2.0 | ⚠️ LEGACY | → Mistral Large 3 |
| Codestral 2501 / 24.05 | ⚠️ LEGACY | → Codestral 2508 |
| Mistral Saba | ⚠️ LEGACY | → Mistral Medium 3.5 (multilingual) |
| Pixtral 12B | ⚠️ LEGACY | → Mistral Small 4 |
| Ministral 3B / 8B (24.10) | ⚠️ LEGACY | → Ministral 3 (3B/8B/14B) |
| Codestral Mamba 7B | ⚠️ LEGACY | → Codestral 2508 |
| Mathstral 7B | ⚠️ LEGACY | → Mistral Small 4 (reasoning_effort=high) |
| Mistral 7B (0.1/0.2/0.3) | ⚠️ LEGACY | → Ministral 3 3B |
| Mistral Large / Small / Medium 1.0 | ⚠️ LEGACY | → Current generation equivalents |
| Mixtral 8x7B / 8x22B (original) | ⚠️ LEGACY (API still active) | → Mistral Small 4 / Large 3 |
| Mistral Moderation (24.11) | ⚠️ LEGACY | → Mistral Moderation 2 (`mistral-moderation-2603`), now Free |

---

## 💡 Cost Optimization Notes

| Feature | Notes |
|---|---|
| **Batch API discount** | 50% off — confirmed per mistral.ai/pricing |
| 🆕 **Prompt caching now on native Mistral models** | Large 3, Medium 3.5, Small 4, Ministral tiers, Codestral, Codestral Embed, OCR 4.1/4.0, and Voxtral Mini Transcribe 2 all now publish a 90%-off cached-input rate — no longer a GLM-5.x-only feature |
| **EU / US data residency** | Regional Endpoints GA — choose EU or US inference region (+10% surcharge) |
| **Priority Tier (public preview)** | SLA-backed committed service levels with custom rate limits for mission-critical workloads |
| **Free tier** | Available via La Plateforme; rate-limited; no credit card required |
| **GLM-5.2 / GLM-5.3 for long-context agentic work** | $1.40/$4.40 per MTok, 1M context — cheaper alternative to Mistral Medium 3.5 ($1.50/$7.50) for long-context, coding-heavy workloads |
| **Classifier API fine-tuning** | Build custom classifiers from Ministral 3B ($0.10/$0.10) or 8B ($0.04/$0.04) inference |
| **Budget reasoning** | Use Mistral Small 4 with `reasoning_effort=high` ($0.15/$0.60) — now the *only* supported reasoning-dial option since Magistral Small's retirement |
| **⚠️ Devstral and Magistral are retired from the hosted API** | Both families (all versions) retired July 31, 2026. Route Devstral/Magistral-tier traffic to Mistral Medium 3.5 or Small 4 with `reasoning_effort` set appropriately |
| **⚠️ Mistral Medium 3 / 3.1 retired August 31, 2026** | Migrate to Medium 3.5 — note this is a price increase for anyone still pinned to Medium 3's old ~$1/MTok input rate |
| **Voxtral transcription** | Voxtral Mini Transcribe 2 (`voxtral-mini-latest`, $0.003/min, now $0.0003/min cached) for batch; Realtime ($0.006/min) for live |
| **OCR 4.1 batch savings** | Batch-API: $2/1K pages (50% off standard $4/1K pages); cached input now $0.40/1K pages |
| **⚠️ Leanstral 1.5 retiring Sept 30, 2026** | Free Labs endpoint (`leanstral-1-5`) — now just over a week out from this refresh; no successor announced yet |
| **Mistral Moderation 2 is Free** | Corrected this refresh from a previously-tracked $0.10/MTok rate |
| **Agent API tool costs add up** | Web search and code execution are both $30/1K calls on the Agent API |
| **Robostral Navigate / Shieldstral are unpriced** | No published API pricing — self-host only |
| **🆕 €3B Series D funding round** | September 8, 2026 — company milestone, no pricing impact |
| **🆕 Mistral x Mozilla (Firefox)** | September 16, 2026 — browser integration partnership, no pricing impact |

---

## 💬 Vibe / Consumer Plans *(separate from API billing)*

| Plan | Price | Notes |
|---|---|---|
| **Free** | $0/mo | Rate-limited, mid-tier models, limited coding sessions |
| **Pro** | $14.99/mo | More messages, all-day coding, extended thinking, deep research, 15GB storage |
| **Team** | $24.99/user/mo | Up to 30GB storage/user, domain verification, data export |
| **Education** | $5.99/mo | Verified students only (max 12 months) |
| **Enterprise** | Custom | SSO, audit logs, white label, custom models |

> ⚠️ Vibe Pro does **not** include API access. Consumer and developer API billing are entirely separate.

---

*Sources last verified: September 23, 2026 against `mistral.ai/pricing/api`, `docs.mistral.ai/inference/pricing`, and `mistral.ai/news`. **This cycle:** independently re-verified every active model price on the live pricing page — all confirmed byte-for-byte unchanged since the September 22 refresh (Mistral Large 3, Medium 3.5, Small 4, Ministral 3 tiers, Codestral, Codestral Embed, OCR 4.1/4.0, Voxtral TTS/Transcribe 2, Moderation 2 Free, Z.ai GLM-5.2/5.3, Leanstral 1.5 Free). No new Mistral news posts since the Sept 16 Mozilla/Firefox partnership. No new model releases, retirements, or price changes found this cycle. **Prior cycle's major corrections (Sept 21, still in effect):** (1) Devstral 2, Devstral Small 2, and the entire Magistral family were confirmed RETIRED July 31, 2026 (previously mistracked as Active) — moved to Legacy with migration guidance to Mistral Medium 3.5 / Small 4; (2) Mistral Medium 3 and 3.1 confirmed RETIRED August 31, 2026 (previously only "Legacy"); (3) Mistral Small 3.2 and Mistral NeMo 12B confirmed RETIRED July 31, 2026.*
