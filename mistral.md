# 🔵 Mistral AI — Model Cards

> **Last updated:** 2026-06-09
> **Source:** https://mistral.ai/pricing · https://docs.mistral.ai/models/overview
> **Scraped / verified:** 2026-06-09 — all active prices confirmed unchanged; new Voxtral Mini Transcribe v2/Realtime and Classifier API models added; legacy table updated.

All prices are **USD per million tokens (MTok)**. Mistral offers a **free experimentation tier** (rate-limited) — no credit card required to start. API and consumer (Vibe) subscriptions are billed **separately**.

> **Mistral's key differentiators:** Native EU data residency (GDPR by default), competitive mid-tier pricing, Apache 2.0 open-weight models, dedicated reasoning (Magistral series), flagship merged model (Medium 3.5), and a 50% batch processing discount.

> 🆕 **June 9, 2026 update:** New models confirmed on official `mistral.ai/pricing` and `docs.mistral.ai/models/overview`:
> - **NEW: Voxtral Mini Transcribe 2** (Premier, v26.02) — dedicated transcription endpoint, improved over the original v25.07 version. API ID: `voxtral-mini-2602` (verify on console)
> - **NEW: Voxtral Mini Transcribe Realtime** (Open, v26.02) — live transcription endpoint for real-time use. API ID: `voxtral-mini-transcribe-realtime`
> - **NEW: Classifier API model 3B** — fine-tunable classifier (moderation, sentiment, fraud detection). Training $1/MTok, Storage $2/month/model, Input $0.10, Output $0.10
> - **NEW: Classifier API model 8B** — fine-tunable classifier (larger). Training $1/MTok, Storage $2/month/model, Input $0.04, Output $0.04
> - **LEGACY UPDATE:** Original Voxtral Mini Transcribe v25.07 (`voxtral-mini-2507`) now in legacy per docs.mistral.ai. Devstral Small 2 now labeled [Labs] on pricing page. Mistral Small Creative now in legacy per docs.mistral.ai.
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

### Magistral Medium 1.2 *(Reasoning Model)*

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

> **Note (June 9, 2026):** `magistral-small-latest` still active on `mistral.ai/pricing` at $0.50/$1.50. The specific version `magistral-small-2509` is in legacy per docs.mistral.ai. Prefer Mistral Small 4 with `reasoning_effort=high` ($0.10/$0.30) for most reasoning tasks.

| Field | Value |
|---|---|
| **Model ID** | `magistral-small-latest` |
| **Status** | ✅ Active via `latest` alias (specific version `magistral-small-2509` is legacy per docs.mistral.ai) |
| **Input price** | $0.50 / MTok |
| **Output price** | $1.50 / MTok |
| **Context window** | 128,000 tokens |

---

### Mistral Medium 3.1 *(Active in docs — not on pricing page)*

> **⚠️ Note (June 9, 2026):** `mistral-medium-3-1` is **not listed on `mistral.ai/pricing`** as of this verification, but still appears in `docs.mistral.ai` as a Premier active model. Use the explicit model ID and verify accessibility before building new workloads on it.

| Field | Value |
|---|---|
| **Model ID** | `mistral-medium-3-1` |
| **Status** | ✅ Active per docs.mistral.ai — ⚠️ Removed from mistral.ai/pricing page |
| **Input price** | $0.40 / MTok *(last confirmed)* |
| **Output price** | $2.00 / MTok *(last confirmed)* |
| **Context window** | 131,072 tokens |

---

### Mistral Small 4 *(Released March 16, 2026)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-small-latest` |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.30 / MTok |
| **Context window** | 262,144 tokens (256K) |
| **Capabilities** | Text, Vision, Function Calling, Reasoning (`reasoning_effort`), Agentic, Coding |
| **Notable** | 119B total params, 6B active (MoE); cheapest multimodal reasoning model from a major provider; configurable `reasoning_effort` (none → high) |

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

### Devstral 2 (2512) *(Coding Agent)*

| Field | Value |
|---|---|
| **Model ID** | `devstral-medium-latest` |
| **Status** | ✅ Active — Agentic Coding *(superseded in Vibe by Medium 3.5)* |
| **Input price** | $0.40 / MTok |
| **Output price** | $2.00 / MTok |
| **Context window** | 256,000 tokens |
| **Notable** | 123B params; SWE-bench Verified 72.2%; open-weight (modified MIT license) |

---

### Devstral Small 2 *(Released December 10, 2025)*

> **Note (June 9, 2026):** Devstral Small 2 is labeled **[Labs]** on the official `mistral.ai/pricing` page as of this verification.

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

### Voxtral Mini *(Audio / Speech — 3B)*

