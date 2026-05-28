# 🔵 Mistral AI — Model Cards

> **Last updated:** 2026-05-28
> **Source:** https://mistral.ai/pricing · https://docs.mistral.ai/models/overview · https://mistral.ai/news/devstral-2-vibe-cli · https://mistral.ai/news/vibe-remote-agents-mistral-medium-3-5 · https://openrouter.ai/mistralai
> **Scraped / verified:** 2026-05-28

All prices are **USD per million tokens (MTok)**. Mistral offers a **free experimentation tier** (rate-limited) — no credit card required to start. API and consumer (Vibe) subscriptions are billed **separately**.

> **Mistral's key differentiators:** Native EU data residency (GDPR by default), competitive mid-tier output pricing, Apache 2.0 open-weight models for self-hosting, dedicated reasoning models (Magistral series), flagship merged model (Medium 3.5), and a batch processing discount (50% off).

> ✅ **May 28, 2026 update:** Multiple price corrections confirmed against `mistral.ai/pricing` (verified May 28, 2026):
> - **Devstral 2 output price corrected: $0.90 → $2.00 per MTok** — the official stated price from the launch announcement (`mistral.ai/news/devstral-2-vibe-cli`: "After the free period, the API pricing will be $0.40/$2.00"). Earlier tracking reflected the free-period price; now confirmed at $2.00 output on the pricing page and OpenRouter.
> - **Pixtral Large moved to Legacy** — no longer listed on `mistral.ai/pricing`; confirmed in `docs.mistral.ai` legacy/deprecated table as `pixtral-large-2411`. Migrate to Mistral Medium 3.5 ($1.50/$7.50) for vision + coding tasks.
> - **Mistral Small 4: $0.15/$0.60 → $0.10/$0.30 per MTok** — per official `mistral.ai/pricing` page (verified May 28, 2026).
> - **Ministral 3B: $0.04/$0.04 → $0.10/$0.10 per MTok** — per official `mistral.ai/pricing` page (verified May 28, 2026).
> - **Ministral 8B: $0.10/$0.10 → $0.15/$0.15 per MTok** — per official `mistral.ai/pricing` page (verified May 28, 2026).
> - **Voxtral Small pricing updated** — audio input now priced at $0.004/min; output updated to $0.40/MTok.
> - **Batch processing discount confirmed**: Mistral now offers 50% off for batch processing (per FAQ on pricing page). Previous cards noted no batch discount.

---

## ✅ Active / Recommended Models

### 🆕 Mistral Medium 3.5 *(Flagship — Released April 29, 2026)*

> **Released April 29, 2026:** Mistral's **first flagship merged model** — a single 128B dense model handling instruction-following, reasoning, coding, and vision. It is the default model in Mistral Vibe CLI and powers the new Work Mode in Le Chat. Pricing confirmed at $1.50/$7.50 per million tokens (from official Mistral AI blog post and pricing page).

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

> **Note (May 2026):** With the release of Mistral Medium 3.5, which includes configurable reasoning effort, Magistral Medium is now redundant for most use cases. Prefer Medium 3.5 for combined reasoning + coding + vision workloads. Magistral Medium remains available as a dedicated reasoning API model. Magistral Small 1.2 has been deprecated — see Legacy section.

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

