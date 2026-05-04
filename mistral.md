# 🔵 Mistral AI — Model Cards

> **Last updated:** 2026-05-04  
> **Source:** https://mistral.ai/pricing · https://mistral.ai/news/vibe-remote-agents-mistral-medium-3-5 · https://pricepertoken.com/pricing-page/provider/mistral-ai · https://artificialanalysis.ai/providers/mistral · https://openrouter.ai/mistralai  
> **Scraped / verified:** 2026-05-04  

All prices are **USD per million tokens (MTok)**. Mistral offers a **free experimentation tier** (rate-limited) — no credit card required to start. API and consumer (Le Chat) subscriptions are billed **separately**.

> **Mistral's key differentiators:** Native EU data residency (GDPR by default), cheapest output pricing in mid-tier, Apache 2.0 open-weight models for self-hosting, dedicated reasoning models (Magistral series), and now a flagship merged model (Medium 3.5).

---

## ✅ Active / Recommended Models

### 🆕 Mistral Medium 3.5 *(New Flagship — Released April 29, 2026)*

> **🆕 ADDED May 4, 2026:** Mistral released Medium 3.5 on April 29, 2026 alongside Vibe Remote Agents. It is Mistral's **first flagship merged model** — a single 128B dense model that handles instruction-following, reasoning, coding, and vision. It replaces Devstral 2 as the default model in Mistral Vibe CLI and also powers the new Work Mode in Le Chat. Pricing confirmed at $1.50/$7.50 per million tokens (from official Mistral AI blog post).

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-medium-3.5` *(check console.mistral.ai for alias routing)* |
| **Released** | April 29, 2026 |
| **Status** | ✅ Active — **New Flagship (Public Preview)** |
| **Input price** | $1.50 / MTok |
| **Output price** | $7.50 / MTok |
| **Context window** | 256,000 tokens |
| **Max output** | Not yet published |
| **Availability** | API (Mistral AI Studio / La Plateforme); NVIDIA NIM; open weights on HuggingFace (modified MIT license) |
| **Capabilities** | Text, Vision (variable image sizes/aspect ratios), Function Calling, JSON mode, Configurable reasoning effort (`reasoning_effort`: none / low / medium / high), Agentic coding, 24-language support |
| **Notable** | First Mistral flagship **merged** model — replaces Medium 3.1 + Magistral + Devstral 2 roles in a single model; 128B dense (non-MoE — all params active per pass); SWE-Bench Verified 77.6%; τ³-Telecom 91.4%; self-hostable on as few as 4× A100/H100 80GB GPUs; defaults model for Mistral Vibe CLI and Le Chat Work Mode; open weights under modified MIT license (large-revenue enterprises must negotiate commercial arrangement); 40% faster than Devstral 2 on coding tasks |

> ⚠️ **Preview pricing note:** Medium 3.5 is in public preview. Pricing ($1.50/$7.50) is confirmed from the official Mistral AI announcement. Verify on console.mistral.ai before large-scale deployment as rates may update when it reaches GA.

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

### Magistral Small 1.2 *(Reasoning Model — Budget)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `magistral-small-latest` |
| **Status** | ✅ Active — Reasoning (Budget) |
| **Input price** | $0.50 / MTok |
| **Output price** | $1.50 / MTok |
| **Context window** | 128,000 tokens *(performance degrades past ~40K — keep inputs under 40K for best results)* |
| **Availability** | API (Mistral AI Studio); open-weight (Apache 2.0) — can run locally on RTX 4090 or 32GB RAM Mac (quantized) |
| **Capabilities** | Chain-of-thought reasoning, same multilingual support as Magistral Medium |
| **Notable** | Same price as Mistral Large 3 ($0.50/$1.50) but with added chain-of-thought reasoning capability; 24B parameters; budget entry into Mistral's reasoning tier |

---

### Mistral Medium 3.1 *(Updated August 2025)*

> **Note (May 2026):** Mistral Medium 3.5 supersedes Medium 3.1 for most use cases. The `mistral-medium-latest` alias may now route to Medium 3.5. Verify your API calls land on the expected version. Medium 3.1 remains available at its lower price point for budget workloads that don't require Medium 3.5's vision, reasoning, or agentic capabilities.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-medium-3-1` *(use explicit model ID — `mistral-medium-latest` may route to Medium 3.5)* |
| **Released** | August 2025 (supersedes Medium 3, May 2025) |
| **Status** | ✅ Active — Balanced *(may be superseded in routing by Medium 3.5)* |
| **Input price** | $0.40 / MTok |
| **Output price** | $2.00 / MTok |
| **Context window** | 131,072 tokens |
| **Max output** | 8,192 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Text, Function Calling, JSON mode |
| **Notable** | Budget option vs Medium 3.5 (3.75× cheaper input, 3.75× cheaper output); use for high-volume text workloads not requiring vision or reasoning |

