# 🔵 Mistral AI — Model Cards

> **Last updated:** 2026-08-03
> **Source:** https://mistral.ai/pricing · https://mistral.ai/pricing/api · https://docs.mistral.ai/models/overview · https://docs.mistral.ai/resources/changelogs
> **Scraped / verified:** 2026-08-03 — ✅ **Re-verified against the live `mistral.ai/pricing/api` page.** Every active price point (Mistral Medium 3.5 $1.50/$7.50, Mistral Large 3 $0.50/$1.50, Mistral Small 4 $0.15/$0.60, Magistral Medium/Small, Codestral $0.30/$0.90, Devstral 2 $0.40/$2.00, Devstral Small 2 $0.10/$0.30, Leanstral 1.5 free, Voxtral family, OCR 4 $4/$2/$5 per 1K pages, Classifier APIs, embeddings, Ministral 3 family, Mixtral, Agent API tool pricing) matches exactly — **no new priced model releases or price changes detected since the July 27, 2026 refresh.** 🔭 **Discovery-only note:** Mistral published "Introducing Robostral Navigate" (July 8, 2026) — an 8B embodied-navigation robotics model (single-camera visual navigation for robots). It is **not listed on `mistral.ai/pricing/api`** and has no published per-token/API pricing, so per this tracker's verification-before-tracking policy it is **not added as a full model card** — flagged here for awareness only.

All prices are **USD per million tokens (MTok)**. Mistral offers a **free experimentation tier** (rate-limited) — no credit card required to start. API and consumer (Vibe) subscriptions are billed **separately**.

> **Mistral's key differentiators:** Native EU data residency (GDPR by default), competitive mid-tier pricing, Apache 2.0 / Modified MIT open-weight models, dedicated reasoning (Magistral series), flagship merged model (Medium 3.5), and a 50% batch processing discount.

> 📝 **August 3, 2026 update:**
> - ✅ Independently re-verified every active price point against `mistral.ai/pricing/api` — **all confirmed unchanged**: Medium 3.5 $1.50/$7.50, Large 3 $0.50/$1.50, Small 4 $0.15/$0.60, Magistral Medium $2/$5, Magistral Small $0.50/$1.50, Codestral $0.30/$0.90, Devstral 2 $0.40/$2.00, Devstral Small 2 $0.10/$0.30, OCR 4 $4/1K pages (std) · $2/1K (Batch) · $5/1K (Document AI), Voxtral family, Ministral 3 tiers, Classifier APIs, embeddings, Agent API tool pricing (Web search/Code execution $30/1K calls, Image generation $100/1K images, etc.), and Mixtral/NeMo legacy-API models.
> - 🔭 **New discovery (not priced, not added as a tracked model):** Mistral published **"Introducing Robostral Navigate"** (July 8, 2026) — an 8B parameter embodied-navigation model that lets robots navigate complex environments using a single RGB camera (no LiDAR/depth sensors), achieving 76.6% on R2R-CE validation-unseen. This is a robotics/embodied-AI research release, not a text/chat LLM, and **no API pricing or token rates are published** for it — it does not appear on `mistral.ai/pricing/api`. Per this tracker's policy of verifying pricing before adding a model card, Robostral Navigate is noted here for awareness only and will be evaluated for a full card if/when Mistral publishes API access and pricing.
> - ℹ️ Checked `mistral.ai/news` for releases since the July 27 refresh — the most recent items are "Your Prompts and Skills need a system of record" (Studio feature, July 9, 2026) and Robostral Navigate (above); **no new priced LLM/API model releases found.**
> - ℹ️ Mistral's "Featured Models" and "Frontier Models" sections on `docs.mistral.ai/models/overview` continue to list Mistral Medium 3.5, Mistral Small 4, Mistral Large 3, Ministral 3 (14B/8B/3B), OCR 4, Devstral 2, and Voxtral TTS as the current flagship lineup — unchanged from the prior refresh.

> 📝 **July 27, 2026 update:**
> - ✅ Independently re-verified every active price point against `mistral.ai/pricing/api` and cross-checked against three independent pricing trackers (benchlm.ai, cloudzero.com, spheron.network, all synced July 20–26, 2026) — **all confirmed unchanged**: Medium 3.5 $1.50/$7.50, Large 3 $0.50/$1.50, Small 4 $0.15/$0.60, Codestral $0.30/$0.90, Devstral 2 $0.40/$2.00, Devstral Small 2 $0.10/$0.30, Ministral 3 tiers $0.10–$0.20, OCR 4 $4/1K pages (std) · $2/1K (Batch) · $5/1K (Document AI).
> - 🆕 **Leanstral 1.5 retirement date now published:** `docs.mistral.ai/resources/changelogs` confirms Leanstral 1.5 will be retired **September 30, 2026**. Still free and fully available until that date.
> - 🔭 Flagged (not yet added as a tracked model): CEO Arthur Mensch confirmed a new, larger open-weight MoE model family entering **July 2026 early access**, with a broader public release expected later this summer. No pricing, benchmarks, or license published yet — will only be added to this tracker once Mistral publishes official specs/pricing, per our verification-before-tracking policy.
> - ℹ️ Mistral's "Featured Models" and "Frontier Models" sections on `docs.mistral.ai/models/overview` continue to list Mistral Medium 3.5, Mistral Small 4, Mistral Large 3, Ministral 3 (14B/8B/3B), OCR 4, Devstral 2, and Voxtral TTS as the current flagship lineup — unchanged from the prior refresh.

