# 🔵 Mistral AI — Model Cards

> **Last updated:** 2026-09-14
> **Source:** https://mistral.ai/pricing · https://mistral.ai/pricing/api · https://docs.mistral.ai/models/overview · https://mistral.ai/news · https://docs.mistral.ai/resources/changelogs
> **Scraped / verified:** 2026-09-14 — ✅ **Re-verified against the live `mistral.ai/pricing/api` and `docs.mistral.ai/models/overview` pages.** Every active model price (Medium 3.5 $1.50/$7.50, Large 3 $0.50/$1.50, Small 4 $0.15/$0.60, Z.ai GLM 5.2 $1.40/$4.40, OCR 4.1 $4/1K pages, Magistral, Codestral, Devstral, Voxtral family, Ministral 3 tiers, Classifier APIs, embeddings, Agent API tool pricing) is **unchanged** since the September 7 refresh. 🆕 **Mistral raised €3B in a Series D round** (announced September 8, 2026, post-money valuation >€21B) — a **funding/company milestone with no pricing impact**. Checked `mistral.ai/news` through September 10, 2026 — two additional posts (a Cloudera partnership and a legacy-code-modernization case study) are both non-pricing.

All prices are **USD per million tokens (MTok)**. Mistral offers a **free experimentation tier** (rate-limited) — no credit card required to start. API and consumer (Vibe) subscriptions are billed **separately**.

> **Mistral's key differentiators:** Native EU data residency (GDPR by default) now paired with **GA'd regional endpoint choice** (EU or US), competitive mid-tier pricing, Apache 2.0 / Modified MIT open-weight models, dedicated reasoning (Magistral series), a flagship merged model (Medium 3.5), a growing **third-party open-model marketplace** (GLM-5.2, more to come), and a 50% batch processing discount.

> 📝 **September 14, 2026 update:**
> - ✅ Independently re-verified every active price point against `mistral.ai/pricing/api` — **all confirmed unchanged**: Medium 3.5 $1.50/$7.50, Large 3 $0.50/$1.50, Small 4 $0.15/$0.60, Magistral Medium $2/$5, Magistral Small $0.50/$1.50, Codestral $0.30/$0.90, Devstral 2 $0.40/$2.00, Devstral Small 2 $0.10/$0.30, OCR 4.1 $4/1K pages (std) · $2/1K (Batch) · $5/1K (Document AI), Z.ai GLM 5.2 $1.40/$0.14 cached/$4.40, Voxtral family, Ministral 3 tiers, Classifier APIs, embeddings, and Agent API tool pricing.
> - 🆕 **September 8, 2026 — Mistral raised €3 billion in a Series D funding round** at a post-money valuation of more than €21 billion, aimed at "making sovereign, open-weight AI the technology frontier." This is a **company/funding milestone — no product pricing changed** as a result.
> - ℹ️ Checked `mistral.ai/news` since the September 7 refresh: Sept 8 "Mistral raises €3B..." (funding, above), Sept 9 "Modernizing complex legacy code with AI agents" (solutions case study, not a priced model), Sept 10 "Cloudera and Mistral Partner to Bring Specialized, Sovereign Intelligence to Enterprise Data" (partnership announcement, not a priced model). **No new priced LLM/API model releases found this cycle.**
> - ✅ Independently re-verified the full models overview page (`docs.mistral.ai/models/overview`) — the featured/active lineup (Medium 3.5, OCR 4.1, Z.ai GLM 5.2, Small 4, Voxtral Mini Transcribe 2, Voxtral Mini Transcribe Realtime) and the deprecated-models table are unchanged from the prior refresh.