---

### Mistral Small 4 *(Released March 16, 2026)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-small-latest` *(alias for `mistral-small-2603`)* |
| **Released** | March 16, 2026 |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.60 / MTok |
| **Context window** | 262,144 tokens (256K) |
| **Availability** | API (Mistral AI Studio); open weights (Apache 2.0) |
| **Capabilities** | Text, Vision (multimodal input), Function Calling, Reasoning (`reasoning_effort` param), Agentic tasks, Coding |
| **Notable** | Merges three models into one: Magistral (reasoning), Pixtral (multimodal vision), Devstral (agentic coding); configurable `reasoning_effort` (none → high) per request; 119B total params, only 6B active per token (MoE 128 experts, 4 active); 40% faster than Small 3.2; cheapest multimodal reasoning model from a major provider; 5× cheaper than GPT-5.4 Mini on input |

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

> **Note (May 2026):** Devstral 2 has been replaced by **Mistral Medium 3.5** as the default model in Mistral Vibe CLI for agentic coding sessions. Devstral 2 remains available via API for teams that prefer its lighter footprint or lower cost ($0.40/$0.90 vs $1.50/$7.50 for Medium 3.5).

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `devstral-latest` *(alias for `devstral-2-2512`)* |
| **Released** | December 10, 2025 |
| **Status** | ✅ Active — Agentic Coding *(superseded in Vibe by Medium 3.5)* |
| **Input price** | $0.40 / MTok |
| **Output price** | $0.90 / MTok |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio); open-weight (Apache 2.0) |
| **Capabilities** | Advanced agentic coding, CI/CD automation, multi-file reasoning, codebase exploration |
| **Notable** | Purpose-built for autonomous coding agents; 123B parameters; open-weight; superseded in Vibe CLI by Medium 3.5 but still available for API use |

---

### Devstral Small 1.1 *(Coding Agent — Budget)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `devstral-small-latest` |
| **Released** | July 2025 |
| **Status** | ✅ Active — Agentic Coding (Budget) |
| **Input price** | $0.07 / MTok |
| **Output price** | $0.28 / MTok |
| **Context window** | 128,000 tokens |
| **Availability** | API (Mistral AI Studio); open weights (Apache 2.0) — deployable on single RTX 4090 or 32GB Mac |
| **Capabilities** | Coding agents, code generation, CI/CD automation |
| **Notable** | Ultra-affordable coding agent; 53.6% SWE-Bench Verified (top open-model at launch); open weights |

---

### Mistral Small Creative *(Experimental)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-small-creative` *(confirm exact API ID on console)* |
| **Released** | December 16, 2025 |
| **Status** | ✅ Active — Specialized (Creative Writing) |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.30 / MTok |
| **Context window** | 33,000 tokens |
| **Availability** | API (Mistral AI Studio); confirmed on OpenRouter |
| **Capabilities** | Creative writing, narrative generation, roleplay, character-driven dialogue, general instruction following, conversational agents |
| **Notable** | Experimental creative-focused model; smaller context than general-purpose models; not recommended as primary production model — use Mistral Small 4 for broad tasks |