> 📝 **July 20, 2026 update:**
> - ✅ Independently re-fetched `mistral.ai/pricing/api` in full — every active model card (Medium 3.5 $1.50/$7.50, Large 3 $0.50/$1.50, Small 4 $0.15/$0.60, Magistral Medium $2/$5, Magistral Small $0.50/$1.50, Codestral $0.30/$0.90, Devstral 2 $0.40/$2.00, Devstral Small 2 $0.10/$0.30, OCR 4 $4/$5 per 1K pages, Voxtral family, Ministral 3 tiers, embeddings, moderation, classifiers, Mixtral/NeMo legacy-API models) matches exactly, including model IDs and license tags (Open/Premier/Labs).
> - ⚠️ **Flagged and resolved a stale marketing-copy discrepancy:** the `mistral.ai/pricing` (non-API) FAQ page still answers "How is API pricing calculated?" with a "$2/M in, $6/M out" Mistral Large example — this is outdated illustrative copy from an earlier Large generation and contradicts the live product table on `mistral.ai/pricing/api`, which is the authoritative source and confirms Large 3 at $0.50/$1.50. No action needed on this repo's figures; flagging here so future refreshes don't mistake the stale FAQ text for a price change.
> - 🆕 **Newly captured this cycle — Agent API tool pricing** (previously listed only in the Platform Tool Pricing table below, now cross-verified against the live `mistral.ai/pricing/api` "Agent API" section): Libraries OCR $3/1K pages, Libraries Indexing $1/MTok, Libraries Call $0.01/call, Code execution $30/1K calls, Web search $30/1K calls, Image generation $100/1K images, Premium news $50/1K calls, Data capture $0.04/MTok. All confirmed unchanged.
> - ✅ Legacy/deprecated table re-cross-checked against `docs.mistral.ai/models/overview` — the full legacy list (OCR 3, Voxtral Mini 3B, Leanstral v26.03, Mistral Medium 3.1/3, Devstral 2 v25.12, Devstral Small 2 v25.12, Magistral Medium 1.1/1.2, Magistral Small 1.1/1.2, Mistral Small Creative, Mistral Small 3.2/3.1/3.0, Pixtral Large/12B, Mistral Saba, Ministral 3B/8B (24.10), Mistral Large 2.1/2.0/1.0, Mistral Nemo 12B, Codestral Mamba, Mathstral, Mistral 7B, Mixtral 8x7B/8x22B, Mistral Small/Medium 1.0, Mistral Next) remains confirmed with no additions or removals since the last refresh.
> - ℹ️ Mistral's "Featured Models" and "Frontier Models" sections on `docs.mistral.ai/models/overview` continue to list Mistral Medium 3.5, Mistral Small 4, Mistral Large 3, Ministral 3 (14B/8B/3B), OCR 4, Devstral 2, and Voxtral TTS as the current flagship lineup — unchanged from the prior refresh.

