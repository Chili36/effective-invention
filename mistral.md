# 🔵 Mistral AI — Model Cards

> **Last updated:** 2026-06-08
> **Source:** https://mistral.ai/pricing · https://docs.mistral.ai/models/overview · https://mistral.ai/news/devstral-2-vibe-cli · https://mistral.ai/news/vibe-remote-agents-mistral-medium-3-5 · https://mistral.ai/news/voxtral/ · https://openrouter.ai/mistralai
> **Scraped / verified:** 2026-06-08

All prices are **USD per million tokens (MTok)**. Mistral offers a **free experimentation tier** (rate-limited) — no credit card required to start. API and consumer (Vibe) subscriptions are billed **separately**.

> **Mistral's key differentiators:** Native EU data residency (GDPR by default), competitive mid-tier output pricing, Apache 2.0 open-weight models for self-hosting, dedicated reasoning models (Magistral series), flagship merged model (Medium 3.5), and a batch processing discount (50% off).

> ✅ **May 28, 2026 update:** Multiple price corrections confirmed against `mistral.ai/pricing`:
> - **Devstral 2 output price corrected: $0.90 → $2.00 per MTok**
> - **Pixtral Large moved to Legacy** — no longer listed on `mistral.ai/pricing`
> - **Mistral Small 4: $0.15/$0.60 → $0.10/$0.30 per MTok**
> - **Ministral 3B: $0.04/$0.04 → $0.10/$0.10 per MTok**
> - **Ministral 8B: $0.10/$0.10 → $0.15/$0.15 per MTok**
> - **Voxtral Small pricing updated** — audio input now priced at $0.004/min; output updated to $0.40/MTok
> - **Batch processing discount confirmed**: 50% off for batch processing

> 🆕 **June 1, 2026 update:** Two new Voxtral Mini models added to pricing page. All other prices confirmed unchanged.
> - **NEW: Voxtral Mini** (audio understanding, 3B) — $0.001/min audio or $0.04/MTok text input; $0.04/MTok output (`voxtral-mini-latest`)
> - **NEW: Voxtral Mini Transcribe** — $0.002/min transcription endpoint (`voxtral-mini-latest` transcription mode); released May 15, 2026
> - **Mixtral 8x7B and 8x22B** confirmed available via API at $0.70/$0.70 and $2.00/$6.00 per MTok respectively

> 🆕 **June 8, 2026 update:** New models confirmed on official `mistral.ai/pricing` page. All previously listed prices confirmed unchanged.
> - **NEW: Leanstral** (Labs) — Free during feedback-collection period. First open-source code agent for Lean 4 formal proof engineering. API ID: `labs-leanstral-2603`
> - **NEW: Mistral Small Creative** (Labs) — $0.10/$0.30 per MTok. Fine-tuned small model for creative writing, roleplay, and chat. API ID: `labs-mistral-small-creative`
> - **NEW: OCR 3** (Premier) — $2.00 / 1K pages (OCR) + $3.00 / 1K pages (Annotations). Best-in-class document extraction. API ID: `mistral-ocr-latest`
> - **NEW: Codestral Embed** (Premier) — $0.15/MTok input only. State-of-the-art code + NL embeddings. API ID: `codestral-embed`
> - **NEW: Mistral Embed** — $0.10/MTok input only. General-purpose semantic embeddings. API ID: `mistral-embed`
> - **NEW: Mistral Moderation** — $0.10/MTok input only. Content moderation classifier. API ID: `mistral-moderation-2603`
> - **⚠️ Mistral Medium 3.1** — no longer listed on `mistral.ai/pricing` page as of June 8 verification. Still listed in `docs.mistral.ai/models/overview` as "Premier" active model. May have been removed from public API catalog; use explicit model ID `mistral-medium-3-1` and verify in API responses.

---

## ✅ Active / Recommended Models

### 🆕 Mistral Medium 3.5 *(Flagship — Released April 29, 2026)*

> **Released April 29, 2026:** Mistral's **first flagship merged model** — a single 128B dense model handling instruction-following, reasoning, coding, and vision. It is the default model in Mistral Vibe CLI and powers the new Work Mode in Le Chat. Pricing confirmed at $1.50/$7.50 per million tokens.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-medium-latest` *(check console.mistral.ai for alias routing)* |
| **Released** | April 29, 2026 |
| **Status** | ✅ Active — **Flagship** |
| **Input price** | $1.50 / MTok |
| **Output price** | $7.50 / MTok |
| **Context window** | 256,000 tokens |
| **Max output** | Not yet published (verify on console.mistral.ai) |
| **Availability** | API (Mistral AI Studio / La Plateforme); NVIDIA NIM; open weights on HuggingFace (modified MIT license) |
| **Capabilities** | Text, Vision (variable image sizes/aspect ratios), Function Calling, JSON mode, Configurable reasoning effort (`reasoning_effort`: none / low / medium / high), Agentic coding, 24-language support |
| **Notable** | First Mistral flagship **merged** model; 128B dense (non-MoE — all params active per pass); SWE-Bench Verified 77.6%; τ³-Telecom 91.4%; self-hostable on as few as 4× A100/H100 80GB GPUs; default model for Mistral Vibe CLI and Le Chat Work Mode; open weights under modified MIT license; 40% faster than Devstral 2 on coding tasks |

