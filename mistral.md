# 🔵 Mistral AI — Model Cards

> **Last updated:** 2026-06-29
> **Source:** https://mistral.ai/pricing · https://docs.mistral.ai/models/overview
> **Scraped / verified:** 2026-06-29 — 🆕 **OCR 4 launched June 23, 2026** ($4/1K pages standard, $2/1K Batch, $5/1K Document AI) — supersedes OCR 3 as flagship OCR model. 📈 **Mistral Small 4 price increased**: $0.10→$0.15 input, $0.30→$0.60 output (verified on mistral.ai/pricing). ⚠️ **Voxtral Mini 3B** (`voxtral-mini-2507`) moved to legacy; `voxtral-mini-latest` alias now points to Voxtral Mini Transcribe 2. Multiple new entries in docs.mistral.ai legacy table.

All prices are **USD per million tokens (MTok)**. Mistral offers a **free experimentation tier** (rate-limited) — no credit card required to start. API and consumer (Vibe) subscriptions are billed **separately**.

> **Mistral's key differentiators:** Native EU data residency (GDPR by default), competitive mid-tier pricing, Apache 2.0 open-weight models, dedicated reasoning (Magistral series), flagship merged model (Medium 3.5), and a 50% batch processing discount.

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
| **Status** | ✅ Active — General Reasoning Flagship |
| **Input price** | $0.50 / MTok |
| **Output price** | $1.50 / MTok |
| **Context window** | 262,144 tokens (256K) |
| **Notable** | Cheapest output pricing vs peers; GDPR-compliant EU hosting; 675B total params, 41B active (MoE) |

---

### Magistral Medium *(Reasoning Model)*

> **Note (June 29, 2026):** Active via `magistral-medium-latest` at $2/$5. The specific version `magistral-medium-2509` is in legacy per docs.mistral.ai. `magistral-medium-latest` routes to the current active version.

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

> **Note (June 29, 2026):** `magistral-small-latest` still active on `mistral.ai/pricing` at $0.50/$1.50. The specific version `magistral-small-2509` is in legacy per docs.mistral.ai. Prefer Mistral Small 4 with `reasoning_effort=high` ($0.15/$0.60) for most reasoning tasks.

| Field | Value |
|---|---|
| **Model ID** | `magistral-small-latest` |
| **Status** | ✅ Active via `latest` alias (specific version `magistral-small-2509` is legacy per docs.mistral.ai) |
| **Input price** | $0.50 / MTok |
| **Output price** | $1.50 / MTok |
| **Context window** | 128,000 tokens |

---

### Mistral Small 4 *(Released March 16, 2026)*