> 📝 **July 14, 2026 update:**
> - 🛠️ **Model ID correction — Leanstral 1.5:** The confirmed API endpoint is `leanstral-1-5` (docs.mistral.ai model card + Mistral's official July 2, 2026 announcement both list it without the `labs-` prefix), even though the model is still tagged **Labs** in the docs.mistral.ai catalog license/category system. Previously documented here as `labs-leanstral-1-5` — corrected.
> - 📄 **Leanstral 1.5 benchmark detail confirmed from Mistral's official announcement:** 119B total / 6B active parameters (Apache 2.0), saturates miniF2F (100% on validation and test sets), solves 587/672 PutnamBench problems, and reaches state-of-the-art on FATE-H (87%) and FATE-X (34%) among comparable formal-reasoning models. On the newly open-sourced FLTEval benchmark, it lifts pass@1 from 21.9 to 28.9 and pass@8 from 31.9 to 43.2 — surpassing Claude Opus 4.6's 39.6 pass@8 at roughly one-seventh the cost. Pricing remains **free** while Mistral gathers feedback.
> - ✅ Independently re-verified all other active pricing against the live `mistral.ai/pricing/api` page — every other model card matches exactly. No new model releases or price changes since the June 30, 2026 update.
> - ✅ Legacy/deprecated table cross-checked against `docs.mistral.ai/models/overview` — confirmed additions since the last refresh: **Magistral Medium 1.1** (`magistral-medium-2507`, v25.07) now also appears in the legacy table (previously only 1.2/v25.09 was listed here). All previously documented legacy entries (OCR 3, Voxtral Mini 3B, Leanstral v26.03, Mistral Medium 3.1, Devstral 2 v25.12, Devstral Small 2 v25.12, Magistral Medium 1.2 v25.09, Magistral Small 1.2 v25.09, Mistral Small Creative, Pixtral Large, Mistral Saba, Mistral Medium 3, Mistral Small 3.1/3.0, and earlier generations) remain confirmed.
> - ℹ️ Mistral's "Featured Models" and "Frontier Models" sections on `docs.mistral.ai/models/overview` continue to list Mistral Medium 3.5, Mistral Small 4, Mistral Large 3, Ministral 3 (14B/8B/3B), OCR 4, Devstral 2, and Voxtral TTS as the current flagship lineup — unchanged from the prior refresh.

> 📝 **June 30, 2026 update:**
> - 🆕 **Leanstral 1.5** (`leanstral-1-5`, Labs) launched June 30, 2026 (announced via blog post July 2, 2026) — an updated Lean 4 formal proof engineering / automated theorem proving agent (119B total params, 6B active), superseding the original Leanstral (v26.03, March 2026). Still free while Mistral gathers feedback. Original v26.03 remains listed but is now formally replaced.

> 📝 **June 29, 2026 update:**
> - 🆕 **OCR 4** (v4.0, Premier) launched June 23, 2026 — $4/1K pages (standard), $2/1K pages (Batch-API), $5/1K pages (Document AI). `mistral-ocr-latest` alias now points to OCR 4. OCR 3 moved to legacy (still available for existing integrations per docs.mistral.ai).
> - 📈 **Mistral Small 4 price increase** — confirmed on live mistral.ai/pricing: Input $0.10→**$0.15/MTok**, Output $0.30→**$0.60/MTok** (+50% input, +100% output).
> - ⚠️ **Voxtral Mini 3B** (`voxtral-mini-2507`) now in legacy table at docs.mistral.ai. `voxtral-mini-latest` alias reassigned to Voxtral Mini Transcribe 2.
> - ⚠️ New legacy additions in docs.mistral.ai: Devstral 2 v25.12 (`devstral-2512`), Devstral Small 2 v25.12 (`labs-devstral-small-2512`), Magistral Medium 1.2 v25.09 (`magistral-medium-2509`). The `devstral-medium-latest`, `devstral-small-latest`, and `magistral-medium-latest` aliases remain active.
> - ✅ All other active prices re-confirmed unchanged.

> 📝 **June 22, 2026 update:** All active prices re-verified unchanged. No new model releases detected. Previously confirmed legacy/deprecated statuses unchanged.

> 📝 **June 15, 2026 update:** Pricing corrections and legacy moves confirmed against official sources:
> - **PRICE CORRECTION:** Voxtral Mini Transcribe 2 (v26.02, Premier): $0.002/min → **$0.003/min** (corrected against mistral.ai/pricing)
> - **PRICE CONFIRMED:** Voxtral Mini Transcribe Realtime (v26.02, Open): **$0.006/min** audio input (was TBD, now confirmed)
> - **MOVED TO LEGACY:** Leanstral (`labs-leanstral-2603`, v26.03) now in legacy/deprecated table at docs.mistral.ai
> - **FORMALLY DEPRECATED:** Mistral Medium 3.1 (`mistral-medium-2508`, v25.08) confirmed in legacy table at docs.mistral.ai
> - All other active prices confirmed unchanged.

---

## ✅ Active / Recommended Models

### 🆕 Mistral Medium 3.5 *(Flagship — Released April 29, 2026)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-medium-latest` |
| **Released** | April 29, 2026 |
| **Status** | ✅ Active — **Flagship** |
| **Input price** | $1.50 / MTok |
| **Output price** | $7.50 / MTok |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio / La Plateforme); NVIDIA NIM; open weights on HuggingFace (modified MIT license) |
| **Capabilities** | Text, Vision, Function Calling, JSON mode, Configurable reasoning effort (`reasoning_effort`), Agentic coding, 24-language support |
| **Notable** | First Mistral flagship merged model; 128B dense; SWE-Bench Verified 77.6%; self-hostable on 4× A100/H100 80GB GPUs; default model for Mistral Vibe CLI and Le Chat Work Mode |

---

### Mistral Large 3 (2512)

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-large-latest` |
| **Status** | ✅ Active — General Reasoning Flagship, Open-weight |
| **Input price** | $0.50 / MTok |
| **Output price** | $1.50 / MTok |
| **Context window** | 262,144 tokens (256K) |
| **Notable** | Cheapest output pricing vs peers; GDPR-compliant EU hosting; open-weight, general-purpose multimodal model. ⚠️ Re-confirmed August 3, 2026 against the live `mistral.ai/pricing/api` product table — do not confuse with the stale "$2/$6" example on the general `mistral.ai/pricing` FAQ page (see header note above) |

---

### Magistral Medium *(Reasoning Model)*

> **Note:** Active via `magistral-medium-latest` at $2/$5. The specific version `magistral-medium-2509` is in legacy per docs.mistral.ai (alongside the earlier `magistral-medium-2507`, v1.1). `magistral-medium-latest` routes to the current active version.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `magistral-medium-latest` |
| **Status** | ✅ Active — Reasoning (Dedicated) |
| **Input price** | $2.00 / MTok |
| **Output price** | $5.00 / MTok |
| **Context window** | 128,000 tokens *(performance best <40K)* |
| **Notable** | Dedicated reasoning model with transparent chain-of-thought; multilingual; for most tasks, Medium 3.5 with `reasoning_effort=high` covers this use case |

---

### Magistral Small *(Active via `magistral-small-latest`)*

> **Note:** `magistral-small-latest` still active on `mistral.ai/pricing` at $0.50/$1.50. The specific version `magistral-small-2509` is in legacy per docs.mistral.ai. Prefer Mistral Small 4 with `reasoning_effort=high` ($0.15/$0.60) for most reasoning tasks.

| Field | Value |
|---|---|
| **Model ID** | `magistral-small-latest` |
| **Status** | ✅ Active via `latest` alias (specific version `magistral-small-2509` is legacy per docs.mistral.ai) |
| **Input price** | $0.50 / MTok |
| **Output price** | $1.50 / MTok |
| **Context window** | 128,000 tokens |

---

### Mistral Small 4 *(Released March 16, 2026)*

> **📈 Price increase confirmed on mistral.ai/pricing:** Input increased from $0.10 → **$0.15/MTok** (+50%). Output increased from $0.30 → **$0.60/MTok** (+100%). Note: Devstral Small 2 (`devstral-small-latest`) remains cheaper at $0.10/$0.30 for coding-focused use cases.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-small-latest` |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.60 / MTok |
| **Context window** | 262,144 tokens (256K) |
| **Capabilities** | Text, Vision, Function Calling, Reasoning (`reasoning_effort`), Agentic, Coding |
| **Notable** | Hybrid model unifying instruct, reasoning, and coding in a single efficient model; multimodal reasoning; configurable `reasoning_effort` (none → high) |