> ⚠️ **Model alias note:** The `mistral-medium-latest` alias may now route to Medium 3.5 instead of Medium 3.1. Check which version your calls land on via the `model` field in API responses. Medium 3.5 at $1.50/$7.50 is significantly more expensive than Medium 3.1 at $0.40/$2.00.

---

### Mistral Large 3 (2512)

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-large-latest` |
| **Released** | December 1, 2025 (version 2512) |
| **Status** | ✅ Active — General Reasoning Flagship |
| **Input price** | $0.50 / MTok |
| **Output price** | $1.50 / MTok |
| **Context window** | 262,144 tokens (256K) |
| **Max output** | 8,192 tokens |
| **Availability** | API (Mistral AI Studio / La Plateforme), Azure AI Foundry |
| **Capabilities** | Text, Vision, Function Calling, JSON mode |
| **Rate limits** | Paid tier; contact Mistral for enterprise limits |
| **Notable** | Exceptionally cheap output pricing vs peers; GDPR-compliant EU hosting by default; 256K context window; open-weight under Apache 2.0; 675B total params, 41B active (MoE) |

---

### Magistral Medium 1.2 *(Reasoning Model)*

> **Note (May 2026):** With the release of Mistral Medium 3.5, which includes configurable reasoning effort, Magistral Medium is now redundant for most use cases. Prefer Medium 3.5 for combined reasoning + coding + vision workloads. Magistral Medium remains available as a dedicated reasoning API model.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `magistral-medium-latest` *(or `magistral-medium-2509`)* |
| **Released** | September 17, 2025 (version 2509) |
| **Status** | ✅ Active — Reasoning (Dedicated) |
| **Input price** | $2.00 / MTok |
| **Output price** | $5.00 / MTok |
| **Context window** | 128,000 tokens *(performance degrades past ~40K — keep inputs under 40K for best results)* |
| **Max output** | 40,000 tokens |
| **Availability** | API (Mistral AI Studio) — open-weight (Apache 2.0) |
| **Capabilities** | Chain-of-thought reasoning, multilingual reasoning (20+ languages), complex problem-solving, multi-step logic, vision |
| **Notable** | Mistral's standalone reasoning model; transparent reasoning traces; multilingual chain-of-thought; open-weight deployment possible. For most tasks, **Mistral Medium 3.5** with `reasoning_effort=high` covers this use case at lower cost. |

---

### Magistral Small *(Active via `magistral-small-latest`)*

> **Note (June 1, 2026):** The `magistral-small-latest` alias is still listed as active on `mistral.ai/pricing` at $0.50/$1.50 per MTok. Note: the specific version `magistral-small-2509` was listed as deprecated in `docs.mistral.ai/models/overview` in May 2026 — this may indicate a newer version routes via the `latest` alias while the specific 2509 version is deprecated. Verify your API response `model` field to confirm which version you receive. For most reasoning tasks, **Mistral Small 4** with `reasoning_effort=high` ($0.10/$0.30) provides equivalent capability at lower cost.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `magistral-small-latest` |
| **Status** | ✅ Active via `latest` alias (specific version `magistral-small-2509` is deprecated per docs.mistral.ai) |
| **Input price** | $0.50 / MTok |
| **Output price** | $1.50 / MTok |
| **Context window** | 128,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Lightweight reasoning, multilingual, transparent chain-of-thought |
| **Notable** | Budget dedicated reasoning model; prefer Mistral Small 4 with `reasoning_effort=high` ($0.10/$0.30) for most use cases |

---

### Mistral Medium 3.1 *(Updated August 2025)*

> **⚠️ Note (June 8, 2026):** Mistral Medium 3.5 supersedes Medium 3.1 for most use cases. The `mistral-medium-latest` alias may now route to Medium 3.5. **As of June 8, 2026, `mistral-medium-3-1` is no longer listed on the `mistral.ai/pricing` page** — it still appears in `docs.mistral.ai/models/overview` as a "Premier" active model, but removal from the pricing page may indicate it is being quietly phased out. Use the explicit model ID and verify via API response `model` field. Medium 3.1 remains the budget text option if still accessible.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-medium-3-1` *(use explicit model ID — `mistral-medium-latest` may route to Medium 3.5; **not listed on mistral.ai/pricing as of June 8, 2026**)* |
| **Released** | August 2025 (supersedes Medium 3, May 2025) |
| **Status** | ✅ Active per docs.mistral.ai — ⚠️ **Removed from mistral.ai/pricing page (June 8, 2026)** |
| **Input price** | $0.40 / MTok *(last confirmed price — verify current availability)* |
| **Output price** | $2.00 / MTok *(last confirmed price)* |
| **Context window** | 131,072 tokens |
| **Max output** | 8,192 tokens |
| **Availability** | API (Mistral AI Studio) — verify current accessibility |
| **Capabilities** | Text, Function Calling, JSON mode |
| **Notable** | Budget option vs Medium 3.5 (3.75× cheaper input, 3.75× cheaper output); use for high-volume text workloads not requiring vision or reasoning. Check availability before building new workloads on this model. |