> **📈 June 29, 2026 — Price increase confirmed on mistral.ai/pricing:** Input increased from $0.10 → **$0.15/MTok** (+50%). Output increased from $0.30 → **$0.60/MTok** (+100%). Note: Devstral Small 2 (`devstral-small-latest`) remains cheaper at $0.10/$0.30 for coding-focused use cases.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-small-latest` |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.15 / MTok *(📈 Updated — was $0.10/MTok as of June 22, 2026)* |
| **Output price** | $0.60 / MTok *(📈 Updated — was $0.30/MTok as of June 22, 2026)* |
| **Context window** | 262,144 tokens (256K) |
| **Capabilities** | Text, Vision, Function Calling, Reasoning (`reasoning_effort`), Agentic, Coding |
| **Notable** | 119B total params, 6B active (MoE); multimodal reasoning model; configurable `reasoning_effort` (none → high) |

---

### Codestral 2508 *(Updated August 2025)*

| Field | Value |
|---|---|
| **Model ID** | `codestral-latest` |
| **Status** | ✅ Active — Specialized (Code) |
| **Input price** | $0.30 / MTok |
| **Output price** | $0.90 / MTok |
| **Context window** | 256,000 tokens |
| **Notable** | Purpose-built code model; fill-in-the-middle (FIM); 70% cheaper than Codestral 2501 |

---

### Devstral 2 *(Coding Agent — Active via `devstral-medium-latest`)*

> **Note (June 29, 2026):** Active via `devstral-medium-latest` at $0.40/$2.00. The specific version `devstral-2512` is now in the legacy table at docs.mistral.ai. `devstral-medium-latest` routes to the current active version.

| Field | Value |
|---|---|
| **Model ID** | `devstral-medium-latest` |
| **Status** | ✅ Active — Agentic Coding *(superseded in Vibe by Medium 3.5)* |
| **Input price** | $0.40 / MTok |
| **Output price** | $2.00 / MTok |
| **Context window** | 256,000 tokens |
| **Notable** | SWE-bench Verified 72.2%; open-weight (modified MIT license) |

---

### Devstral Small 2 *(Active via `devstral-small-latest`)*

> **Note (June 29, 2026):** Active via `devstral-small-latest` at $0.10/$0.30. Labeled **[Labs]** on mistral.ai/pricing. The specific version `labs-devstral-small-2512` is now in the legacy table at docs.mistral.ai. `devstral-small-latest` routes to the current active version.

| Field | Value |
|---|---|
| **Model ID** | `devstral-small-latest` |
| **Status** | ✅ Active — Labs tag on pricing page |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.30 / MTok |
| **Context window** | 256,000 tokens |
| **Notable** | 24B params; ~58% SWE-bench Verified; deployable on single RTX 4090/32GB Mac at Q4 |

---

### Voxtral Small 24B *(Audio / Speech)*

| Field | Value |
|---|---|
| **Model ID** | `voxtral-small-latest` |
| **Status** | ✅ Active — Specialized (Audio) |
| **Input price (audio)** | $0.004 / min |
| **Input price (text)** | $0.10 / MTok |
| **Output price** | $0.40 / MTok |
| **Context window** | 128,000 tokens |

---

### Voxtral Mini Transcribe 2 *(Premier — v26.02)*

> **Re-verified June 29, 2026:** $0.003/min confirmed. `voxtral-mini-latest` alias now points to this model (reassigned from the deprecated Voxtral Mini 3B standalone).

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-mini-latest` *(alias — previously pointed to standalone Voxtral Mini; now points to Voxtral Mini Transcribe 2)* |
| **Released** | February 2026 (version 26.02) |
| **Status** | ✅ Active — Specialized (Transcription) — Premier |
| **Pricing** | $0.003 / min *(confirmed on mistral.ai/pricing — June 29, 2026)* |
| **Availability** | API (`/v1/audio/transcriptions`) |
| **Capabilities** | Batch speech-to-text transcription, speaker diarization, multilingual (13 languages) |
| **Notable** | Superseded original Voxtral Mini Transcribe (v25.07) and took over `voxtral-mini-latest` alias |

---

### Voxtral Mini Transcribe Realtime *(Open — v26.02)*