---

### Codestral 2508 *(Updated August 2025)*

| Field | Value |
|---|---|
| **Model ID** | `codestral-latest` |
| **Status** | ✅ Active — Specialized (Code), Premier |
| **Input price** | $0.30 / MTok |
| **Output price** | $0.90 / MTok |
| **Context window** | 256,000 tokens |
| **Notable** | Purpose-built code model; fill-in-the-middle (FIM); low-latency completion, chat-based code generation |

---

### Devstral 2 *(Coding Agent — Active via `devstral-medium-latest`)*

> **Note:** Active via `devstral-medium-latest` at $0.40/$2.00. The specific version `devstral-2512` is in the legacy table at docs.mistral.ai. `devstral-medium-latest` routes to the current active version.

| Field | Value |
|---|---|
| **Model ID** | `devstral-medium-latest` |
| **Status** | ✅ Active — Agentic Coding *(superseded in Vibe by Medium 3.5)* |
| **Input price** | $0.40 / MTok |
| **Output price** | $2.00 / MTok |
| **Context window** | 256,000 tokens |
| **Notable** | Frontier code agents model for solving software engineering tasks; open-weight (modified MIT license) |

---

### Devstral Small 2 *(Active via `devstral-small-latest`)*

> **Note:** Active via `devstral-small-latest` at $0.10/$0.30. Labeled **[Labs]** on mistral.ai/pricing. The specific version `labs-devstral-small-2512` is now in the legacy table at docs.mistral.ai. `devstral-small-latest` routes to the current active version.

| Field | Value |
|---|---|
| **Model ID** | `devstral-small-latest` |
| **Status** | ✅ Active — Labs tag on pricing page |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.30 / MTok |
| **Context window** | 256,000 tokens |
| **Notable** | Best lightweight, open model for coding agents; deployable on single RTX 4090/32GB Mac at Q4 |

---

### Leanstral 1.5 *(Labs — Released June 30, 2026 — ⚠️ scheduled retirement Sept 30, 2026)*

> **Leanstral 1.5 launched June 30, 2026** (official announcement published July 2, 2026). Updated version of Mistral's open-source Lean 4 formal proof engineering / automated theorem proving agent, superseding the original Leanstral (v26.03, released March 16, 2026 — see Legacy section). Still free while Mistral gathers real-world feedback and observability data. Model ID confirmed as `leanstral-1-5` (no `labs-` prefix on the endpoint itself, despite the Labs license/category tag), per `docs.mistral.ai/models/model-cards/leanstral-1-5` and Mistral's official blog post. The official Mistral docs changelog lists a scheduled retirement date of September 30, 2026 — plan migrations accordingly; no successor has been announced yet. Source: https://mistral.ai/news/leanstral-1-5 · https://docs.mistral.ai/resources/changelogs

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `leanstral-1-5` |
| **Released** | June 30, 2026 |
| **Scheduled retirement** | September 30, 2026 (per docs.mistral.ai changelog) |
| **Status** | ✅ Active — Labs — **Supersedes Leanstral v26.03**; retirement date published |
| **Pricing** | **Free** *(API endpoint kept highly accessible for a limited period to gather feedback)* |
| **Context window** | 256,000 tokens |
| **Parameters** | 119B total, 6B active (MoE — same family as Mistral Small 4) |
| **License** | Apache 2.0 (weights on Hugging Face: `mistralai/Leanstral-1.5-119B-A6B`) |
| **Capabilities** | Chat Completions, Function Calling, Agents & Conversations, Built-In Tools, Structured/Predicted Outputs, OCR, FIM, Embeddings, Moderations, Transcriptions, Text-to-Speech, Batching |
| **Availability** | API (`leanstral-1-5` endpoint); Mistral Vibe (`/leanstall`, `vibe --agent lean`) |
| **Benchmarks** | Saturates miniF2F (100% val/test); solves 587/672 PutnamBench problems; SOTA on FATE-H (87%) and FATE-X (34%); FLTEval pass@1 28.9 / pass@8 43.2 (up from 21.9 / 31.9), surpassing Claude Opus 4.6's 39.6 pass@8 at ~1/7th the cost; uncovered 5 previously unknown bugs across 57 tested open-source repositories |
| **Notable** | First-of-kind open-source code agent purpose-built for Lean 4 formal proof engineering and autoformalization; strongest test-time scaling seen from a formal-reasoning model (587 PutnamBench problems solved at a 4M-token budget, up from 44 at 50K); ⚠️ scheduled for retirement September 30, 2026 |

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
| **Model ID** | `voxtral-mini-latest` *(alias — previously pointed to standalone Voxtral Mini; now points to Voxtral Mini Transcribe 2)* |
| **Released** | February 2026 (version 26.02) |
| **Status** | ✅ Active — Specialized (Transcription) — Premier |
| **Pricing** | $0.003 / min |
| **Availability** | API (`/v1/audio/transcriptions`) |
| **Capabilities** | Batch speech-to-text transcription, speaker diarization, multilingual |
| **Notable** | Superseded original Voxtral Mini Transcribe (v25.07) and took over `voxtral-mini-latest` alias |