---

### Mistral Small 4 *(Released March 16, 2026)*

> **Price update (May 28, 2026):** Official `mistral.ai/pricing` now shows $0.10/$0.30 per MTok, down from the $0.15/$0.60 at launch. Confirmed against official pricing page (June 8, 2026).

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-small-latest` *(alias for `mistral-small-2603`)* |
| **Released** | March 16, 2026 |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.30 / MTok |
| **Context window** | 262,144 tokens (256K) |
| **Availability** | API (Mistral AI Studio); open weights (Apache 2.0) |
| **Capabilities** | Text, Vision (multimodal input), Function Calling, Reasoning (`reasoning_effort` param), Agentic tasks, Coding |
| **Notable** | Merges three models into one: Magistral (reasoning), Pixtral (multimodal vision), Devstral (agentic coding); configurable `reasoning_effort` (none → high) per request; 119B total params, only 6B active per token (MoE 128 experts, 4 active); cheapest multimodal reasoning model from a major provider |

---

### Codestral 2508 *(Updated August 2025)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `codestral-latest` |
| **Released** | August 2025 (version 2508; supersedes Codestral 2501) |
| **Status** | ✅ Active — Specialized (Code) |
| **Input price** | $0.30 / MTok |
| **Output price** | $0.90 / MTok |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio); free Codestral API endpoint for IDE integrations |
| **Capabilities** | Code generation, code completion, fill-in-the-middle (FIM), code refactoring |
| **Notable** | Purpose-built code model; 70% cheaper than previous Codestral 2501 ($1.00/$3.00); powers Mistral Vibe coding agent (alongside Medium 3.5 for agentic sessions) |

---

### Devstral 2 (2512) *(Coding Agent)*

> **Price correction (May 28, 2026):** Devstral 2 output price corrected to **$2.00/MTok**. The official Mistral launch announcement (`mistral.ai/news/devstral-2-vibe-cli`) stated "After the free period, the API pricing will be $0.40/$2.00 per million tokens." OpenRouter also confirms $0.40/$2.00.

> **Note (May 2026):** Devstral 2 has been replaced by **Mistral Medium 3.5** as the default model in Mistral Vibe CLI for agentic coding sessions. Devstral 2 remains available via API. For smaller-scale agentic coding, consider **Devstral Small 2** ($0.10/$0.30).

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `devstral-medium-latest` *(updated alias; also `devstral-2-2512`)* |
| **Released** | December 10, 2025 |
| **Status** | ✅ Active — Agentic Coding *(superseded in Vibe by Medium 3.5)* |
| **Input price** | $0.40 / MTok |
| **Output price** | $2.00 / MTok |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio); open-weight (modified MIT license) |
| **Capabilities** | Advanced agentic coding, CI/CD automation, multi-file reasoning, codebase exploration |
| **Notable** | Purpose-built for autonomous coding agents; 123B parameters; SWE-bench Verified 72.2%; open-weight (modified MIT license — large-revenue enterprises should review terms); superseded in Vibe CLI by Medium 3.5 but still available for API use |

---

### Devstral Small 2 *(Released December 10, 2025)*

> **Note (May 28, 2026):** The `labs-devstral-small-2512` Labs variant is deprecated per `docs.mistral.ai`. The production `devstral-small-latest` alias remains active.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `devstral-small-latest` *(ensure not `labs-devstral-small-2512` — Labs variant deprecated)* |
| **Released** | December 10, 2025 (companion release with Devstral 2) |
| **Status** | ✅ Active — Agentic Coding (Budget / Local) |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.30 / MTok |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio); open-weight (Apache 2.0) — deployable on single RTX 4090, RTX 3090, or 32GB+ Mac |
| **Capabilities** | Agentic coding, multi-file editing, autonomous bug fixing, CI/CD automation, codebase navigation, image inputs (multimodal) |
| **Notable** | 24B parameters; ~58% SWE-bench Verified; 256K context; requires ~14GB VRAM at Q4 for local deployment; Apache 2.0 license for self-hosting |

---

### Voxtral Small 24B *(Audio / Speech)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-small-latest` |
| **Released** | October 2025 (version 2507) |
| **Status** | ✅ Active — Specialized (Audio) |
| **Input price (audio)** | $0.004 / min |
| **Input price (text)** | $0.10 / MTok |
| **Output price** | $0.40 / MTok |
| **Context window** | 128,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Audio processing, voice understanding, speech-to-text, audio analysis, instruct use cases |
| **Notable** | Mistral's core audio instruct model; purpose-built for voice and speech workloads; 24B parameters |