---

### Voxtral Small 24B *(Audio / Speech)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-small-latest` |
| **Released** | October 2025 (version 2507) |
| **Status** | ✅ Active — Specialized (Audio Transcription) |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.30 / MTok |
| **Context window** | 128,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Audio processing, voice understanding, speech-to-text, audio analysis |
| **Notable** | Mistral's core audio transcription model; purpose-built for voice and speech workloads; audio priced at $100 per million seconds |

---

### Voxtral TTS *(Text-to-Speech — Released March 2026)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-tts` *(verify exact ID on console)* |
| **Released** | March 23, 2026 |
| **Status** | ✅ Active — Specialized (Text-to-Speech) |
| **Pricing** | $0.016 per 1,000 characters *(confirmed by third-party sources; verify on console.mistral.ai)* |
| **Availability** | API (Mistral AI Studio); open weights on HuggingFace (CC BY-NC 4.0 — non-commercial) |
| **Capabilities** | Multilingual TTS (9 languages: English, French, German, Spanish, Dutch, Portuguese, Italian, Hindi, Arabic), zero-shot voice cloning (3s reference), cross-lingual voice transfer, emotionally expressive voices, low-latency streaming (70ms on H200), enterprise voice agents |
| **Model size** | 4B parameters (based on Ministral 3B) |
| **Notable** | First Mistral TTS model; direct competitor to ElevenLabs; self-hostable on 16GB VRAM+ GPU |

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

### Ministral 14B

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `ministral-14b-latest` |
| **Status** | ✅ Active |
| **Input price** | $0.20 / MTok |
| **Output price** | $0.20 / MTok |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio) |

---

### Ministral 8B

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `ministral-8b-latest` |
| **Status** | ✅ Active |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.10 / MTok |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio) |

---

### Ministral 3B

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `ministral-3b-latest` |
| **Status** | ✅ Active |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.10 / MTok |
| **Context window** | 556,032 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Notable** | Largest context window in the Ministral family; fastest model on Mistral at 266 tokens/sec (Artificial Analysis) |

---

## 🔓 Open-Weight / Self-Hosted Models

> These models are available for free self-hosting under **Apache 2.0** license (except Voxtral TTS which is CC BY-NC 4.0, and Medium 3.5 which uses a modified MIT license with a large-revenue carve-out). No API costs — only compute infrastructure.

| Model | Parameters | License | Best For |
|---|---|---|---|
| **Mistral Medium 3.5** 🆕 | 128B (dense) | Modified MIT | Self-hosted flagship: coding + reasoning + vision in one model |
| **Mistral Small 4** | 119B (MoE, 6B active) | Apache 2.0 | Self-hosted multimodal reasoning + coding |
| **Mistral Large 3 (2512)** | 675B (MoE) | Apache 2.0 | Self-hosted flagship general reasoning |
| **Devstral 2 (2512)** | 123B | Apache 2.0 | Self-hosted coding agents |
| **Magistral Medium 1.2** | — | Apache 2.0 | Self-hosted reasoning workloads |
| **Magistral Small 1.2** | 24B | Apache 2.0 | Self-hosted budget reasoning (fits on RTX 4090 quantized) |
| **Mixtral 8×22B** | 141B (MoE) | Apache 2.0 | Self-hosted complex reasoning, high-throughput |
| **Mixtral 8×7B** | 46.7B (MoE) | Apache 2.0 | General-purpose self-hosted tasks |
| **Mistral 7B** | 7B | Apache 2.0 | Edge deployment, on-device, low-resource |

> **Note:** Mistral Medium 3.5 requires as few as 4× A100/H100 80GB GPUs (FP8). Q4-quantized versions require ~70GB VRAM. EAGLE speculative decoding models are available for vLLM/SGLang.

---

## ⚠️ Legacy Models