> 📝 **September 7, 2026 update:**
> - 🆕 **Z.ai GLM-5.2 now hosted on Mistral's platform** (announced August 11, 2026 in ["In-region inference, open models, and new European infrastructure for sovereign AI"](https://mistral.ai/news/regional-inference-open-models-new-compute/)) — the **first third-party open model** available through Mistral AI Studio, running on the same infrastructure, regional controls, and service commitments as native Mistral models. A 1M-token-context open-weight model specializing in long-context agentic workflows and coding. Pricing: **$1.40/MTok input · $0.14/MTok cached input · $4.40/MTok output**. Model ID: `zai-glm-5-2`. Factory (Matan Grinberg, CEO) is a named launch customer citing regional-control benefits.
> - 🆕 **OCR 4.1 launched**, superseding OCR 4.0 as Mistral's flagship OCR/document-intelligence model — same pricing ($4/1K pages standard, $5/1K Document AI), adds block-level confidence scores on top of OCR 4.0's paragraph-level bounding boxes and structural block labels. `mistral-ocr-latest` alias now points to OCR 4.1.
> - 🆕 **Mistral Regional Endpoints reached General Availability** (previously in preview) — customers can choose EU or US inference regions for supported models, with a confirmed **+10% surcharge**, addressing data-residency/regulatory/latency requirements.
> - 🆕 **Mistral Priority Tier entered public preview** — committed service levels for mission-critical workloads (custom rate limits, uptime SLA), positioning Mistral as offering both regional processing choice and an SLA-backed tier — something Mistral states no other European AI lab currently offers.
> - ℹ️ Checked `mistral.ai/news` since the August 10 refresh: Aug 20 "Agentic Search" (a retrieval-layer product feature, not a priced model), Aug 24 "Mistral x HUMAIN" (partnership announcement, not a model). No other new priced LLM releases found.
> - ✅ All previously tracked active prices (Medium 3.5 $1.50/$7.50, Large 3 $0.50/$1.50, Small 4 $0.15/$0.60, Magistral Medium $2/$5, Magistral Small $0.50/$1.50, Codestral $0.30/$0.90, Devstral 2 $0.40/$2.00, Devstral Small 2 $0.10/$0.30, Voxtral family, Ministral 3 tiers, Classifier APIs, embeddings, Agent API tool pricing) re-confirmed unchanged.

> 📝 **August 10, 2026 update:**
> - ✅ Independently re-verified every active price point against `mistral.ai/pricing/api` — **all confirmed unchanged**: Medium 3.5 $1.50/$7.50, Large 3 $0.50/$1.50, Small 4 $0.15/$0.60, Magistral Medium $2/$5, Magistral Small $0.50/$1.50, Codestral $0.30/$0.90, Devstral 2 $0.40/$2.00, Devstral Small 2 $0.10/$0.30, OCR 4 $4/1K pages (std) · $2/1K (Batch) · $5/1K (Document AI), Voxtral family, Ministral 3 tiers, Classifier APIs, embeddings, Agent API tool pricing (Web search/Code execution $30/1K calls, Image generation $100/1K images, etc.), and Mixtral/NeMo legacy-API models.
> - 🆕 **New discovery (not priced, not added as a full tracked model):** Mistral published **"Introducing Shieldstral"** (August 4, 2026) — a 3B (docs list 3.8B total/active parameters) open-weights, policy-adaptive multimodal safety classifier that accepts natural-language policy questions at inference time and returns a calibrated yes/no safety score for text and images, unifying prompt moderation, response moderation, and refusal detection into a single model. Released under Apache 2.0 as an inaugural member of the Open Secure AI Alliance (with NVIDIA and others); runs on a single 16GB GPU; 32K context window; listed as **Public Preview** on `docs.mistral.ai/models/model-cards/shieldstral-1-0`. **Mistral has not published a hosted API model ID or per-token rate for Shieldstral** — it does not appear as a priced row on `mistral.ai/pricing/api`, unlike the existing free `mistral-moderation-2603` classifier endpoint, which is a separate, already-priced (free) product. Per this tracker's policy of verifying pricing before adding a full model card, Shieldstral is documented in the Discovery-Only section below and will be upgraded to a full card if/when Mistral publishes API access and pricing. Source: https://mistral.ai/news/shieldstral/ · https://docs.mistral.ai/models/model-cards/shieldstral-1-0
> - ℹ️ Checked `mistral.ai/news` for releases since the August 3 refresh — the only new post is Shieldstral (above); no other new priced LLM/API model releases found.