---

### Voxtral Mini *(Audio / Speech — 3B)*

> **🆕 NEW (June 1, 2026):** Voxtral Mini is Mistral's lightweight speech intelligence model. It is listed on the official `mistral.ai/pricing` page. Lower-cost alternative to Voxtral Small for edge, embedded, and cost-sensitive audio workloads. Available as open weights (Apache 2.0) on HuggingFace.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-mini-latest` |
| **Released** | ~July 2025 (version 2507; companion to Voxtral Small) |
| **Status** | ✅ Active — Specialized (Audio / Low-Latency Speech) |
| **Input price (audio)** | $0.001 / min |
| **Input price (text)** | $0.04 / MTok |
| **Output price** | $0.04 / MTok |
| **Context window** | 32,000 tokens |
| **Availability** | API (Mistral AI Studio); open-weight (Apache 2.0) on HuggingFace |
| **Capabilities** | Low-latency speech recognition, audio understanding, transcription, voice Q&A, speech translation |
| **Notable** | 3B parameters; 4× cheaper than Voxtral Small for audio input ($0.001 vs $0.004/min); ideal for edge deployment, real-time transcription, and cost-sensitive ASR workloads; Apache 2.0 licensed; outperforms GPT-4o mini Transcribe and Gemini 2.5 Flash on several benchmarks |

---

### Voxtral Mini Transcribe *(Transcription — Released May 15, 2026)*

> **🆕 NEW (June 1, 2026):** Voxtral Mini Transcribe is a transcription-optimized endpoint of the Voxtral Mini model. Listed on the official `mistral.ai/pricing` page as a distinct pricing tier for pure transcription workloads. Uses the `voxtral-mini-latest` model endpoint with transcription-optimized decoding.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-mini-latest` *(transcription endpoint)* |
| **Released** | May 15, 2026 |
| **Status** | ✅ Active — Specialized (Transcription) |
| **Pricing** | $0.002 / min *(official mistral.ai/pricing page, verified June 8, 2026)* |
| **Availability** | API (Mistral AI Studio audio transcription endpoint) |
| **Capabilities** | Batch speech-to-text transcription, speaker diarization, 13-language support (English, Chinese, Hindi, Spanish, Arabic, French, Portuguese, Russian, German, Japanese, Korean, Italian, Dutch) |
| **Notable** | Transcription-specific variant of Voxtral Mini; optimized for batch ASR workloads; supports diarization; outperforms OpenAI Whisper large-v3 at less than half the price; ~4% WER on FLEURS benchmark; processes audio ~3× faster than ElevenLabs Scribe v2 while matching quality. OpenRouter lists this at $0.003/min — use official Mistral API pricing ($0.002/min) as canonical |

---

### Voxtral TTS *(Text-to-Speech — Released March 2026)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-tts` *(verify exact ID on console)* |
| **Released** | March 23, 2026 |
| **Status** | ✅ Active — Specialized (Text-to-Speech) |
| **Pricing** | $0.016 per 1,000 characters |
| **Availability** | API (Mistral AI Studio); open weights on HuggingFace (CC BY-NC 4.0 — non-commercial) |
| **Capabilities** | Multilingual TTS (9 languages: English, French, German, Spanish, Dutch, Portuguese, Italian, Hindi, Arabic), zero-shot voice cloning (3s reference), cross-lingual voice transfer, emotionally expressive voices, low-latency streaming (70ms on H200), enterprise voice agents |
| **Model size** | 4B parameters (based on Ministral 3B) |
| **Notable** | First Mistral TTS model; direct competitor to ElevenLabs; self-hostable on 16GB VRAM+ GPU |

---

### 🆕 OCR 3 *(Premier — Document Extraction)*

