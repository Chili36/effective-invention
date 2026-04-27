# 🔵 Mistral AI — Model Cards

> **Last updated:** 2026-04-27  
> **Source:** https://mistral.ai/pricing · https://pricepertoken.com/pricing-page/provider/mistral-ai (updated Apr 23, 2026) · https://openrouter.ai/mistralai · https://margindash.com/mistral-api-pricing · https://artificialanalysis.ai/providers/mistral  
> **Scraped / verified:** 2026-04-27  

All prices are **USD per million tokens (MTok)**. Mistral offers a **free experimentation tier** (rate-limited) — no credit card required to start. API and consumer (Le Chat) subscriptions are billed **separately**.

> **Mistral's key differentiators:** Native EU data residency (GDPR by default), cheapest output pricing in mid-tier, Apache 2.0 open-weight models for self-hosting, dedicated reasoning models (Magistral series).

> ⚠️ **Pricing note — Mistral Large 3:** Some January–February 2026 sources list Large 3 at $2.00/$6.00. More recent provider listings (pricepertoken.com, Apr 23 2026; margindash.com Apr 2026; artificialanalysis.ai) list `mistral-large-3-2512` at **$0.50/$1.50**, suggesting a significant price cut for the December 2025 release. The cards below reflect the $0.50/$1.50 rate; verify on the official Mistral console before large-scale deployment.

---

## ✅ Active / Recommended Models

### Mistral Large 3 (2512)

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-large-latest` |
| **Released** | December 1, 2025 (version 2512) |
| **Status** | ✅ Active — Flagship |
| **Input price** | $0.50 / MTok |
| **Output price** | $1.50 / MTok |
| **Context window** | 262,144 tokens (256K) |
| **Max output** | 8,192 tokens |
| **Availability** | API (Mistral AI Studio / La Plateforme), Azure AI Foundry |
| **Capabilities** | Text, Vision, Function Calling, JSON mode |
| **Rate limits** | Paid tier; contact Mistral for enterprise limits |
| **Notable** | Exceptionally cheap output pricing vs peers; GDPR-compliant EU hosting by default; 256K context window; open-weight under Apache 2.0 |

---

### Magistral Medium 1.2 *(Reasoning Model)*

> **Added Apr 25, 2026:** Magistral is Mistral's reasoning model line, comparable to OpenAI's o-series. Uses chain-of-thought to work through complex problems. Note: reasoning generates more output tokens per request — actual per-request costs run higher than a simple token-count estimate.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `magistral-medium-latest` *(or `magistral-medium-2509`)* |
| **Released** | September 17, 2025 (version 2509) |
| **Status** | ✅ Active — Reasoning (Enterprise) |
| **Input price** | $2.00 / MTok |
| **Output price** | $5.00 / MTok |
| **Context window** | 128,000 tokens *(performance degrades past ~40K — keep inputs under 40K for best results)* |
| **Max output** | 40,000 tokens |
| **Availability** | API (Mistral AI Studio) — open-weight (Apache 2.0) |
| **Capabilities** | Chain-of-thought reasoning, multilingual reasoning (20+ languages), complex problem-solving, multi-step logic, vision |
| **Notable** | Mistral's most capable reasoning model; transparent reasoning traces; multilingual chain-of-thought; open-weight deployment possible |

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

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-medium-latest` |
| **Released** | August 2025 (supersedes Medium 3, May 2025) |
| **Status** | ✅ Active — Balanced |
| **Input price** | $0.40 / MTok |
| **Output price** | $2.00 / MTok |
| **Context window** | 131,072 tokens |
| **Max output** | 8,192 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Text, Function Calling, JSON mode |
| **Notable** | Updated August 2025 release of the Medium tier; balanced cost and capability for chat, summarization, and code review |

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
| **Notable** | Purpose-built code model; 70% cheaper than previous Codestral 2501 ($1.00/$3.00); powers Mistral Vibe coding agent; largest context window in the Codestral family |

---

### Devstral 2 (2512) *(Coding Agent)*

> **✏️ CORRECTION (Apr 27, 2026):** Output price updated to **$0.90/MTok** (was incorrectly listed as $2.00). pricepertoken.com (updated Apr 23, 2026) and Artificial Analysis confirm $0.40/$0.90 for the Dec 2025 version (`devstral-2-2512`). Context window also corrected from 128K to **256K** per Artificial Analysis. The $2.00 output price was carried over from the legacy Devstral Medium (Jul 2025 — now superseded). Verify on console.mistral.ai before large-scale deployment.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `devstral-latest` *(alias for `devstral-2-2512`)* |
| **Released** | December 10, 2025 |
| **Status** | ✅ Active — Agentic Coding (Flagship) |
| **Input price** | $0.40 / MTok |
| **Output price** | $0.90 / MTok *(✏️ corrected from $2.00 — see note above)* |
| **Context window** | 256,000 tokens *(✏️ corrected from 128K)* |
| **Availability** | API (Mistral AI Studio); open-weight (Apache 2.0) |
| **Capabilities** | Advanced agentic coding, CI/CD automation, multi-file reasoning, codebase exploration |
| **Notable** | Purpose-built for autonomous coding agents; 123B parameters; open-weight; Devstral Small 2 (24B) released alongside for budget deployments |

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