---

### Voxtral Mini Transcribe Realtime *(Open — v26.02)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-mini-transcribe-realtime-2602` |
| **Released** | February 2026 (version 26.02) |
| **Status** | ✅ Active — Specialized (Real-time Transcription) — Open (Apache 2.0) |
| **Pricing** | $0.006 / min audio input |
| **Availability** | API (`/v1/audio/transcriptions`) |
| **Capabilities** | Live/streaming speech-to-text transcription, low-latency, edge-compatible |
| **Notable** | Open-weight (Apache 2.0); purpose-built for real-time transcription use cases |

---

### Voxtral TTS *(Text-to-Speech — Released March 2026)*

| Field | Value |
|---|---|
| **Model ID** | `voxtral-mini-tts-latest` |
| **Status** | ✅ Active — Specialized (Text-to-Speech), Open |
| **Pricing** | $0.016 per 1,000 characters |
| **Notable** | State-of-the-art TTS with zero-shot voice cloning and multilingual support; 4B params; open weights on HuggingFace (CC BY-NC 4.0 — non-commercial) |

---

### OCR 4 *(Released June 23, 2026 — Flagship OCR)*

> **OCR 4 launched June 23, 2026.** Supersedes OCR 3 as the flagship OCR model. `mistral-ocr-latest` alias now points to OCR 4. OCR 3 remains accessible for existing integrations. Independent annotators reportedly prefer OCR 4 over every leading OCR/document-AI system tested, with win rates averaging 72%, and it tops OlmOCRBench. Source: https://mistral.ai/news/ocr-4/

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-ocr-latest` *(alias — now points to OCR 4)* |
| **Released** | June 23, 2026 |
| **Status** | ✅ Active — **Flagship OCR** — Premier |
| **OCR price (standard)** | $4.00 / 1,000 pages |
| **OCR price (Batch-API)** | $2.00 / 1,000 pages *(50% off)* |
| **Document AI price** | $5.00 / 1,000 pages |
| **Availability** | API (Mistral Studio), Amazon SageMaker, Microsoft Foundry, self-hosted (enterprise) |
| **Capabilities** | Text extraction, **bounding boxes** (paragraph-level), block classification (titles, tables, equations, signatures, headers/footers), inline confidence scores, markdown output, 170-language support across 10 language groups |
| **Notable** | World's best document extraction and understanding model per Mistral; compact enough for single-container self-hosted deployment; ingestion component for Mistral's open-source Search Toolkit |
| **Source** | https://mistral.ai/news/ocr-4/ · https://docs.mistral.ai/models/model-cards/ocr-4-0 |

---

### Codestral Embed *(Premier — Code Embeddings)*

| Field | Value |
|---|---|
| **Model ID** | `codestral-embed` |
| **Status** | ✅ Active — Specialized (Code Embeddings) |
| **Input price** | $0.15 / MTok |

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
| **Input price** | $0.10 / MTok |
| **Notable** | 128K context window; jailbreaking detection |

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
| **Capabilities** | Content moderation, sentiment analysis, fraud detection, custom classification |
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
| **Capabilities** | Content moderation, sentiment analysis, fraud detection, custom classification |
| **Notable** | Fine-tunes Ministral 8B; lower inference cost than 3B variant |

---

### Ministral 3 - 14B

| Field | Value |
|---|---|
| **Model ID** | `ministral-14b-latest` |
| **Status** | ✅ Active — Open |
| **Input price** | $0.20 / MTok |
| **Output price** | $0.20 / MTok |
| **Context window** | 256,000 tokens |
| **Notable** | Best-in-class frontier AI to the edge |

---

### Ministral 3 - 8B

| Field | Value |
|---|---|
| **Model ID** | `ministral-8b-latest` |
| **Status** | ✅ Active — Open |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.15 / MTok |
| **Context window** | 256,000 tokens |

---

### Ministral 3 - 3B

| Field | Value |
|---|---|
| **Model ID** | `ministral-3b-latest` |
| **Status** | ✅ Active — Open |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.10 / MTok |
| **Context window** | 256,000 tokens (up to 556K on some deployments) |

---

### Mistral NeMo *(Legacy Open-Weight, still on API)*

| Field | Value |
|---|---|
| **Model ID** | `open-mistral-nemo` |
| **Status** | ✅ Active (API) — Legacy open-weight, cheapest at $0.02/MTok on some hosts |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.15 / MTok |
| **Context window** | 128,000 tokens |

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

## 🤖 Discovery-Only: Non-LLM Model Releases *(not priced, not tracked as full cards)*

> Per this tracker's verification-before-tracking policy, releases without published API/token pricing are noted here for awareness only and are not given a full model card.

### Robostral Navigate *(Embodied Navigation — Released July 8, 2026)*

> **July 8, 2026 —** Mistral introduced **Robostral Navigate**, its first model built for embodied robot navigation. An 8B parameter model that takes RGB camera images plus a natural-language instruction and moves a robot through an environment, using only a single ordinary RGB camera (no depth sensors, LiDAR, or multi-camera rigs). Achieves 79.4% success (validation seen) / 76.6% success (validation unseen) on R2R-CE, beating the best single-camera approach by 9.7 points and the best multi-sensor system by 4.5 points. Trained on ~400,000 simulated trajectories across 6,000 scenes with a prefix-caching training method (22× more token-efficient) plus online RL (CISPO) post-training.
>
> **Why it's not a tracked model card:** Robostral Navigate is a robotics/embodied-AI research release, not a text/chat completions model, and **has no listing or pricing on `mistral.ai/pricing/api`** — there is no published per-token, per-call, or per-request rate. It will be evaluated for a full pricing card if/when Mistral publishes commercial API access and rates.
>
> Source: https://mistral.ai/news/robostral-navigate/

---

## 🔧 Platform Tool Pricing (Mistral AI Studio — Agent API)

> ✅ Re-confirmed August 3, 2026 against the live `mistral.ai/pricing/api` "Agent API" section — all figures unchanged.

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
| **Devstral 2** | 123B | Modified MIT | Self-hosted coding agents |
| **Devstral Small 2** | 24B | Apache 2.0 | Self-hosted budget coding agent (RTX 4090) |
| **Magistral Medium** | — | Apache 2.0 | Self-hosted reasoning |
| **Leanstral 1.5** | 119B (MoE, 6B active) | Apache 2.0 | Self-hosted Lean 4 formal proof engineering *(retiring Sept 30, 2026)* |
| **Voxtral Small 24B** | 24B | Apache 2.0 | Self-hosted audio understanding |
| **Voxtral Mini Transcribe Realtime** | — | Apache 2.0 | Self-hosted real-time transcription |
| **Voxtral TTS** | 4B | CC BY-NC 4.0 | Self-hosted TTS (non-commercial only) |
| **OCR 4** | — | Premier (API) | Self-hosted document OCR (enterprise, single container) |
| **Mixtral 8×22B** | 141B (MoE) | Apache 2.0 | Self-hosted complex reasoning |
| **Mixtral 8×7B** | 46.7B (MoE) | Apache 2.0 | General-purpose self-hosted |
| **Mistral 7B** | 7B | Apache 2.0 | Edge / on-device |

---

## ⚠️ Legacy Models

### ⚠️ LEGACY — OCR 3 v25.12 *(Superseded by OCR 4 — June 23, 2026)*

> **SUPERSEDED (June 23, 2026):** OCR 4 is now the flagship OCR model. `mistral-ocr-latest` alias now points to OCR 4. Per docs.mistral.ai: "OCR 4 is available as the newer model. OCR 3 remains available for existing integrations and production workloads."

| Field | Value |
|---|---|
| **Model ID** | `mistral-ocr-2512` |
| **Status** | ⚠️ LEGACY — Superseded by OCR 4 (June 23, 2026); available for existing integrations |
| **Last price** | $2.00 / 1,000 pages · $3.00 / 1,000 pages (annotations) |
| **Migration** | → **OCR 4** (`mistral-ocr-latest`) — $4/1K pages (standard), $2/1K pages (Batch-API), $5/1K pages (Document AI); adds bounding boxes, block classification |

---

### ⚠️ LEGACY — Voxtral Mini 3B v25.07 *(Moved to Legacy — June 2026)*

| Field | Value |
|---|---|
| **Model ID** | `voxtral-mini-2507` |
| **Status** | ⚠️ LEGACY — In legacy table at docs.mistral.ai; `voxtral-mini-latest` alias reassigned |
| **Last price** | $0.001/min (audio) · $0.04/MTok (text) · $0.04/MTok (output) |
| **Migration** | → **Voxtral Mini Transcribe 2** (`voxtral-mini-latest`, $0.003/min) for batch transcription · **Voxtral Mini Transcribe Realtime** ($0.006/min) for live transcription · **Voxtral Small 24B** ($0.004/min) for speech understanding |

---

### ⚠️ LEGACY — Leanstral v26.03 *(🔄 Replaced by Leanstral 1.5 — June 30, 2026)*

> 🔄 **REPLACED (June 30, 2026):** The original Leanstral (`labs-leanstral-2603`, v26.03, released March 16, 2026) has been superseded by **Leanstral 1.5** (`leanstral-1-5`, released June 30, 2026, now itself scheduled for retirement September 30, 2026). Both versions remain free; new projects should use Leanstral 1.5.

| Field | Value |
|---|---|
| **Model ID** | `labs-leanstral-2603` |
| **Status** | ⚠️ LEGACY — 🔄 Replaced by Leanstral 1.5 (June 30, 2026); still free while accessible |
| **Pricing** | **Free** *(while accessible)* |
| **Notable** | First open-source code agent for Lean 4 formal proof engineering; superseded by Leanstral 1.5 |
| **Migration** | → **Leanstral 1.5** (`leanstral-1-5`) — note: also scheduled for retirement Sept 30, 2026 |

---

### ⚠️ LEGACY — Mistral Medium 3.1 v25.08 *(Formally Deprecated June 2026)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-medium-2508` |
| **Status** | ⚠️ LEGACY — Confirmed in legacy table at docs.mistral.ai |
| **Last price** | $0.40 / MTok input · $2.00 / MTok output *(last confirmed)* |
| **Migration** | → **Mistral Medium 3.5** ($1.50/$7.50) for flagship; **Mistral Large 3** ($0.50/$1.50) for general; **Mistral Small 4** ($0.15/$0.60) for budget |