> **🆕 ADDED (June 8, 2026):** OCR 3 is now formally documented with pricing from the official `mistral.ai/pricing` page. It is Mistral's best-in-class document extraction and understanding model, powering the Document AI stack.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-ocr-latest` |
| **Released** | December 2025 (v25.12) |
| **Status** | ✅ Active — Specialized (Document OCR) |
| **OCR price** | $2.00 / 1,000 pages |
| **Annotations price** | $3.00 / 1,000 pages |
| **Availability** | API (Mistral AI Studio) — Premier tier |
| **Capabilities** | Document extraction, table parsing, formula recognition, multilingual OCR, structured output, multimodal document understanding |
| **Notable** | "The world's best document extraction and understanding model" per Mistral; powers Mistral Document AI stack; Page-level billing (not token-based); supports complex layouts including scientific papers, financial documents, and forms |

---

### 🆕 Codestral Embed *(Premier — Code Embeddings)*

> **🆕 ADDED (June 8, 2026):** Codestral Embed is now formally documented with pricing from the official `mistral.ai/pricing` page.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `codestral-embed` |
| **Released** | May 2025 (v25.05) |
| **Status** | ✅ Active — Specialized (Code Embeddings) |
| **Input price** | $0.15 / MTok *(input/query only — embeddings have no output tokens)* |
| **Availability** | API (Mistral AI Studio) — Premier tier |
| **Capabilities** | Code semantic search, code retrieval, NL-to-code similarity, dual-encoder for code + natural language |
| **Notable** | State-of-the-art embeddings for code and natural language queries; enables code search pipelines, RAG over codebases, and semantic code review |

---

### 🆕 Mistral Embed *(General Embeddings)*

> **🆕 ADDED (June 8, 2026):** Mistral Embed is now formally documented with pricing from the official `mistral.ai/pricing` page.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-embed` |
| **Released** | December 2023 (v23.12) |
| **Status** | ✅ Active — Specialized (General Embeddings) |
| **Input price** | $0.10 / MTok *(input only — embeddings have no output tokens)* |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Semantic similarity, text retrieval, RAG pipelines, clustering, classification |
| **Notable** | General-purpose text embedding model; 1024-dimension output; competitive with OpenAI text-embedding-3-small at similar price; good default for non-code embedding use cases |

---

### 🆕 Mistral Moderation *(Content Classifier)*

> **🆕 ADDED (June 8, 2026):** Mistral Moderation is now formally documented with pricing from the official `mistral.ai/pricing` page. Version 2603 (March 2026) supersedes the legacy 2411 version.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-moderation-2603` |
| **Released** | March 2026 (version 2603) |
| **Status** | ✅ Active — Specialized (Content Moderation) |
| **Input price** | $0.10 / MTok |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Text content moderation, 128K context window, jailbreaking detection, policy classification |
| **Notable** | Latest moderation model; 128K context window; jailbreaking detection; use for content safety pipelines, policy enforcement, and input/output filtering |

---

### 🆕 Leanstral *(Labs — Formal Proof Engineering)*

> **🆕 ADDED (June 8, 2026):** Leanstral is now listed on the official `mistral.ai/pricing` page as a [Labs] model. It is **free** during the feedback-collection period. First open-source code agent for Lean 4 formal proof engineering.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `labs-leanstral-2603` |
| **Released** | March 2026 (v26.03) |
| **Status** | ✅ Active — Labs (Free during feedback-collection period) |
| **Pricing** | **Free** — "Keeping this endpoint highly accessible for a limited period to gather realistic feedback and observability data" |
| **Availability** | API (Mistral AI Studio) — Labs tier |
| **Capabilities** | Lean 4 formal proof engineering, theorem proving, verified code generation |
| **Notable** | First open-source code agent for Lean 4; designed for formal verification workflows; free period enables broad experimentation; pricing will be introduced after the feedback period ends |

---

### 🆕 Mistral Small Creative *(Labs — Creative Writing)*

> **🆕 ADDED (June 8, 2026):** Mistral Small Creative is now listed on the official `mistral.ai/pricing` page as a [Labs] model at $0.10/$0.30 per MTok.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `labs-mistral-small-creative` |
| **Released** | December 2025 (v25.12) |
| **Status** | ✅ Active — Labs |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.30 / MTok |
| **Availability** | API (Mistral AI Studio) — Labs tier |
| **Capabilities** | Creative writing, roleplay, chat, story generation, dialogue writing |
| **Notable** | Fine-tuned variant of Mistral Small on curated creative data; designed to produce more expressive, engaging, and personality-rich outputs than the base Small model; same price as Devstral Small 2 and Mistral Small 4 ($0.10/$0.30) |