| Field | Value |
|---|---|
| **Model ID** | `voxtral-mini-latest` |
| **Status** | ✅ Active — Specialized (Audio / Low-Latency Speech) |
| **Input price (audio)** | $0.001 / min |
| **Input price (text)** | $0.04 / MTok |
| **Output price** | $0.04 / MTok |
| **Context window** | 32,000 tokens |
| **Notable** | 4× cheaper than Voxtral Small for audio; Apache 2.0 open-weight |

---

### 🆕 Voxtral Mini Transcribe 2 *(Premier — v26.02)*

> **🆕 NEW (June 9, 2026):** Voxtral Mini Transcribe 2 is an improved transcription model (v26.02), superseding the original Voxtral Mini Transcribe (v25.07 — now in legacy). Listed on `mistral.ai/pricing` and `docs.mistral.ai`.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-mini-2602` *(verify exact ID on console.mistral.ai)* |
| **Released** | February 2026 (version 26.02) |
| **Status** | ✅ Active — Specialized (Transcription) — Premier |
| **Pricing** | $0.002 / min *(verify on console — same tier as original Voxtral Mini Transcribe)* |
| **Availability** | API (Mistral AI Studio — Premier tier) |
| **Capabilities** | Batch speech-to-text transcription, speaker diarization, multilingual (13 languages) |
| **Notable** | Improved over v25.07; replaces original Voxtral Mini Transcribe as the primary batch transcription endpoint |

---

### 🆕 Voxtral Mini Transcribe Realtime *(Open — v26.02)*

> **🆕 NEW (June 9, 2026):** Voxtral Mini Transcribe Realtime is a new live transcription model for real-time use cases. Listed as Open (Apache 2.0) on `docs.mistral.ai`.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-mini-transcribe-realtime` *(verify exact ID on console.mistral.ai)* |
| **Released** | February 2026 (version 26.02) |
| **Status** | ✅ Active — Specialized (Real-time Transcription) — Open (Apache 2.0) |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Live/streaming speech-to-text transcription, low-latency, edge-compatible |
| **Notable** | Open-weight (Apache 2.0); purpose-built for real-time transcription use cases; complements Voxtral Mini Transcribe 2 (batch) |

---

### Voxtral TTS *(Text-to-Speech — Released March 2026)*

| Field | Value |
|---|---|
| **Model ID** | `voxtral-tts` |
| **Status** | ✅ Active — Specialized (Text-to-Speech) |
| **Pricing** | $0.016 per 1,000 characters |
| **Notable** | 9-language TTS; zero-shot voice cloning; 4B params; open weights on HuggingFace (CC BY-NC 4.0 — non-commercial) |

---

### OCR 3 *(Premier — Document Extraction)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-ocr-latest` |
| **Status** | ✅ Active — Specialized (Document OCR) |
| **OCR price** | $2.00 / 1,000 pages |
| **Annotations price** | $3.00 / 1,000 pages |
| **Notable** | Best-in-class document extraction; powers Mistral Document AI stack |

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

### 🆕 Classifier API model 3B *(Fine-tunable Classifier)*

> **🆕 ADDED (June 9, 2026):** Classifier API model 3B is listed on the official `mistral.ai/pricing` page. Fine-tune Ministral 3B for classification tasks.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Status** | ✅ Active — Specialized (Classification) |
| **Training cost** | $1.00 / MTok *(one-off fine-tuning; minimum $4 per job)* |
| **Storage cost** | $2.00 / month per model |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.10 / MTok |
| **Capabilities** | Content moderation, sentiment analysis, fraud detection, custom classification |
| **Notable** | Fine-tunes Ministral 3B; minimum $4 per fine-tuning job; storage billed regardless of usage (models can be deleted any time) |

---

### 🆕 Classifier API model 8B *(Fine-tunable Classifier — Larger)*

> **🆕 ADDED (June 9, 2026):** Classifier API model 8B is listed on the official `mistral.ai/pricing` page. Fine-tune Ministral 8B for classification tasks.

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

### Leanstral *(Labs — Formal Proof Engineering)*

| Field | Value |
|---|---|
| **Model ID** | `labs-leanstral-2603` |
| **Status** | ✅ Active — Labs (Free during feedback-collection period) |
| **Pricing** | **Free** |
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
| **Devstral 2 (2512)** | 123B | Modified MIT | Self-hosted coding agents |
| **Devstral Small 2** | 24B | Apache 2.0 | Self-hosted budget coding agent (RTX 4090) |
| **Magistral Medium 1.2** | — | Apache 2.0 | Self-hosted reasoning |
| **Voxtral Small 24B** | 24B | Apache 2.0 | Self-hosted audio understanding |
| **Voxtral Mini 3B** | 3B | Apache 2.0 | Self-hosted lightweight ASR / edge |
| **Voxtral Mini Transcribe Realtime** | — | Apache 2.0 | Self-hosted real-time transcription |
| **Voxtral TTS** | 4B | CC BY-NC 4.0 | Self-hosted TTS (non-commercial only) |
| **Mixtral 8×22B** | 141B (MoE) | Apache 2.0 | Self-hosted complex reasoning |
| **Mixtral 8×7B** | 46.7B (MoE) | Apache 2.0 | General-purpose self-hosted |
| **Mistral 7B** | 7B | Apache 2.0 | Edge / on-device |