> **Price update (May 28, 2026):** Official `mistral.ai/pricing` now shows $0.10/$0.30 per MTok, down from the $0.15/$0.60 at launch. Confirmed against official pricing page (May 28, 2026). OpenRouter still reflects $0.15/$0.60 (may lag the official change). Use official API pricing as canonical.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-small-latest` *(alias for `mistral-small-2603`)* |
| **Released** | March 16, 2026 |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.10 / MTok *(updated May 28, 2026 — was $0.15)* |
| **Output price** | $0.30 / MTok *(updated May 28, 2026 — was $0.60)* |
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

> **Price correction (May 28, 2026):** Devstral 2 output price corrected to **$2.00/MTok**. The official Mistral launch announcement (`mistral.ai/news/devstral-2-vibe-cli`) stated "After the free period, the API pricing will be $0.40/$2.00 per million tokens." OpenRouter also confirms $0.40/$2.00. Previous tracking of $0.40/$0.90 reflected an incorrect inference during the free launch period. The `devstral-medium-latest` alias is now the canonical alias on the pricing page.

> **Note (May 2026):** Devstral 2 has been replaced by **Mistral Medium 3.5** as the default model in Mistral Vibe CLI for agentic coding sessions. Devstral 2 remains available via API. For smaller-scale agentic coding, consider **Devstral Small 2** ($0.10/$0.30).

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `devstral-medium-latest` *(updated alias; also `devstral-2-2512`)* |
| **Released** | December 10, 2025 |
| **Status** | ✅ Active — Agentic Coding *(superseded in Vibe by Medium 3.5)* |
| **Input price** | $0.40 / MTok |
| **Output price** | $2.00 / MTok *(corrected May 28, 2026 — was incorrectly recorded as $0.90)* |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio); open-weight (modified MIT license) |
| **Capabilities** | Advanced agentic coding, CI/CD automation, multi-file reasoning, codebase exploration |
| **Notable** | Purpose-built for autonomous coding agents; 123B parameters; SWE-bench Verified 72.2%; open-weight (modified MIT license — large-revenue enterprises should review terms); superseded in Vibe CLI by Medium 3.5 but still available for API use |

---

### Devstral Small 2 *(Released December 10, 2025)*

> **Note (May 28, 2026):** The `labs-devstral-small-2512` Labs variant is deprecated per `docs.mistral.ai`. The production `devstral-small-latest` alias remains active. Verify your model ID is not prefixed with `labs-` when calling the API.

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

> **Pricing update (May 28, 2026):** Audio input pricing structure updated to match official page: $0.004/min audio or $0.10/MTok text input; output $0.40/MTok (was $0.30/MTok).

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-small-latest` |
| **Released** | October 2025 (version 2507) |
| **Status** | ✅ Active — Specialized (Audio) |
| **Input price (audio)** | $0.004 / min |
| **Input price (text)** | $0.10 / MTok |
| **Output price** | $0.40 / MTok *(updated May 28, 2026 — was $0.30/MTok)* |
| **Context window** | 128,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Audio processing, voice understanding, speech-to-text, audio analysis, instruct use cases |
| **Notable** | Mistral's core audio instruct model; purpose-built for voice and speech workloads |

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

> **Price update (May 28, 2026):** Price updated to $0.15/$0.15 per MTok per official `mistral.ai/pricing` page (was $0.10/$0.10).

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `ministral-8b-latest` |
| **Status** | ✅ Active |
| **Input price** | $0.15 / MTok *(updated May 28, 2026 — was $0.10)* |
| **Output price** | $0.15 / MTok *(updated May 28, 2026 — was $0.10)* |
| **Context window** | 256,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Notable** | Updated December 2025 as Ministral 3 family (v25.12); vision capabilities |

---

### Ministral 3 3B

> **Price update (May 28, 2026):** Price reverted to $0.10/$0.10 per MTok per official `mistral.ai/pricing` page (was corrected to $0.04/$0.04 on May 18 based on an aipricing.guru scrape; official page now shows $0.10/$0.10 as of May 28, 2026).

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `ministral-3b-latest` |
| **Status** | ✅ Active |
| **Input price** | $0.10 / MTok *(updated May 28, 2026 — was $0.04 per May 18 correction)* |
| **Output price** | $0.10 / MTok *(updated May 28, 2026 — was $0.04)* |
| **Context window** | 556,032 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Notable** | Largest context window in the Ministral family; fastest model on Mistral at 266 tokens/sec (Artificial Analysis). Updated December 2025 as Ministral 3 family (v25.12); vision capabilities. |

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
| **Mixtral 8×22B** | 141B (MoE) | Apache 2.0 | Self-hosted complex reasoning, high-throughput |
| **Mixtral 8×7B** | 46.7B (MoE) | Apache 2.0 | General-purpose self-hosted tasks |
| **Mistral 7B** | 7B | Apache 2.0 | Edge deployment, on-device, low-resource |

> **Note:** Mistral Medium 3.5 requires as few as 4× A100/H100 80GB GPUs (FP8). Q4-quantized versions require ~70GB VRAM. Devstral Small 2 requires ~14GB VRAM at Q4 (RTX 4090 / 32GB Mac).

---

## ⚠️ Legacy Models

### ⚠️ LEGACY — Pixtral Large *(Deprecated — May 2026)*

> **🆕 MOVED TO LEGACY (May 28, 2026):** Pixtral Large (`pixtral-large-2411`) is no longer listed on `mistral.ai/pricing` and appears in the `docs.mistral.ai` legacy/deprecated table (version 24.11). Mistral Medium 3.5 now handles vision + coding + reasoning in a single model at $1.50/$7.50. For pure vision workloads, consider Mistral Small 4 ($0.10/$0.30) which also includes multimodal capabilities.