---

### Mistral Nemo

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `open-mistral-nemo` |
| **Status** | ✅ Active — Ultra-Budget |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.15 / MTok |
| **Context window** | 128,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Notable** | Flat input = output pricing; extremely affordable; open weights available |

---

### Ministral 3 14B

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `ministral-14b-latest` |
| **Status** | ✅ Active |
| **Input price** | $0.20 / MTok |
| **Output price** | $0.20 / MTok |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Notable** | Updated December 2025 as Ministral 3 family (v25.12); vision capabilities; best-in-class text and vision for edge |

---

### Ministral 3 8B

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `ministral-8b-latest` |
| **Status** | ✅ Active |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.15 / MTok |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Notable** | Updated December 2025 as Ministral 3 family (v25.12); vision capabilities |

---

### Ministral 3 3B

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `ministral-3b-latest` |
| **Status** | ✅ Active |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.10 / MTok |
| **Context window** | 556,032 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Notable** | Largest context window in the Ministral family; fastest model on Mistral at 266 tokens/sec (Artificial Analysis). Updated December 2025 as Ministral 3 family (v25.12); vision capabilities. |

---

### Mixtral 8x22B *(API — Legacy Open-Weight)*

> **Note (June 8, 2026):** Mixtral 8x22B remains listed on `mistral.ai/pricing` with active API pricing. While this is a legacy open-weight model (predating the Ministral/Medium/Small 4 generation), it is still API-accessible for existing integrations.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `open-mixtral-8x22b` |
| **Status** | ✅ Active (API) — Legacy open-weight |
| **Input price** | $2.00 / MTok |
| **Output price** | $6.00 / MTok |
| **Context window** | 65,536 tokens (64K) |
| **Availability** | API (Mistral AI Studio); open-weight (Apache 2.0) for self-hosting |
| **Capabilities** | Text, multilingual, general reasoning |
| **Notable** | 141B total parameters (39B active — Sparse MoE); most capable legacy Mixtral; Apache 2.0 license; available as self-hosted alternative to paying API rates |

---

### Mixtral 8x7B *(API — Legacy Open-Weight)*

> **Note (June 8, 2026):** Mixtral 8x7B remains listed on `mistral.ai/pricing` with active API pricing. Legacy model; prefer Mistral Small 4 or Ministral 3 8B for newer workloads.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `open-mixtral-8x7b` |
| **Status** | ✅ Active (API) — Legacy open-weight |
| **Input price** | $0.70 / MTok |
| **Output price** | $0.70 / MTok |
| **Context window** | 32,768 tokens (32K) |
| **Availability** | API (Mistral AI Studio); open-weight (Apache 2.0) for self-hosting |
| **Capabilities** | Text, multilingual, general tasks |
| **Notable** | 46.7B total parameters (12.9B active — Sparse MoE); Apache 2.0 license; superseded by Mistral Nemo ($0.15/$0.15, 128K ctx) and Ministral 3 8B ($0.15/$0.15, 256K ctx) — both cheaper and more capable |

---

## 🔓 Open-Weight / Self-Hosted Models

> These models are available for free self-hosting under **Apache 2.0** license (except Voxtral TTS which is CC BY-NC 4.0, Medium 3.5 and Devstral 2 which use modified MIT with a large-revenue carve-out). No API costs — only compute infrastructure.

| Model | Parameters | License | Best For |
|---|---|---|---|
| **Mistral Medium 3.5** 🆕 | 128B (dense) | Modified MIT | Self-hosted flagship: coding + reasoning + vision in one model |
| **Mistral Small 4** | 119B (MoE, 6B active) | Apache 2.0 | Self-hosted multimodal reasoning + coding |
| **Mistral Large 3 (2512)** | 675B (MoE) | Apache 2.0 | Self-hosted flagship general reasoning |
| **Devstral 2 (2512)** | 123B | Modified MIT | Self-hosted coding agents (large-revenue commercial use requires arrangement) |
| **Devstral Small 2** | 24B | Apache 2.0 | Self-hosted budget coding agent (fits on RTX 4090 / 32GB Mac) |
| **Magistral Medium 1.2** | — | Apache 2.0 | Self-hosted reasoning workloads |
| **Voxtral Small 24B** | 24B | Apache 2.0 | Self-hosted audio understanding |
| **Voxtral Mini 3B** | 3B | Apache 2.0 | Self-hosted lightweight transcription / edge ASR |
| **Voxtral TTS** | 4B | CC BY-NC 4.0 | Self-hosted TTS (non-commercial only) |
| **Mixtral 8×22B** | 141B (MoE) | Apache 2.0 | Self-hosted complex reasoning, high-throughput |
| **Mixtral 8×7B** | 46.7B (MoE) | Apache 2.0 | General-purpose self-hosted tasks |
| **Mistral 7B** | 7B | Apache 2.0 | Edge deployment, on-device, low-resource |