---

## ⚠️ Legacy Models

### ⚠️ LEGACY — Voxtral Mini Transcribe v25.07 *(Superseded by v26.02)*

> **🆕 MOVED TO LEGACY (June 9, 2026):** The original Voxtral Mini Transcribe (v25.07, `voxtral-mini-2507`) is now in the legacy table at `docs.mistral.ai`. Superseded by **Voxtral Mini Transcribe 2** (v26.02, Premier) and **Voxtral Mini Transcribe Realtime** (v26.02, Open).

| Field | Value |
|---|---|
| **Model ID** | `voxtral-mini-2507` |
| **Status** | ⚠️ LEGACY — Superseded by v26.02 versions (June 2026) |
| **Last price** | $0.002 / min |
| **Migration** | → **Voxtral Mini Transcribe 2** (v26.02, Premier) for batch transcription; **Voxtral Mini Transcribe Realtime** (v26.02, Open) for live transcription |

---

### ⚠️ LEGACY — Mistral Small Creative v25.12 *(Now in Legacy per docs.mistral.ai)*

> **MOVED TO LEGACY (June 9, 2026):** `docs.mistral.ai/models/overview` now lists Mistral Small Creative (v25.12, `labs-mistral-small-creative`) in the legacy/deprecated table. The `mistral.ai/pricing` page still shows the model and its pricing.

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
| **Migration** | → **Mistral Medium 3.5** ($1.50/$7.50) or **Mistral Small 4** ($0.10/$0.30) |

---

### ⚠️ LEGACY — Magistral Small 1.2 / version 2509

| Field | Value |
|---|---|
| **Model ID** | `magistral-small-2509` |
| **Status** | ⚠️ LEGACY — Specific version deprecated per docs.mistral.ai; `magistral-small-latest` still active |
| **Last price** | $0.50 / $1.50 per MTok |
| **Migration** | Use `magistral-small-latest` for active routing, or **Mistral Small 4** with `reasoning_effort=high` ($0.10/$0.30) |

---

### ⚠️ LEGACY — Devstral Small 1.1

| Field | Value |
|---|---|
| **Model ID** | `devstral-small-1-1` |
| **Status** | ⚠️ LEGACY — Superseded by Devstral Small 2 (Dec 2025) |
| **Migration** | → **Devstral Small 2** ($0.10/$0.30) |

---

### ⚠️ LEGACY — Devstral Medium

| Field | Value |
|---|---|
| **Model ID** | `devstral-medium` |
| **Status** | ⚠️ LEGACY — Superseded by Devstral 2 (Dec 2025) |
| **Migration** | → **Devstral 2** ($0.40/$2.00) or **Medium 3.5** ($1.50/$7.50) |

---

### ⚠️ LEGACY — Mistral Small 3.2 24B

| Field | Value |
|---|---|
| **Model ID** | `mistral-small-3.2` |
| **Status** | ⚠️ LEGACY — Superseded by Mistral Small 4 (March 2026) |
| **Migration** | → **Mistral Small 4** ($0.10/$0.30, 256K context) |

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
| **Classifier API fine-tuning** | Build custom classifiers from Ministral 3B ($0.04/$0.04) or 8B ($0.10/$0.10) inference |
| **Budget reasoning** | Use Mistral Small 4 with `reasoning_effort=high` ($0.10/$0.30) as the budget reasoning option |
| **Voxtral transcription** | Voxtral Mini ($0.001/min audio) is 4× cheaper than Voxtral Small ($0.004/min) for audio |
| **Voxtral Mini Transcribe 2 vs Realtime** | Use v26.02 Premier for batch; v26.02 Open/Realtime for live/streaming |
| **Leanstral (Labs)** | Free during feedback-collection period for Lean 4 formal verification |

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

*Sources last verified: June 9, 2026 against `mistral.ai/pricing` (all active prices confirmed unchanged; Classifier API model 3B and 8B confirmed; Devstral Small 2 confirmed as [Labs]; Voxtral Mini Transcribe v26.02 Premier and Realtime confirmed) and `docs.mistral.ai/models/overview` (Voxtral Mini Transcribe v25.07 in legacy; Mistral Small Creative v25.12 in legacy; Voxtral Mini Transcribe 2 v26.02 and Realtime v26.02 confirmed active).*