> 📝 **August 3, 2026 update:**
> - ✅ Independently re-verified every active price point against `mistral.ai/pricing/api` — **all confirmed unchanged**: Medium 3.5 $1.50/$7.50, Large 3 $0.50/$1.50, Small 4 $0.15/$0.60, Magistral Medium $2/$5, Magistral Small $0.50/$1.50, Codestral $0.30/$0.90, Devstral 2 $0.40/$2.00, Devstral Small 2 $0.10/$0.30, OCR 4 $4/1K pages (std) · $2/1K (Batch) · $5/1K (Document AI), Voxtral family, Ministral 3 tiers, Classifier APIs, embeddings, Agent API tool pricing (Web search/Code execution $30/1K calls, Image generation $100/1K images, etc.), and Mixtral/NeMo legacy-API models.
> - 🔭 **New discovery (not priced, not added as a tracked model):** Mistral published "Introducing Robostral Navigate" (July 8, 2026) — an 8B parameter embodied-navigation model that lets robots navigate complex environments using a single RGB camera (no LiDAR/depth sensors), achieving 76.6% on R2R-CE validation-unseen. This is a robotics/embodied-AI research release, not a text/chat LLM, and **no API pricing or token rates are published** for it — it does not appear on `mistral.ai/pricing/api`. Per this tracker's policy of verifying pricing before adding a model card, Robostral Navigate is noted here for awareness only and will be evaluated for a full card if/when Mistral publishes API access and pricing.
> - ℹ️ Checked `mistral.ai/news` for releases since the July 27 refresh — the most recent items are "Your Prompts and Skills need a system of record" (Studio feature, July 9, 2026) and Robostral Navigate (above); **no new priced LLM/API model releases found.**

---

## ✅ Active / Recommended Models

### 🆕 Z.ai GLM-5.2 *(Third-Party Open Model — Added to Mistral's Platform August 11, 2026)*

> **August 11, 2026 —** Mistral began hosting **Z.ai's GLM-5.2**, its first third-party open model, as part of a broader push to expand model choice on Mistral's regionally-controlled infrastructure without fragmenting where customers' AI runs. GLM-5.2 is a long-context agentic/coding model with a **1M-token context window**, running under the same regional controls and SLA commitments as native Mistral models. Announced alongside the Open Secure AI Alliance and NVIDIA Nemotron Coalition partnerships.