---

### ⚠️ LEGACY — Mistral Medium 3 v25.05

| Field | Value |
|---|---|
| **Model ID** | `mistral-medium-2505` |
| **Status** | ⚠️ LEGACY — Confirmed in legacy table at docs.mistral.ai |
| **Migration** | → **Mistral Medium 3.5** |

---

### ⚠️ LEGACY — Voxtral Mini Transcribe v25.07 *(Superseded by v26.02)*

| Field | Value |
|---|---|
| **Model ID** | `voxtral-mini-2507` |
| **Status** | ⚠️ LEGACY — Superseded by v26.02 versions (June 2026) |
| **Last price** | $0.002 / min |
| **Migration** | → **Voxtral Mini Transcribe 2** (v26.02, Premier, $0.003/min) for batch transcription; **Voxtral Mini Transcribe Realtime** (v26.02, Open, $0.006/min) for live transcription |

---

### ⚠️ LEGACY — Mistral Small Creative v25.12 *(Labs)*

| Field | Value |
|---|---|
| **Model ID** | `labs-mistral-small-creative` |
| **Status** | ⚠️ LEGACY — Listed in legacy table on docs.mistral.ai |
| **Last price** | $0.10 / MTok input · $0.30 / MTok output |
| **Migration** | Verify current availability on console.mistral.ai |