### ⚠️ LEGACY — Devstral Medium *(July 2025)*

| Field | Value |
|---|---|
| **Model ID** | `devstral-medium` |
| **Released** | July 2025 |
| **Status** | ⚠️ LEGACY — Superseded by Devstral 2 (Dec 2025) |
| **Last price** | $0.40 input / $2.00 output per MTok |
| **Migration** | Upgrade to **Devstral 2** ($0.40/$0.90 — same input, 55% cheaper output) or **Mistral Medium 3.5** ($1.50/$7.50 — for vision/reasoning/agentic) |

---

### ⚠️ LEGACY — Mistral Small 3.2 24B *(Superseded by Small 4)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-small-3.2` |
| **Released** | June 2025 |
| **Status** | ⚠️ LEGACY — Superseded by Mistral Small 4 (March 2026) |
| **Last price** | $0.07 input / $0.20 output per MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Upgrade to **Mistral Small 4** — better capabilities, larger context (256K), $0.15/$0.60; `mistral-small-latest` now routes to Small 4 |

---

### ⚠️ LEGACY — Mistral Small 3.1 *(Superseded)*

| Field | Value |
|---|---|
| **Status** | ⚠️ LEGACY — Superseded by Small 3.2 and then Small 4 |
| **Last price** | $0.20 input / $0.60 output per MTok |
| **Migration** | Upgrade to **Mistral Small 4** ($0.15/M input) |

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
| **Migration** | Upgrade to **Mistral Medium 3.5** for flagship capabilities, or **Mistral Medium 3.1** for budget text tasks |

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
| **No prompt caching** | Unlike OpenAI/Anthropic, Mistral does NOT offer prompt caching discounts |
| **No Batch API discount** | Mistral does not currently offer a batch processing discount tier |
| **EU data residency** | All API traffic processed in the EU by default — no extra configuration |
| **Free tier** | Available via La Plateforme; rate-limited on mid-tier models; no credit card required |
| **Fine-tuning** | Available on Small and Medium — fine-tuned small models can match Large at 10× lower cost on narrow tasks |
| **Self-hosting** | Apache 2.0 open-weight models eliminate per-token costs; cost-effective above ~$500–1K/month API spend |
| **Model routing** | Route 60/25/15 split (Small/Medium/Large) vs all-Large to reduce costs by 70–80% |
| **Magistral vs Medium 3.5** | For most reasoning tasks, Medium 3.5 with `reasoning_effort=high` ($1.50/$7.50) replaces Magistral Medium ($2/$5) at similar or lower cost |
| **Devstral 2 vs Medium 3.5 for coding** | Devstral 2 ($0.40/$0.90) is 3.75× cheaper on input; prefer it for high-volume pure coding tasks. Medium 3.5 adds vision + reasoning + general tasks. |

---

## 💬 Le Chat Consumer Plans *(separate from API billing)*

| Plan | Price | Notes |
|---|---|---|
| **Free** | $0/mo | Rate-limited messages, mid-tier models, web search, image generation |
| **Pro** | $14.99/mo | More messages, extended thinking, deep research, 15GB storage, Mistral Vibe CLI (powered by Medium 3.5), Vibe Remote Agents — **does NOT include API credits** |
| **Team** | $24.99/user/mo | Up to 30GB storage per user, domain verification, data export, collaborative workspace |
| **Enterprise** | Custom | SSO, audit logs, white label, custom models; contact sales |

> ⚠️ Le Chat Pro does **not** include API access. Consumer and developer API billing are entirely separate.

---

*Sources last verified: May 4, 2026 against mistral.ai/news/vibe-remote-agents-mistral-medium-3-5 (official Mistral announcement, confirmed $1.50/$7.50 pricing), mistral.ai/pricing, pricepertoken.com/pricing-page/provider/mistral-ai, artificialanalysis.ai/models/mistral-medium-3-5/providers, openrouter.ai/mistralai*