> **Re-verified June 29, 2026:** $0.006/min confirmed. Listed as Open (Apache 2.0) on `docs.mistral.ai`.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-mini-transcribe-realtime-2602` |
| **Released** | February 2026 (version 26.02) |
| **Status** | ✅ Active — Specialized (Real-time Transcription) — Open (Apache 2.0) |
| **Pricing** | $0.006 / min audio input *(confirmed on mistral.ai/pricing, June 29, 2026)* |
| **Availability** | API (`/v1/audio/transcriptions`) |
| **Capabilities** | Live/streaming speech-to-text transcription, low-latency, edge-compatible |
| **Notable** | Open-weight (Apache 2.0); purpose-built for real-time transcription use cases |

---

### Voxtral TTS *(Text-to-Speech — Released March 2026)*

| Field | Value |
|---|---|
| **Model ID** | `voxtral-mini-tts-latest` *(confirmed on mistral.ai/pricing — June 29, 2026; previously listed as `voxtral-tts`)* |
| **Status** | ✅ Active — Specialized (Text-to-Speech) |
| **Pricing** | $0.016 per 1,000 characters |
| **Notable** | 9-language TTS; zero-shot voice cloning; 4B params; open weights on HuggingFace (CC BY-NC 4.0 — non-commercial) |

---

### 🆕 OCR 4 *(Released June 23, 2026 — New Flagship OCR)*

> **🆕 June 23, 2026 — OCR 4 launched.** Supersedes OCR 3 as the flagship OCR model. `mistral-ocr-latest` alias now points to OCR 4. OCR 3 remains accessible for existing integrations. Source: https://mistral.ai/news/ocr-4/

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-ocr-latest` *(alias — now points to OCR 4)* |
| **Released** | June 23, 2026 |
| **Status** | ✅ Active — **Flagship OCR** — Premier |
| **OCR price (standard)** | $4.00 / 1,000 pages |
| **OCR price (Batch-API)** | $2.00 / 1,000 pages *(50% off)* |
| **Document AI price** | $5.00 / 1,000 pages |
| **Availability** | API (Mistral Studio), Amazon SageMaker, Microsoft Foundry, Snowflake Parse Document *(coming soon)*, self-hosted (enterprise) |
| **Capabilities** | Text extraction, **bounding boxes** (paragraph-level), block classification (titles, tables, equations, signatures, headers/footers), inline confidence scores, markdown output |
| **Languages** | 170 languages across 10 language groups (English, Western Europe, Eastern Europe, Middle Eastern, Chinese, East Asian, Southeast Asian, Specialized) |
| **Formats** | PDF, DOC, PPT, OpenDocument, and other common enterprise formats |
| **Notable** | OlmOCRBench #1 overall (85.20); OmniDocBench 93.07; human preference win rate ~72% vs all tested systems; compact enough for single-container self-hosted deployment; integrated with Mistral Search Toolkit |
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
| **Status** | ✅ Active — Specialized (Content Moderation) |
| **Input price** | $0.10 / MTok |
| **Notable** | 128K context window; jailbreaking detection; March 2026 (v2603) |

---

### Classifier API model 3B *(Fine-tunable Classifier)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Status** | ✅ Active — Specialized (Classification) |
| **Training cost** | $1.00 / MTok *(one-off fine-tuning; minimum $4 per job)* |
| **Storage cost** | $2.00 / month per model |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.10 / MTok |
| **Capabilities** | Content moderation, sentiment analysis, fraud detection, custom classification |
| **Notable** | Fine-tunes Ministral 3B; minimum $4 per fine-tuning job |

---

### Classifier API model 8B *(Fine-tunable Classifier — Larger)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Status** | ✅ Active — Specialized (Classification) |
| **Training cost** | $1.00 / MTok *(one-off fine-tuning; minimum $4 per job)* |
| **Storage cost** | $2.00 / month per model |
| **Input price** | $0.04 / MTok |
| **Output price** | $0.04 / MTok |
| **Capabilities** | Content moderation, sentiment analysis, fraud detection, custom classification |
| **Notable** | Fine-tunes Ministral 8B; lower inference cost than 3B variant at $0.04/$0.04 |

---

### Leanstral *(⚠️ Moved to Legacy — June 2026)*

> **⚠️ June 15, 2026:** Leanstral (`labs-leanstral-2603`, v26.03) has been moved to the legacy/deprecated table at `docs.mistral.ai/models/overview`. Still listed on `mistral.ai/pricing` — verify accessibility on console.mistral.ai before building new workloads.

| Field | Value |
|---|---|
| **Model ID** | `labs-leanstral-2603` |
| **Status** | ⚠️ LEGACY — In legacy table at docs.mistral.ai (June 2026); still on pricing page |
| **Pricing** | **Free** *(while accessible)* |
| **Notable** | First open-source code agent for Lean 4 formal proof engineering |

---

### Mistral Nemo

| Field | Value |
|---|---|
| **Model ID** | `open-mistral-nemo` |
| **Status** | ✅ Active — Ultra-Budget |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.15 / MTok |
| **Context window** | 128,000 tokens |

---

### Ministral 3 14B

| Field | Value |
|---|---|
| **Model ID** | `ministral-14b-latest` |
| **Status** | ✅ Active |
| **Input price** | $0.20 / MTok |
| **Output price** | $0.20 / MTok |
| **Context window** | 256,000 tokens |

---

### Ministral 3 8B

| Field | Value |
|---|---|
| **Model ID** | `ministral-8b-latest` |
| **Status** | ✅ Active |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.15 / MTok |
| **Context window** | 256,000 tokens |