---

### ⚠️ LEGACY — Pixtral Large *(Deprecated — May 2026)*

| Field | Value |
|---|---|
| **Model ID** | `pixtral-large-2411` |
| **Status** | ⚠️ LEGACY — Deprecated per docs.mistral.ai; removed from mistral.ai/pricing |
| **Last price** | $2.00 input / $6.00 output per MTok |
| **Migration** | → **Mistral Medium 3.5** ($1.50/$7.50) or **Mistral Small 4** ($0.15/$0.60) |

---

### ⚠️ LEGACY — Magistral Small 1.2 / version 2509

| Field | Value |
|---|---|
| **Model ID** | `magistral-small-2509` |
| **Status** | ⚠️ LEGACY — Specific version deprecated per docs.mistral.ai; `magistral-small-latest` still active |
| **Last price** | $0.50 / $1.50 per MTok |
| **Migration** | Use `magistral-small-latest` for active routing, or **Mistral Small 4** with `reasoning_effort=high` ($0.15/$0.60) |

---

### ⚠️ LEGACY — Magistral Medium 1.2 v25.09 *(version 2509)*

| Field | Value |
|---|---|
| **Model ID** | `magistral-medium-2509` |
| **Status** | ⚠️ LEGACY — Specific version in legacy table at docs.mistral.ai; `magistral-medium-latest` alias still active and routes to current version |
| **Last price** | $2.00 / $5.00 per MTok |
| **Migration** | Use `magistral-medium-latest` for active routing |

---

### ⚠️ LEGACY — Magistral Medium 1.1 v25.07 *(version 2507)*

| Field | Value |
|---|---|
| **Model ID** | `magistral-medium-2507` |
| **Status** | ⚠️ LEGACY — Confirmed in legacy table at docs.mistral.ai; `magistral-medium-latest` alias still active |
| **Migration** | Use `magistral-medium-latest` for active routing |

---

### ⚠️ LEGACY — Devstral 2 v25.12 *(version devstral-2512)*

| Field | Value |
|---|---|
| **Model ID** | `devstral-2512` |
| **Status** | ⚠️ LEGACY — Specific version in legacy table at docs.mistral.ai; `devstral-medium-latest` alias still active |
| **Migration** | Use `devstral-medium-latest` for active routing |

---

### ⚠️ LEGACY — Devstral Small 2 v25.12 *(version labs-devstral-small-2512)*

| Field | Value |
|---|---|
| **Model ID** | `labs-devstral-small-2512` |
| **Status** | ⚠️ LEGACY — Specific version in legacy table at docs.mistral.ai; `devstral-small-latest` alias still active at $0.10/$0.30 |
| **Migration** | Use `devstral-small-latest` for active routing |

---

### ⚠️ LEGACY — Devstral Small 1.1 / 1.0

| Field | Value |
|---|---|
| **Model ID** | `devstral-small-1-1` / `devstral-small-2505` |
| **Status** | ⚠️ LEGACY — Superseded by Devstral Small 2 (Dec 2025) |
| **Migration** | → **Devstral Small 2** (`devstral-small-latest`, $0.10/$0.30) |

---

### ⚠️ LEGACY — Devstral Medium 1.0

| Field | Value |
|---|---|
| **Model ID** | `devstral-medium-2507` |
| **Status** | ⚠️ LEGACY — Superseded by Devstral 2 (Dec 2025) |
| **Migration** | → **Devstral 2** (`devstral-medium-latest`, $0.40/$2.00) or **Medium 3.5** ($1.50/$7.50) |

---

### ⚠️ LEGACY — Mistral Small 3.2 24B

| Field | Value |
|---|---|
| **Model ID** | `mistral-small-2506` |
| **Status** | ⚠️ LEGACY — Superseded by Mistral Small 4 (March 2026) |
| **Migration** | → **Mistral Small 4** (`mistral-small-latest`, $0.15/$0.60, 256K context) |

---