| Field | Value |
|---|---|
| **Model ID** | `pixtral-large-2411` |
| **Released** | November 2024 |
| **Status** | ⚠️ LEGACY — Deprecated per docs.mistral.ai (May 2026); removed from mistral.ai/pricing |
| **Last price** | $2.00 input / $6.00 output per MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Use **Mistral Medium 3.5** ($1.50/$7.50, 256K context, vision + reasoning + coding) or **Mistral Small 4** ($0.10/$0.30, vision + reasoning at budget price) |

---

### ⚠️ LEGACY — Magistral Small 1.2 *(Deprecated per docs.mistral.ai — May 2026)*

> **🆕 MOVED TO LEGACY (May 25, 2026):** `docs.mistral.ai/models/overview` lists **Magistral Small 1.2** (`magistral-small-2509`) in the **deprecated/legacy model table**. For budget reasoning, use **Mistral Small 4** with `reasoning_effort=high` ($0.10/$0.30) or **Magistral Medium 1.2** ($2/$5).

| Field | Value |
|---|---|
| **Model ID** | `magistral-small-2509` |
| **Released** | September 2025 (version 25.09) |
| **Status** | ⚠️ LEGACY — Deprecated per docs.mistral.ai (May 25, 2026) |
| **Last price** | $0.50 input / $1.50 output per MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Use **Mistral Small 4** with `reasoning_effort=high` ($0.10/$0.30, 256K context) for budget reasoning, or **Magistral Medium 1.2** ($2/$5) for dedicated reasoning |

---

### ⚠️ LEGACY — Mistral Small Creative *(Labs model — Deprecated)*

> **🆕 MOVED TO LEGACY (May 25, 2026):** `docs.mistral.ai/models/overview` lists **Mistral Small Creative** under the legacy/deprecated table with API ID `labs-mistral-small-creative`. The `labs-` prefix indicates this was an **experimental Labs model**, not a production model.

| Field | Value |
|---|---|
| **Model ID** | `labs-mistral-small-creative` |
| **Released** | December 16, 2025 |
| **Status** | ⚠️ LEGACY — Labs experimental model; deprecated per docs.mistral.ai (May 25, 2026) |
| **Last price** | $0.10 input / $0.30 output per MTok |
| **Context window** | 33,000 tokens |
| **Migration** | Use **Mistral Small 4** ($0.10/$0.30, 256K context) for general tasks |

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
| **Batch API discount** | ✅ 50% off — confirmed per mistral.ai/pricing FAQ (May 28, 2026). Previous cards noted no batch discount; this has been added. |
| **No prompt caching** | Unlike OpenAI/Anthropic, Mistral does NOT offer prompt caching discounts |
| **EU data residency** | All API traffic processed in the EU by default — no extra configuration |
| **Free tier** | Available via La Plateforme; rate-limited on mid-tier models; no credit card required |
| **Fine-tuning** | Available on Small and Medium — fine-tuned small models can match Large at 10× lower cost on narrow tasks |
| **Self-hosting** | Apache 2.0 open-weight models eliminate per-token costs; cost-effective above ~$500–1K/month API spend |
| **Model routing** | Route 60/25/15 split (Small/Medium/Large) vs all-Large to reduce costs by 70–80% |
| **Magistral vs Medium 3.5** | For most reasoning tasks, Medium 3.5 with `reasoning_effort=high` ($1.50/$7.50) replaces Magistral Medium ($2/$5) at similar or lower cost |
| **Devstral 2 vs Medium 3.5 for coding** | Devstral 2 ($0.40/$2.00) is 3.75× cheaper on input; prefer it for high-volume pure coding tasks where vision/general reasoning not needed. | 
| **Devstral Small 2 vs Devstral 2** | Devstral Small 2 ($0.10/$0.30) is 4× cheaper on input and ~7× cheaper on output vs Devstral 2 ($0.40/$2.00); suits high-volume or local-first coding agent workloads. |
| **Budget reasoning** | Magistral Small 1.2 is deprecated. Use Mistral Small 4 with `reasoning_effort=high` ($0.10/$0.30) as the budget reasoning option. |

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

*Sources last verified: May 28, 2026 against mistral.ai/pricing (official pricing page — Mistral Small 4 $0.10/$0.30, Ministral 3B $0.10/$0.10, Ministral 8B $0.15/$0.15, Devstral 2 $0.40/$2.00, Pixtral Large absent confirmed), docs.mistral.ai/models/overview (Pixtral Large 24.11 and Magistral Small 1.2 in legacy table confirmed), mistral.ai/news/devstral-2-vibe-cli (official pricing announcement: "$0.40/$2.00 per million tokens" for Devstral 2), OpenRouter devstral-2-2512 listing ($0.40/$2.00 per MTok confirmed). Batch API discount (50%) confirmed per mistral.ai/pricing FAQ.*