---

### Ministral 3 3B

| Field | Value |
|---|---|
| **Model ID** | `ministral-3b-latest` |
| **Status** | ✅ Active |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.10 / MTok |
| **Context window** | 556,032 tokens |

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

## 🔧 Platform Tool Pricing (Mistral AI Studio)

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

> **SUPERSEDED (June 23, 2026):** OCR 4 is now the flagship OCR model. `mistral-ocr-latest` alias now points to OCR 4. Per docs.mistral.ai: "OCR 3 remains available for existing integrations and production workloads."

| Field | Value |
|---|---|
| **Model ID** | `mistral-ocr-2512` |
| **Status** | ⚠️ LEGACY — Superseded by OCR 4 (June 23, 2026); available for existing integrations |
| **Last price** | $2.00 / 1,000 pages · $3.00 / 1,000 pages (annotations) |
| **Migration** | → **OCR 4** (`mistral-ocr-latest`) — $4/1K pages (standard), $2/1K pages (Batch-API), $5/1K pages (Document AI); adds bounding boxes, block classification, 170-language support |

---

### ⚠️ LEGACY — Voxtral Mini 3B v25.07 *(Moved to Legacy — June 2026)*

> **MOVED TO LEGACY:** `voxtral-mini-2507` (the standalone Voxtral Mini 3B model) is now in the legacy table at `docs.mistral.ai`. The `voxtral-mini-latest` alias has been reassigned to Voxtral Mini Transcribe 2 (v26.02). Do not use `voxtral-mini-latest` expecting the old audio-understanding model.

| Field | Value |
|---|---|
| **Model ID** | `voxtral-mini-2507` |
| **Status** | ⚠️ LEGACY — In legacy table at docs.mistral.ai; `voxtral-mini-latest` alias reassigned |
| **Last price** | $0.001/min (audio) · $0.04/MTok (text) · $0.04/MTok (output) |
| **Migration** | → **Voxtral Mini Transcribe 2** (`voxtral-mini-latest`, $0.003/min) for batch transcription · **Voxtral Mini Transcribe Realtime** ($0.006/min) for live transcription · **Voxtral Small 24B** ($0.004/min) for speech understanding |

---

### ⚠️ LEGACY — Leanstral v26.03 *(Moved to Legacy June 2026)*

> **MOVED TO LEGACY (June 15, 2026):** `docs.mistral.ai/models/overview` now lists Leanstral (v26.03, `labs-leanstral-2603`) in the legacy/deprecated table.

| Field | Value |
|---|---|
| **Model ID** | `labs-leanstral-2603` |
| **Status** | ⚠️ LEGACY — Moved to legacy table at docs.mistral.ai (June 2026) |
| **Last price** | Free |
| **Migration** | No direct successor; check Mistral docs for alternatives |

---

### ⚠️ LEGACY — Mistral Medium 3.1 v25.08 *(Formally Deprecated June 2026)*

> **FORMALLY DEPRECATED (June 15, 2026):** `docs.mistral.ai/models/overview` confirms Mistral Medium 3.1 (`mistral-medium-2508`, v25.08) in the legacy/deprecated table.

| Field | Value |
|---|---|
| **Model ID** | `mistral-medium-2508` |
| **Status** | ⚠️ LEGACY — Confirmed in legacy table at docs.mistral.ai (June 2026) |
| **Last price** | $0.40 / MTok input · $2.00 / MTok output *(last confirmed)* |
| **Migration** | → **Mistral Medium 3.5** ($1.50/$7.50) for flagship; **Mistral Large 3** ($0.50/$1.50) for general; **Mistral Small 4** ($0.15/$0.60) for budget |

---

### ⚠️ LEGACY — Voxtral Mini Transcribe v25.07 *(Superseded by v26.02)*

> **MOVED TO LEGACY (June 9, 2026):** The original Voxtral Mini Transcribe (v25.07, `voxtral-mini-2507`) is now in the legacy table at `docs.mistral.ai`. Superseded by **Voxtral Mini Transcribe 2** (v26.02, Premier) and **Voxtral Mini Transcribe Realtime** (v26.02, Open).