> **Note:** Mistral Medium 3.5 requires as few as 4× A100/H100 80GB GPUs (FP8). Q4-quantized versions require ~70GB VRAM. Devstral Small 2 requires ~14GB VRAM at Q4 (RTX 4090 / 32GB Mac). Voxtral Mini 3B fits on edge devices with quantization.

---

## ⚠️ Legacy Models

### ⚠️ LEGACY — Pixtral Large *(Deprecated — May 2026)*

> **🆕 MOVED TO LEGACY (May 28, 2026):** Pixtral Large (`pixtral-large-2411`) is no longer listed on `mistral.ai/pricing` and appears in the `docs.mistral.ai` legacy/deprecated table (version 24.11). Mistral Medium 3.5 now handles vision + coding + reasoning in a single model at $1.50/$7.50.

| Field | Value |
|---|---|
| **Model ID** | `pixtral-large-2411` |
| **Released** | November 2024 |
| **Status** | ⚠️ LEGACY — Deprecated per docs.mistral.ai (May 2026); removed from mistral.ai/pricing |
| **Last price** | $2.00 input / $6.00 output per MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Use **Mistral Medium 3.5** ($1.50/$7.50, 256K context, vision + reasoning + coding) or **Mistral Small 4** ($0.10/$0.30, vision + reasoning at budget price) |

---

### ⚠️ LEGACY — Magistral Small 1.2 / version 2509 *(Deprecated version)*

> **🆕 MOVED TO LEGACY (May 25, 2026):** `docs.mistral.ai/models/overview` lists **Magistral Small 1.2** (`magistral-small-2509`) in the **deprecated/legacy model table**. Note: the `magistral-small-latest` alias still routes to an active version at $0.50/$1.50 on the pricing page — see the Active section above. Only the specific `magistral-small-2509` version is deprecated.

| Field | Value |
|---|---|
| **Model ID** | `magistral-small-2509` *(specific version — use `magistral-small-latest` for active routing)* |
| **Released** | September 2025 (version 25.09) |
| **Status** | ⚠️ LEGACY — Specific version deprecated per docs.mistral.ai (May 25, 2026) |
| **Last price** | $0.50 input / $1.50 output per MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Use `magistral-small-latest` for active routing, **Mistral Small 4** with `reasoning_effort=high` ($0.10/$0.30, 256K context) for budget reasoning, or **Magistral Medium 1.2** ($2/$5) for dedicated reasoning |

---

### ⚠️ LEGACY — Devstral Small 1.1 *(Superseded by Devstral Small 2)*

| Field | Value |
|---|---|
| **Model ID** | `devstral-small-1-1` |
| **Released** | July 2025 |
| **Status** | ⚠️ LEGACY — Superseded by Devstral Small 2 (Dec 2025) |
| **Last price** | $0.07 input / $0.28 output per MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Upgrade to **Devstral Small 2** ($0.10/$0.30, 256K context, ~58% SWE-bench, Apache 2.0) |

---

### ⚠️ LEGACY — Devstral Medium *(July 2025)*

| Field | Value |
|---|---|
| **Model ID** | `devstral-medium` |
| **Released** | July 2025 |
| **Status** | ⚠️ LEGACY — Superseded by Devstral 2 (Dec 2025) |
| **Last price** | $0.40 input / $2.00 output per MTok |
| **Migration** | Upgrade to **Devstral 2** ($0.40/$2.00) or **Mistral Medium 3.5** ($1.50/$7.50) |

---

### ⚠️ LEGACY — Mistral Small 3.2 24B *(Superseded by Small 4)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-small-3.2` |
| **Released** | June 2025 |
| **Status** | ⚠️ LEGACY — Superseded by Mistral Small 4 (March 2026) |
| **Last price** | $0.07 input / $0.20 output per MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Upgrade to **Mistral Small 4** ($0.10/$0.30, 256K context) |

---

### ⚠️ LEGACY — Mistral Small 3.1 *(Superseded)*

| Field | Value |
|---|---|
| **Status** | ⚠️ LEGACY — Superseded by Small 3.2 and then Small 4 |
| **Last price** | $0.20 input / $0.60 output per MTok |
| **Migration** | Upgrade to **Mistral Small 4** ($0.10/M input) |

---

### ⚠️ LEGACY — Mistral Large 2 (2407)