### ⚠️ LEGACY — Mistral Small 3.1 / 3.0 / Mistral Large 2.x / Codestral 2501 / 2405, Mistral Saba, Ministral 3B/8B (24.10), Pixtral 12B, Mistral Nemo 12B, Codestral Mamba, Mathstral, Mistral 7B, Mixtral 8x7B/8x22B (early versions), Mistral Large 1.0, Mistral Medium 1.0

| Model | Status | Migration |
|---|---|---|
| Mistral Small 3.1 (`mistral-small-2503`) | ⚠️ LEGACY | → Mistral Small 4 |
| Mistral Small 3.0 (`mistral-small-2501`) | ⚠️ LEGACY | → Mistral Small 4 |
| Mistral Large 2.1 (`mistral-large-2411`) | ⚠️ LEGACY | → Mistral Large 3 |
| Mistral Large 2.0 (`mistral-large-2407`) | ⚠️ LEGACY | → Mistral Large 3 |
| Codestral 2501 | ⚠️ LEGACY | → Codestral 2508 |
| Codestral 24.05 | ⚠️ LEGACY | → Codestral 2508 |
| Mistral Saba (`mistral-saba-2502`) | ⚠️ LEGACY | → Mistral Medium 3.5 (multilingual) |
| Pixtral Large (`pixtral-large-2411`) | ⚠️ LEGACY | → Mistral Medium 3.5 |
| Pixtral 12B (`pixtral-12b-2409`) | ⚠️ LEGACY | → Mistral Small 4 |
| Ministral 3B / 8B (24.10) | ⚠️ LEGACY | → Ministral 3 (3B/8B/14B) |
| Mistral Nemo 12B (`open-mistral-nemo-2407`) | ⚠️ LEGACY (API still active) | → Mistral Small 4 or Ministral 3 |
| Codestral Mamba 7B | ⚠️ LEGACY | → Codestral 2508 |
| Mathstral 7B | ⚠️ LEGACY | → Magistral Small |
| Mistral 7B (0.1/0.2/0.3) | ⚠️ LEGACY | → Ministral 3 3B |
| Mistral Large 1.0 (24.02) | ⚠️ LEGACY | → Mistral Large 3 |
| Mistral Small 1.0 (24.02) | ⚠️ LEGACY | → Mistral Small 4 |
| Mistral Medium 1.0 (23.12) | ⚠️ LEGACY | → Mistral Medium 3.5 |
| Mixtral 8x7B / 8x22B (original) | ⚠️ LEGACY (API still active) | → Mistral Small 4 / Large 3 |

---

## 💡 Cost Optimization Notes

| Feature | Notes |
|---|---|
| **Batch API discount** | 50% off — confirmed per mistral.ai/pricing |
| **No prompt caching** | Unlike OpenAI/Anthropic, Mistral does NOT offer prompt caching discounts |
| **EU data residency** | All API traffic processed in the EU by default |
| **Free tier** | Available via La Plateforme; rate-limited; no credit card required |
| **Classifier API fine-tuning** | Build custom classifiers from Ministral 3B ($0.10/$0.10) or 8B ($0.04/$0.04) inference |
| **📈 Small 4 price increase** | Mistral Small 4 increased to $0.15/$0.60 (from $0.10/$0.30). Use **Devstral Small 2** ($0.10/$0.30) for coding tasks or **Ministral 3B** ($0.10/$0.10) for simple tasks |
| **Budget reasoning** | Use Mistral Small 4 with `reasoning_effort=high` ($0.15/$0.60) as the budget reasoning option |
| **Voxtral transcription** | Voxtral Mini Transcribe 2 (`voxtral-mini-latest`, $0.003/min) for batch; Realtime ($0.006/min) for live |
| **OCR 4 batch savings** | OCR 4 Batch-API: $2/1K pages (50% off standard $4/1K pages) |
| **⚠️ Leanstral 1.5 retiring Sept 30, 2026** | Free Labs endpoint (`leanstral-1-5`) for Lean 4 formal proof engineering — has a published retirement date; no successor announced yet, so plan migration/monitoring ahead of that date |
| **⚠️ Ignore the stale "$2/$6" Large example** | The general `mistral.ai/pricing` FAQ page has an outdated Mistral Large example; always price Large 3 off the `mistral.ai/pricing/api` product table ($0.50/$1.50) |
| **Agent API tool costs add up** | Web search and code execution are both $30/1K calls on the Agent API — for high-volume agentic workloads, budget these alongside model token costs |
| **🔭 Robostral Navigate is unpriced** | Mistral's new embodied-navigation robotics model (July 8, 2026) has no published API pricing — do not budget for it as a text/chat model; it is a distinct robotics research release |

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

*Sources last verified: August 3, 2026 against `mistral.ai/pricing/api` (all active prices re-confirmed exactly, including OCR 4 $4/$2/$5 per 1K pages, Mistral Small 4 $0.15/$0.60, Mistral Medium 3.5 $1.50/$7.50, Mistral Large 3 $0.50/$1.50, Leanstral 1.5 free, and the full Agent API tool-pricing table), `docs.mistral.ai/models/overview`, and `mistral.ai/news`. No new priced model releases or price changes detected since the July 27, 2026 refresh. 🔭 Discovery-only: Mistral published "Introducing Robostral Navigate" (July 8, 2026), an 8B embodied-navigation robotics model with no published API pricing — noted for awareness only, not added as a tracked model card per this tracker's verification-before-tracking policy.*