> **Added Apr 27, 2026:** Experimental model confirmed on OpenRouter (released Dec 16, 2025). Designed specifically for creative and narrative use cases — not a general-purpose production model. Verify availability and pricing on console.mistral.ai.

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
| **Notable** | Experimental creative-focused model; smaller context than general-purpose models; not recommended as primary production model — use Mistral Small 4 for general tasks |

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

> **Added Apr 16, 2026:** Voxtral TTS was released March 23, 2026. Built on Ministral 3B. Open weights available under CC BY-NC 4.0 (non-commercial); commercial API use available. Pricing per API call TBD — verify on the official Mistral console.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-tts` *(verify exact ID on console)* |
| **Released** | March 23, 2026 |
| **Status** | ✅ Active — Specialized (Text-to-Speech) |
| **Pricing** | ⚠️ TBD — Not yet published in standard per-MTok format. Check console.mistral.ai |
| **Availability** | API (Mistral AI Studio); open weights on HuggingFace (CC BY-NC 4.0 — non-commercial) |
| **Capabilities** | Multilingual TTS (9 languages), zero-shot voice cloning (3s reference), cross-lingual voice transfer, emotionally expressive voices, low-latency streaming (70ms on H200), enterprise voice agents |
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

> These models are available for free self-hosting under **Apache 2.0** license (except Voxtral TTS which is CC BY-NC 4.0). No API costs — only compute infrastructure.

| Model | Parameters | License | Best For |
|---|---|---|---|
| **Mistral Small 4** | 119B (MoE, 6B active) | Apache 2.0 | Self-hosted multimodal reasoning + coding |
| **Mistral Large 3 (2512)** | 675B (MoE) | Apache 2.0 | Self-hosted flagship general reasoning |
| **Devstral 2 (2512)** | 123B | Apache 2.0 | Self-hosted coding agents |
| **Magistral Medium 1.2** | — | Apache 2.0 | Self-hosted reasoning workloads |
| **Magistral Small 1.2** | 24B | Apache 2.0 | Self-hosted budget reasoning (fits on RTX 4090 quantized) |
| **Mixtral 8×22B** | 141B (MoE) | Apache 2.0 | Self-hosted complex reasoning, high-throughput |
| **Mixtral 8×7B** | 46.7B (MoE) | Apache 2.0 | General-purpose self-hosted tasks |
| **Mistral 7B** | 7B | Apache 2.0 | Edge deployment, on-device, low-resource |

> **Note:** Open-weight models do not receive commercial support and may lag behind API models in capability. Mixtral 8×7B on a single A100 GPU can compete with API costs above ~$500–1,000/month.

---

## ⚠️ Legacy Models

### ⚠️ LEGACY — Devstral Medium *(July 2025)*

| Field | Value |
|---|---|
| **Model ID** | `devstral-medium` |
| **Released** | July 2025 |
| **Status** | ⚠️ LEGACY — Superseded by Devstral 2 (Dec 2025) |
| **Last price** | $0.40 input / $2.00 output per MTok |
| **Migration** | Upgrade to **Devstral 2** ($0.40/$0.90 — same input, 55% cheaper output) |

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
| **Status** | ⚠️ LEGACY — Superseded by Medium 3.1 (August 2025) |
| **Last price** | $0.40 input / $2.00 output per MTok |
| **Migration** | Upgrade to **Mistral Medium 3.1** |

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
| **Magistral vs GPT o-series** | Magistral Medium ($2/$5) is priced similarly to o3 ($2/$8) but with cheaper output; good for output-heavy reasoning |
| **Devstral 2 vs Devstral Medium** | Devstral 2 is 55% cheaper on output ($0.90 vs $2.00) and has 2× the context (256K vs 128K) — always prefer Devstral 2 |

---

## 💬 Le Chat Consumer Plans *(separate from API billing)*

| Plan | Price | Notes |
|---|---|---|
| **Free** | $0/mo | Rate-limited messages, mid-tier models, web search, image generation |
| **Pro** | $14.99/mo | More messages, extended thinking, deep research, 15GB storage, Mistral Vibe CLI — **does NOT include API credits** |
| **Team** | $24.99/user/mo | Up to 30GB storage per user, domain verification, data export, collaborative workspace |
| **Enterprise** | Custom | SSO, audit logs, white label, custom models; contact sales |

> ⚠️ Le Chat Pro does **not** include API access. Consumer and developer API billing are entirely separate. Team plan confirmed at $24.99/user/month on mistral.ai/pricing.

---

*Sources last verified: April 27, 2026 against mistral.ai/pricing, pricepertoken.com/pricing-page/provider/mistral-ai (updated Apr 23, 2026), openrouter.ai/mistralai, openrouter.ai/provider/mistral, margindash.com/mistral-api-pricing, artificialanalysis.ai/providers/mistral*