| Field | Value |
|---|---|
| **Model ID** | `mistral-large-2407` |
| **Status** | ⚠️ LEGACY — Superseded by Large 3 |
| **Last price** | $2.00 input / $6.00 output per MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Upgrade to **Mistral Large 3 (2512)** — 256K context, 75% cheaper input, 75% cheaper output |

---

### ⚠️ LEGACY — Mistral Medium 3 (original, May 2025)

| Field | Value |
|---|---|
| **Status** | ⚠️ LEGACY — Superseded by Medium 3.1 (August 2025) and Medium 3.5 (April 2026) |
| **Last price** | $0.40 input / $2.00 output per MTok |
| **Migration** | Upgrade to **Mistral Medium 3.5** for flagship capabilities, or **Mistral Medium 3.1** if still accessible |

---

### ⚠️ LEGACY — Codestral 2501 *(Superseded by Codestral 2508)*

| Field | Value |
|---|---|
| **Status** | ⚠️ LEGACY — Superseded by Codestral 2508 (August 2025) |
| **Last price** | $1.00 input / $3.00 output per MTok |
| **Migration** | Upgrade to **Codestral 2508** ($0.30/$0.90) — 70% price reduction |

---

## 💡 Cost Optimization Notes

| Feature | Notes |
|---|---|
| **Batch API discount** | ✅ 50% off — confirmed per mistral.ai/pricing FAQ |
| **No prompt caching** | Unlike OpenAI/Anthropic, Mistral does NOT offer prompt caching discounts |
| **EU data residency** | All API traffic processed in the EU by default — no extra configuration |
| **Free tier** | Available via La Plateforme; rate-limited on mid-tier models; no credit card required |
| **Fine-tuning** | Available on Small and Medium — fine-tuned small models can match Large at 10× lower cost on narrow tasks |
| **Self-hosting** | Apache 2.0 open-weight models eliminate per-token costs; cost-effective above ~$500–1K/month API spend |
| **Model routing** | Route 60/25/15 split (Small/Medium/Large) vs all-Large to reduce costs by 70–80% |
| **Magistral vs Medium 3.5** | For most reasoning tasks, Medium 3.5 with `reasoning_effort=high` ($1.50/$7.50) replaces Magistral Medium ($2/$5) at similar or lower cost |
| **Devstral 2 vs Medium 3.5 for coding** | Devstral 2 ($0.40/$2.00) is 3.75× cheaper on input; prefer it for high-volume pure coding tasks where vision/general reasoning not needed |
| **Devstral Small 2 vs Devstral 2** | Devstral Small 2 ($0.10/$0.30) is 4× cheaper on input and ~7× cheaper on output vs Devstral 2 ($0.40/$2.00) |
| **Budget reasoning** | Use Mistral Small 4 with `reasoning_effort=high` ($0.10/$0.30) as the budget reasoning option |
| **Voxtral Mini vs Small** | Voxtral Mini ($0.001/min) is 4× cheaper than Voxtral Small ($0.004/min) for audio input; use Mini for cost-sensitive ASR, Small for higher-quality audio understanding |
| **Leanstral (Labs)** | Free during feedback-collection period — ideal for formal verification / Lean 4 proof engineering workloads while pricing is waived |

---

## 💬 Vibe / Le Chat Consumer Plans *(separate from API billing)*

| Plan | Price | Notes |
|---|---|---|
| **Free** | $0/mo | Rate-limited messages, mid-tier models, web search, image generation, Vibe CLI (limited) |
| **Pro** | $14.99/mo | More messages, extended thinking, deep research, 15GB storage, Mistral Vibe CLI, Vibe Remote Agents — **does NOT include API credits** |
| **Team** | $24.99/user/mo | Up to 30GB storage per user, domain verification, data export, collaborative workspace |
| **Education** | $5.99/mo | For verified students |
| **Enterprise** | Custom | SSO, audit logs, white label, custom models; contact sales |

> ⚠️ Vibe Pro does **not** include API access. Consumer and developer API billing are entirely separate.

---

*Sources last verified: June 8, 2026 against mistral.ai/pricing (official pricing page — all active prices confirmed unchanged; Leanstral Free, Mistral Small Creative $0.10/$0.30, OCR 3 $2/$3 per 1K pages, Codestral Embed $0.15/MTok, Mistral Embed $0.10/MTok, Mistral Moderation $0.10/MTok confirmed as new entries; Mistral Medium 3.1 NOT listed on pricing page), docs.mistral.ai/models/overview (Medium 3.1 still listed as Premier; Leanstral v26.03, Mistral Small Creative v25.12 in active section), mistral.ai/news/ (no new model announcements since June 1). Batch API discount (50%) confirmed per mistral.ai/pricing FAQ.*