| Field | Value |
|---|---|
| **Model ID** | `voxtral-mini-2507` |
| **Status** | ⚠️ LEGACY — Superseded by v26.02 versions (June 2026) |
| **Last price** | $0.002 / min |
| **Migration** | → **Voxtral Mini Transcribe 2** (v26.02, Premier, $0.003/min) for batch transcription; **Voxtral Mini Transcribe Realtime** (v26.02, Open, $0.006/min) for live transcription |

---

### ⚠️ LEGACY — Mistral Small Creative v25.12 *(Now in Legacy per docs.mistral.ai)*

| Field | Value |
|---|---|
| **Model ID** | `labs-mistral-small-creative` |
| **Status** | ⚠️ LEGACY — Listed in legacy table on docs.mistral.ai (June 2026); still on pricing page |
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
| **Status** | ⚠️ LEGACY — Specific version in legacy table at docs.mistral.ai (June 2026); `magistral-medium-latest` alias still active and routes to current version |
| **Last price** | $2.00 / $5.00 per MTok |
| **Migration** | Use `magistral-medium-latest` for active routing |

---

### ⚠️ LEGACY — Devstral 2 v25.12 *(version devstral-2512)*

| Field | Value |
|---|---|
| **Model ID** | `devstral-2512` |
| **Status** | ⚠️ LEGACY — Specific version in legacy table at docs.mistral.ai (June 2026); `devstral-medium-latest` alias still active |
| **Migration** | Use `devstral-medium-latest` for active routing |

---

### ⚠️ LEGACY — Devstral Small 2 v25.12 *(version labs-devstral-small-2512)*

| Field | Value |
|---|---|
| **Model ID** | `labs-devstral-small-2512` |
| **Status** | ⚠️ LEGACY — Specific version in legacy table at docs.mistral.ai (June 2026); `devstral-small-latest` alias still active at $0.10/$0.30 |
| **Migration** | Use `devstral-small-latest` for active routing |

---

### ⚠️ LEGACY — Devstral Small 1.1

| Field | Value |
|---|---|
| **Model ID** | `devstral-small-1-1` |
| **Status** | ⚠️ LEGACY — Superseded by Devstral Small 2 (Dec 2025) |
| **Migration** | → **Devstral Small 2** (`devstral-small-latest`, $0.10/$0.30) |

---

### ⚠️ LEGACY — Devstral Medium

| Field | Value |
|---|---|
| **Model ID** | `devstral-medium` |
| **Status** | ⚠️ LEGACY — Superseded by Devstral 2 (Dec 2025) |
| **Migration** | → **Devstral 2** (`devstral-medium-latest`, $0.40/$2.00) or **Medium 3.5** ($1.50/$7.50) |

---

### ⚠️ LEGACY — Mistral Small 3.2 24B

| Field | Value |
|---|---|
| **Model ID** | `mistral-small-3.2` |
| **Status** | ⚠️ LEGACY — Superseded by Mistral Small 4 (March 2026) |
| **Migration** | → **Mistral Small 4** (`mistral-small-latest`, $0.15/$0.60, 256K context) |

---

### ⚠️ LEGACY — Mistral Small 3.1 / 3.0 / Mistral Large 2

| Model | Status | Migration |
|---|---|---|
| Mistral Small 3.1 | ⚠️ LEGACY | → Mistral Small 4 |
| Mistral Small 3.0 | ⚠️ LEGACY | → Mistral Small 4 |
| Mistral Large 2 (2407) | ⚠️ LEGACY | → Mistral Large 3 |
| Codestral 2501 | ⚠️ LEGACY | → Codestral 2508 |

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

*Sources last verified: June 29, 2026 against `mistral.ai/pricing` (OCR 4 $4/$2/$5 per 1K pages confirmed; Mistral Small 4 price $0.15/$0.60 confirmed; all other active prices re-confirmed) and `docs.mistral.ai/models/overview` (OCR 3, Voxtral Mini 3B, Magistral Medium 1.2 v2509, Devstral 2 v25.12, Devstral Small 2 v25.12 confirmed in legacy table).*