| Field | Value |
|---|---|
| **Provider** | Z.ai *(hosted on Mistral AI Studio)* |
| **Model ID** | `zai-glm-5-2` |
| **Added to Mistral** | August 11, 2026 |
| **Status** | ✅ Active — **First third-party open model on Mistral's platform** |
| **Input price** | $1.40 / MTok |
| **Cached input price** | $0.14 / MTok *(90% off — Mistral's first cached-input discount for a hosted model)* |
| **Output price** | $4.40 / MTok |
| **Context window** | 1,000,000 tokens |
| **License** | Open |
| **Capabilities** | Text-to-text, long-context agentic workflows, coding |
| **Availability** | Mistral AI Studio / La Plateforme, with EU/US Regional Endpoint choice and Priority Tier support like native Mistral models |
| **Notable** | Specializes in long-context agentic workflows and coding; Factory (coding-agent startup) cited it as a launch customer for regional-control benefits. Represents a strategic shift — Mistral's platform now brokers third-party open models, not just its own |

---

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
| **Notable** | Cheapest output pricing vs peers; GDPR-compliant EU hosting; open-weight, general-purpose multimodal model. ⚠️ Re-confirmed September 14, 2026 against the live `mistral.ai/pricing/api` product table — do not confuse with the stale "$2/$6" example on the general `mistral.ai/pricing` FAQ page |

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

| Field | Value |
|---|---|
| **Model ID** | `devstral-small-latest` |
| **Status** | ✅ Active — Labs tag on pricing page |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.30 / MTok |
| **Context window** | 256,000 tokens |
| **Notable** | Best lightweight, open model for coding agents; deployable on single RTX 4090/32GB Mac at Q4 |

---

### Leanstral 1.5 *(Labs — ⚠️ scheduled retirement Sept 30, 2026)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `leanstral-1-5` |
| **Released** | June 30, 2026 |
| **Scheduled retirement** | September 30, 2026 (per docs.mistral.ai changelog) |
| **Status** | ✅ Active — Labs — retirement date published, now ~2 weeks out from this refresh |
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
| **Pricing** | $0.016 per 1,000 characters |
| **Notable** | State-of-the-art TTS with zero-shot voice cloning and multilingual support; 4B params; CC BY-NC 4.0 (non-commercial) |

---

### OCR 4.1 *(Flagship OCR, supersedes OCR 4.0)*

> **OCR 4.1 supersedes OCR 4.0** as Mistral's flagship OCR model, confirmed on the live `mistral.ai/pricing/api` product table. Adds **block-level confidence scores** on top of OCR 4.0's paragraph-level bounding boxes and structural block labels. `mistral-ocr-latest` alias points to 4.1; pricing is unchanged from OCR 4.0.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-ocr-latest` *(alias — points to OCR 4.1)* / docs card `ocr-4-1` |
| **Status** | ✅ Active — **Flagship OCR** — Premier |
| **OCR price (standard)** | $4.00 / 1,000 pages |
| **OCR price (Batch-API)** | $2.00 / 1,000 pages *(50% off)* |
| **Document AI price** | $5.00 / 1,000 pages |
| **Availability** | API (Mistral Studio), Amazon SageMaker, Microsoft Foundry, self-hosted (enterprise) |
| **Capabilities** | Text extraction, paragraph-level bounding boxes, block classification (titles, tables, equations, signatures, headers/footers), block-level confidence scores, markdown output, 170-language support |
| **Notable** | "The world's best document extraction and understanding model" per Mistral; OCR 4.0 remains available for existing integrations |
| **Source** | https://mistral.ai/news/ocr-4/ · `mistral.ai/pricing/api` |

---

### ⚠️ LEGACY — OCR 4.0 *(Superseded by OCR 4.1)*

| Field | Value |
|---|---|
| **Model ID** | `ocr-4-0` |
| **Status** | ⚠️ LEGACY — Superseded by OCR 4.1; available for existing integrations |
| **Last price** | $4.00/1K pages (standard) · $2.00/1K (Batch) · $5.00/1K (Document AI) — identical to 4.1 |
| **Migration** | → **OCR 4.1** (`mistral-ocr-latest`) for confidence-score support; same price |

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
| **Input price** | $0.10 / MTok *(mistral.ai/pricing/api also lists this classifier as a free service tier — verify current billing in console)* |
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
| **Output price** | $0.20 / MTok |
| **Context window** | 256,000 tokens |

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
| **Status** | ✅ Active (API) — Legacy open-weight |
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

## 🌐 Regional Endpoints & Priority Tier *(GA / Public Preview — confirmed unchanged Sept 14, 2026)*

> Confirmed on `mistral.ai/news/regional-inference-open-models-new-compute/` (August 11, 2026) and `mistral.ai/pricing/api`.

| Feature | Status | Details |
|---|---|---|
| **Mistral Regional Endpoints** | ✅ **General Availability** | Choose EU or US inference region for supported models (including third-party models like GLM-5.2). **+10% surcharge.** Addresses data-residency, regulatory, and latency requirements. Subject to limited, safeguarded sub-processor transfers as described in Mistral's Trust Center. |
| **Mistral Priority Tier** | 🆕 **Public Preview** | Committed service levels for mission-critical workloads: custom rate limits, uptime SLA. Mistral states it is the only European AI lab offering both regional processing choice and an SLA-backed priority tier. |
| **Cached input tokens** | Configurable add-on | -90% on input tokens for repeated prompts (first applied as a first-class rate for GLM-5.2) |

---

## 🏦 Company Milestone: €3B Series D *(September 8, 2026 — non-pricing)*

> Mistral announced it raised **€3 billion in a Series D funding round** at a post-money valuation of more than **€21 billion**, framed around "making sovereign, open-weight AI the technology frontier." This is a **corporate funding milestone with no direct impact on API or subscription pricing** — no product prices changed alongside this announcement. Source: https://mistral.ai/news/mistral-makes-sovereign-open-weight-ai-to-frontier/

---

## 🤖 Discovery-Only: Non-LLM / Unpriced Model Releases *(not priced, not tracked as full cards)*

> Per this tracker's verification-before-tracking policy, releases without published API/token pricing are noted here for awareness only and are not given a full model card.

### Shieldstral 1.0 *(Open-Weight Multimodal Safety Classifier — Released August 4, 2026)*

> A 3B-class (3.8B total/active parameters) open-weights, policy-adaptive multimodal safety classifier for text and images. Accepts a plain-language policy question at inference time and returns a calibrated yes/no safety score. Built on a Ministral-3-3B backbone with a Pixtral vision encoder. Released under Apache 2.0 (`mistralai/Shieldstral-1.0`) as an inaugural member of the Open Secure AI Alliance. **No hosted API model ID or per-token rate published** — self-host only (single 16GB GPU). Distinct from the already-priced `mistral-moderation-2603` endpoint. Source: https://mistral.ai/news/shieldstral/

### Robostral Navigate *(Embodied Navigation — Released July 8, 2026)*

> An 8B parameter model for embodied robot navigation using a single RGB camera (no LiDAR/depth sensors). Achieves 79.4%/76.6% success (seen/unseen) on R2R-CE. **Has no listing or pricing on `mistral.ai/pricing/api`** — a robotics research release, not a text/chat model. Source: https://mistral.ai/news/robostral-navigate/

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
| **Devstral 2** | 123B | Modified MIT | Self-hosted coding agents |
| **Devstral Small 2** | 24B | Apache 2.0 | Self-hosted budget coding agent (RTX 4090) |
| **Magistral Medium** | — | Apache 2.0 | Self-hosted reasoning |
| **Leanstral 1.5** | 119B (MoE, 6B active) | Apache 2.0 | Self-hosted Lean 4 formal proof engineering *(retiring Sept 30, 2026)* |
| **Shieldstral 1.0** | 3.8B | Apache 2.0 | Self-hosted policy-adaptive text/image safety classification *(no hosted API yet)* |
| **Voxtral Small 24B** | 24B | Apache 2.0 | Self-hosted audio understanding |
| **Voxtral Mini Transcribe Realtime** | — | Apache 2.0 | Self-hosted real-time transcription |
| **Voxtral TTS** | 4B | CC BY-NC 4.0 | Self-hosted TTS (non-commercial only) |
| **OCR 4.1** | — | Premier (API) | Self-hosted document OCR (enterprise, single container) |
| **Z.ai GLM-5.2** | — | Open | Hosted on Mistral's platform (not self-hosted, but open-weight) — long-context agentic/coding |
| **Mixtral 8×22B** | 141B (MoE) | Apache 2.0 | Self-hosted complex reasoning |
| **Mixtral 8×7B** | 46.7B (MoE) | Apache 2.0 | General-purpose self-hosted |
| **Mistral 7B** | 7B | Apache 2.0 | Edge / on-device |

---

## ⚠️ Legacy Models

### ⚠️ LEGACY — OCR 4.0 *(Superseded by OCR 4.1)*

> See full card above in Active Models section.

### ⚠️ LEGACY — OCR 3 v25.12 *(Superseded by OCR 4 line)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-ocr-2512` |
| **Status** | ⚠️ LEGACY — Superseded by the OCR 4 line (OCR 4.0, then 4.1); available for existing integrations |
| **Last price** | $2.00 / 1,000 pages · $3.00 / 1,000 pages (annotations) |
| **Migration** | → **OCR 4.1** (`mistral-ocr-latest`) — $4/1K pages (standard), $2/1K pages (Batch-API), $5/1K pages (Document AI) |

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

### ⚠️ LEGACY — Mistral Medium 3.1 v25.08

| Field | Value |
|---|---|
| **Model ID** | `mistral-medium-2508` |
| **Status** | ⚠️ LEGACY |
| **Migration** | → **Mistral Medium 3.5** ($1.50/$7.50) |

---

### ⚠️ LEGACY — Mistral Medium 3 v25.05

| Field | Value |
|---|---|
| **Model ID** | `mistral-medium-2505` |
| **Status** | ⚠️ LEGACY |
| **Migration** | → **Mistral Medium 3.5** |

---

### ⚠️ LEGACY — Voxtral Mini Transcribe v25.07

| Field | Value |
|---|---|
| **Model ID** | `voxtral-mini-2507` |
| **Status** | ⚠️ LEGACY — Superseded by v26.02 versions |
| **Migration** | → **Voxtral Mini Transcribe 2** or **Voxtral Mini Transcribe Realtime** |

---

### ⚠️ LEGACY — Mistral Small Creative v25.12 *(Labs)*

| Field | Value |
|---|---|
| **Model ID** | `labs-mistral-small-creative` |
| **Status** | ⚠️ LEGACY |
| **Migration** | Verify current availability on console.mistral.ai |

---

### ⚠️ LEGACY — Pixtral Large

| Field | Value |
|---|---|
| **Model ID** | `pixtral-large-2411` |
| **Status** | ⚠️ LEGACY |
| **Migration** | → **Mistral Medium 3.5** or **Mistral Small 4** |

---

### ⚠️ LEGACY — Magistral Small 1.2 / version 2509

| Field | Value |
|---|---|
| **Model ID** | `magistral-small-2509` |
| **Status** | ⚠️ LEGACY |
| **Migration** | Use `magistral-small-latest` |

---

### ⚠️ LEGACY — Magistral Medium 1.2 / 1.1

| Field | Value |
|---|---|
| **Model ID** | `magistral-medium-2509` / `magistral-medium-2507` |
| **Status** | ⚠️ LEGACY |
| **Migration** | Use `magistral-medium-latest` |

---

### ⚠️ LEGACY — Devstral 2 v25.12 / Devstral Small 2 v25.12

| Model | Status | Migration |
|---|---|---|
| `devstral-2512` | ⚠️ LEGACY | Use `devstral-medium-latest` |
| `labs-devstral-small-2512` | ⚠️ LEGACY | Use `devstral-small-latest` |

---

### ⚠️ LEGACY — Older Generations

| Model | Status | Migration |
|---|---|---|
| Devstral Small 1.1 / 1.0 | ⚠️ LEGACY | → Devstral Small 2 |
| Devstral Medium 1.0 | ⚠️ LEGACY | → Devstral 2 or Medium 3.5 |
| Mistral Small 3.2 24B | ⚠️ LEGACY | → Mistral Small 4 |
| Mistral Small 3.1 / 3.0 | ⚠️ LEGACY | → Mistral Small 4 |
| Mistral Large 2.1 / 2.0 | ⚠️ LEGACY | → Mistral Large 3 |
| Codestral 2501 / 24.05 | ⚠️ LEGACY | → Codestral 2508 |
| Mistral Saba | ⚠️ LEGACY | → Mistral Medium 3.5 (multilingual) |
| Pixtral 12B | ⚠️ LEGACY | → Mistral Small 4 |
| Ministral 3B / 8B (24.10) | ⚠️ LEGACY | → Ministral 3 (3B/8B/14B) |
| Mistral Nemo 12B | ⚠️ LEGACY (API still active) | → Mistral Small 4 or Ministral 3 |
| Codestral Mamba 7B | ⚠️ LEGACY | → Codestral 2508 |
| Mathstral 7B | ⚠️ LEGACY | → Magistral Small |
| Mistral 7B (0.1/0.2/0.3) | ⚠️ LEGACY | → Ministral 3 3B |
| Mistral Large / Small / Medium 1.0 | ⚠️ LEGACY | → Current generation equivalents |
| Mixtral 8x7B / 8x22B (original) | ⚠️ LEGACY (API still active) | → Mistral Small 4 / Large 3 |

---

## 💡 Cost Optimization Notes

| Feature | Notes |
|---|---|
| **Batch API discount** | 50% off — confirmed per mistral.ai/pricing |
| **No prompt caching (native Mistral models)** | Mistral's own models do NOT offer prompt caching discounts — but **GLM-5.2 (third-party) does**, at $0.14/MTok cached input (90% off) |
| **EU / US data residency** | Regional Endpoints GA — choose EU or US inference region (+10% surcharge) |
| **Priority Tier (public preview)** | SLA-backed committed service levels with custom rate limits for mission-critical workloads |
| **Free tier** | Available via La Plateforme; rate-limited; no credit card required |
| **GLM-5.2 for long-context agentic work** | $1.40/$4.40 per MTok, 1M context — a cheaper alternative to Mistral Medium 3.5 ($1.50/$7.50) for long-context, coding-heavy workloads, with a 90%-off cached-input option Mistral's own models lack |
| **Classifier API fine-tuning** | Build custom classifiers from Ministral 3B ($0.10/$0.10) or 8B ($0.04/$0.04) inference |
| **Budget reasoning** | Use Mistral Small 4 with `reasoning_effort=high` ($0.15/$0.60) as the budget reasoning option |
| **Voxtral transcription** | Voxtral Mini Transcribe 2 (`voxtral-mini-latest`, $0.003/min) for batch; Realtime ($0.006/min) for live |
| **OCR 4.1 batch savings** | Batch-API: $2/1K pages (50% off standard $4/1K pages) |
| **⚠️ Leanstral 1.5 retiring Sept 30, 2026** | Free Labs endpoint (`leanstral-1-5`) — now ~2 weeks out from this refresh; no successor announced yet |
| **⚠️ Ignore the stale "$2/$6" Large example** | The general `mistral.ai/pricing` FAQ page has an outdated Mistral Large example; always price Large 3 off the `mistral.ai/pricing/api` product table ($0.50/$1.50) |
| **Agent API tool costs add up** | Web search and code execution are both $30/1K calls on the Agent API |
| **Robostral Navigate is unpriced** | No published API pricing — do not budget for it as a text/chat model |
| **Shieldstral is unpriced (self-host only)** | No hosted API SKU or rate — using it today means self-hosting on your own GPU |
| **🆕 €3B Series D funding round** | September 8, 2026 — company milestone, no pricing impact |

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

*Sources last verified: September 14, 2026 against `mistral.ai/pricing/api` (all active prices re-confirmed, including Z.ai GLM-5.2, OCR 4.1's unchanged $4/$2/$5-per-1K-pages pricing, Mistral Small 4 $0.15/$0.60, Mistral Medium 3.5 $1.50/$7.50, Mistral Large 3 $0.50/$1.50, Leanstral 1.5 free, and the full Agent API tool-pricing table), `docs.mistral.ai/models/overview`, and `mistral.ai/news` (through September 10, 2026). **This cycle:** no new priced-model releases or price changes were found — every active and legacy price point matched the September 7 refresh exactly. The only notable news was Mistral's €3B Series D funding round (Sept 8, 2026), a corporate milestone with no pricing impact, plus a partnership announcement (Cloudera) and a solutions case study, both non-pricing. Shieldstral 1.0 and Robostral Navigate remain discovery-only (unpriced).*
