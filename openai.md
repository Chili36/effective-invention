# 🟢 OpenAI — Model Cards

> **Last updated:** 2026-07-01
> **Source:** https://developers.openai.com/api/docs/pricing · https://openai.com/index/previewing-gpt-5-6-sol/
> **Scraped / verified:** 2026-07-01 — 🆕 **GPT-5.6 (Sol / Terra / Luna) previewed June 26, 2026** — next-generation model family in **limited preview** (~20 trusted partners, coordinated with the US government). Not yet generally available via public API. GPT-5.5 remains the current widely-available flagship. All other active prices re-confirmed unchanged against live pricing page. Independently re-verified against the live `developers.openai.com/api/docs/pricing` page on July 1, 2026 — no pricing changes detected; GPT-5.6 remains restricted-preview only, with OpenAI targeting general availability "in the coming weeks."

All prices are **USD per million tokens (MTok)** unless noted. Batch/Flex API gives a flat **50% discount** on all models. Cached input tokens get **50–90% off** depending on model.

> **Context tiers for GPT-5.5 and GPT-5.4:** Standard pricing applies for prompts **under ~270K tokens**. Long-context tier applies a surcharge for both models. For GPT-5.5, long-context pricing is **$10 input / $45 output** per MTok (full session). For GPT-5.5 Pro, long-context is **$60 input / $270 output** per MTok.

> **Service tiers:** Three processing tiers — **Priority** (highest availability + predictable latency), **Standard** (default), and **Batch/Flex** (async 24hr, 50% off). Priority tier is available for GPT-5.5, GPT-5.4, and GPT-5.4 mini.

> 📝 **July 1, 2026 update:** All active prices re-confirmed unchanged against live `developers.openai.com/api/docs/pricing`. 🆕 Added **GPT-5.6 (Sol/Terra/Luna)** as a Restricted/Preview entry — announced June 26, 2026, limited to ~20 trusted partner organizations pending a US government review process (per Executive Order issued June 2, 2026). No public API pricing tier active yet; published preview pricing documented below. GPT-5.6 introduces a new caching model (cache writes at 1.25× uncached input rate) that will apply once GA.

---

## 🔒 Restricted / Preview Models (Not Yet Generally Available)

### 🆕 GPT-5.6 — Sol / Terra / Luna *(Preview — Limited Access, announced June 26, 2026)*

> **Status:** 🔒 **RESTRICTED PREVIEW** — Available only to ~20 trusted partner organizations approved through a US government review process, following a June 2, 2026 executive order directing federal agencies to establish a benchmarking/assessment process for new frontier model releases. OpenAI states it expects to expand access to more companies "in the coming weeks" and target a broader public release by end of July 2026. **Not available via standard public API access as of July 1, 2026.**
>
> GPT-5.6 introduces a new naming system: the version number identifies the model generation, while **Sol**, **Terra**, and **Luna** identify durable capability tiers (top-tier / balanced / speed-and-cost) that can each advance on their own release cadence going forward — replacing the old flagship/mini/nano naming within a generation.

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model IDs** | `gpt-5.6-sol` · `gpt-5.6-terra` · `gpt-5.6-luna` *(preview)* |
| **Announced** | June 26, 2026 |
| **Status** | 🔒 Restricted preview — ~20 trusted partners; broader release expected by end of July 2026 |
| **Sol — Input / Output** | $5.00 / $30.00 per MTok *(same headline price as GPT-5.5)* |
| **Terra — Input / Output** | $2.50 / $15.00 per MTok |
| **Luna — Input / Output** | $1.00 / $6.00 per MTok |
| **Cache writes (GPT-5.6+)** | 1.25× the model's uncached input rate *(new caching model, replaces prior discount-on-write approach)* |
| **Cache reads (GPT-5.6+)** | 90% off uncached input rate (unchanged discount) |
| **Cache minimum life** | 30 minutes (new minimum for explicit cache breakpoints) |
| **Availability** | API + Codex, limited to approved preview partners only |
| **Also launching** | GPT-5.6 Sol on Cerebras hardware (up to ~750 tokens/sec) — planned for July 2026, targeting low-latency enterprise workloads |
| **New capabilities** | Max reasoning effort tier (Sol); new "ultra" mode using subagents for complex, long-running work; strong gains on Terminal-Bench 2.1 (coding) and GeneBench v1 (genomics/biology); OpenAI's most capable model yet for cybersecurity per its own benchmarking |
| **Safety** | Most extensive red-teaming to date (~700,000 A100e-equivalent GPU hours); layered cyber/bio misuse safeguards; released in coordination with the US government given elevated cyber capability |
| **Notable** | Sol is the flagship successor to GPT-5.5 at the same $5/$30 headline price; Terra and Luna are new mid/budget tiers replacing the previous "-mini"/"-nano" suffix convention for this generation |

> 📝 **Not yet reflected in the live OpenAI pricing page** (`developers.openai.com/api/docs/pricing`) as of July 1, 2026 — treat the prices above as preview/announcement pricing subject to change at GA. **GPT-5.5 remains the recommended flagship for general API access** until GPT-5.6 exits preview.

---

### GPT-5.4-Cyber *(Restricted — Limited Access)*

> **Status:** 🔒 RESTRICTED — Vetted security vendors and researchers only via OpenAI's Trusted Access for Cyber program.
> **Note:** No public API pricing.

---

## ✅ Active / Recommended Models

### GPT-5.5 *(Current Widely-Available Flagship — Released April 23-24, 2026)*

> **📝 July 1, 2026:** Remains the current generally-available flagship while **GPT-5.6 Sol** (see Restricted/Preview above) is limited to trusted partners. Expect GPT-5.5 to be superseded once GPT-5.6 reaches general availability (targeted by end of July 2026).

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.5` |
| **Released** | April 23, 2026 (ChatGPT/Codex) · April 24, 2026 (API) |
| **Status** | ✅ Active — **Current Widely-Available Flagship** *(GPT-5.6 Sol in restricted preview)* |
| **Input price (std ctx <~270K)** | $5.00 / MTok |
| **Input price (long ctx >~270K)** | $10.00 / MTok *(2× standard — full session)* |
| **Output price (std ctx)** | $30.00 / MTok |
| **Output price (long ctx)** | $45.00 / MTok *(1.5× standard — full session)* |
| **Cached input (std)** | $0.50 / MTok |
| **Cached input (long ctx)** | $1.00 / MTok |
| **Priority tier (input/output)** | $12.50 / $75.00 per MTok |
| **Priority cached input** | $1.25 / MTok |
| **Batch/Flex input (std)** | $2.50 / MTok |
| **Batch/Flex input (long)** | $5.00 / MTok |
| **Batch/Flex output (std)** | $15.00 / MTok |
| **Batch/Flex output (long)** | $22.50 / MTok |
| **Batch/Flex cached input (std)** | $0.25 / MTok |
| **Context window** | 1,050,000 tokens |
| **Max output** | 128,000 tokens |
| **Availability** | API (Responses + Chat Completions) · ChatGPT Plus/Pro/Business/Enterprise · Codex |
| **Regional processing** | +10% uplift |
| **Notable** | First fully retrained base since GPT-4.5; natively omnimodal (text+image+audio+video); top Artificial Analysis Intelligence Index; successor **GPT-5.6 Sol** in restricted preview at the same headline price |

---

### GPT-5.5 Pro

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.5-pro` |
| **Status** | ✅ Active — Ultra-Premium |
| **Input price (std)** | $30.00 / MTok |
| **Input price (long ctx)** | $60.00 / MTok |
| **Output price (std)** | $180.00 / MTok |
| **Output price (long ctx)** | $270.00 / MTok |
| **Batch/Flex input (std)** | $15.00 / MTok |
| **Batch/Flex output (std)** | $90.00 / MTok |
| **Context window** | 1,000,000 tokens |
| **Availability** | API · ChatGPT Pro/Business/Enterprise only |
| **Regional processing** | +10% uplift |
| **Notable** | Extra parallel test-time compute; deep research, legal, financial, scientific workloads |

---

### GPT-5.4 *(released March 5, 2026)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4` |
| **Status** | ✅ Active — Previous Flagship |
| **Input price (short ctx <~270K)** | $2.50 / MTok |
| **Cached input (short)** | $0.25 / MTok |
| **Output price (short ctx)** | $15.00 / MTok |
| **Input price (long ctx >~270K)** | $5.00 / MTok |
| **Cached input (long)** | $0.50 / MTok |
| **Output price (long ctx)** | $22.50 / MTok |
| **Priority input/output** | $5.00 / $30.00 per MTok |
| **Priority cached input** | $0.50 / MTok |
| **Batch input (std)** | $1.25 / MTok |
| **Batch input (long)** | $2.50 / MTok |
| **Batch output (std)** | $7.50 / MTok |
| **Batch output (long)** | $11.25 / MTok |
| **Context window** | 1,050,000 tokens |
| **Availability** | API |
| **Regional processing** | +10% uplift |
| **Notable** | Still recommended for cost-sensitive workloads vs GPT-5.5; multimodal (text + image); computer-use capabilities |

---

### GPT-5.4 Pro

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4-pro` |
| **Status** | ✅ Active *(superseded by GPT-5.5 Pro at same standard price)* |
| **Input price (std)** | $30.00 / MTok |
| **Input price (long ctx)** | $60.00 / MTok |
| **Output price (std)** | $180.00 / MTok |
| **Output price (long ctx)** | $270.00 / MTok |
| **Batch/Flex input (std)** | $15.00 / MTok |
| **Batch/Flex output (std)** | $90.00 / MTok |
| **Batch/Flex input (long)** | $30.00 / MTok |
| **Batch/Flex output (long)** | $135.00 / MTok |
| **Context window** | 1,050,000 tokens |
| **Regional processing** | +10% uplift |

---

### GPT-5.4 mini *(released March 17, 2026)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4-mini` |
| **Status** | ✅ Active — Mid-Tier |
| **Input price** | $0.75 / MTok |
| **Cached input** | $0.075 / MTok |
| **Output price** | $4.50 / MTok |
| **Priority input/output** | $1.50 / $9.00 per MTok |
| **Priority cached input** | $0.15 / MTok |
| **Batch input** | $0.375 / MTok |
| **Batch output** | $2.25 / MTok |
| **Context window** | 400,000 tokens |
| **Availability** | API · ChatGPT Free/Go via Thinking |
| **Regional processing** | +10% uplift |
| **Notable** | ~90% of flagship quality at ~6× lower cost vs GPT-5.4; most competitive mid-tier model |

---

### GPT-5.4 nano *(released March 17, 2026)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-5.4-nano` |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.20 / MTok |
| **Cached input** | $0.020 / MTok |
| **Output price** | $1.25 / MTok |
| **Batch input** | $0.10 / MTok |
| **Batch output** | $0.625 / MTok |
| **Context window** | 400,000 tokens |
| **Regional processing** | +10% uplift |
| **Notable** | Cheapest proprietary model in GPT-5.4 family; ideal for classification, extraction |

---

### GPT-4.1

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4.1` |
| **Status** | ✅ Active — Recommended for long-context workloads |
| **Input price** | $2.00 / MTok |
| **Cached input** | $0.50 / MTok |
| **Output price** | $8.00 / MTok |
| **Batch input** | $1.00 / MTok |
| **Batch output** | $4.00 / MTok |
| **Context window** | 1,040,000 tokens |
| **Notable** | 1M context at lower cost than GPT-5.4; better instruction-following and coding vs GPT-4o |

---

### GPT-4.1 mini

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4.1-mini` |
| **Status** | ✅ Active — Balanced, Long-Context Budget |
| **Input price** | $0.40 / MTok |
| **Cached input** | $0.10 / MTok |
| **Output price** | $1.60 / MTok |
| **Context window** | 1,000,000 tokens |

---

### GPT-4.1 nano

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `gpt-4.1-nano` |
| **Status** | ✅ Active — Budget long-context |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.40 / MTok |
| **Context window** | 1,000,000+ tokens |

---

### o3 *(Reasoning model)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `o3` |
| **Status** | ✅ Active — Reasoning Flagship |
| **Input price** | $2.00 / MTok |
| **Cached input** | $0.50 / MTok |
| **Output price** | $8.00 / MTok |
| **Context window** | 200,000 tokens |
| **Notable** | Chain-of-thought reasoning; best for math, logic, multi-step coding |

---

### o3-pro *(Reasoning model — Maximum Depth)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `o3-pro` |
| **Status** | ✅ Active — Maximum Reasoning |
| **Input price** | $20.00 / MTok |
| **Output price** | $80.00 / MTok |
| **Context window** | 200,000 tokens |

---

### o4-mini *(Reasoning model)*

| Field | Value |
|---|---|
| **Provider** | OpenAI |
| **Model ID** | `o4-mini` |
| **Status** | ✅ Active — Budget Reasoning |
| **Input price** | $1.10 / MTok |
| **Cached input** | $0.275 / MTok |
| **Output price** | $4.40 / MTok |
| **Context window** | 200,000 tokens |

---

## 🎙️ Multimodal, Realtime & Specialized Models

### GPT-Realtime-2 *(Latest Realtime Model)*

> **Status:** ✅ Active — Latest realtime voice interaction model. Supports audio, text, and image inputs.

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $32.00 / MTok | $0.40 / MTok | $64.00 / MTok |
| **Text** | $4.00 / MTok | $0.40 / MTok | $24.00 / MTok |
| **Image** | $5.00 / MTok | $0.50 / MTok | — |

---

### GPT-Realtime-Translate *(Live Translation)*

> **Status:** ✅ Active — Live translation model; translates speech in real time at speaker pace.

| Pricing | Value |
|---|---|
| **Price** | $0.034 / minute |

---

### GPT-Realtime-Whisper *(Real-time Speech Recognition)*

> **Status:** ✅ Active — Real-time Whisper-based speech recognition model.

| Pricing | Value |
|---|---|
| **Price** | $0.017 / minute |

---

### GPT-Image-2 *(Latest Image Generation)*

> **Status:** ✅ Active — State-of-the-art image generation model. **Recommended migration target from deprecated image models.**

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Image** | $8.00 / MTok | $2.00 / MTok | $30.00 / MTok |
| **Text** | $5.00 / MTok | $1.25 / MTok | — |

> Batch pricing: Image input $4.00, cached $1.00, output $15.00 per MTok.

---

### ⚠️ GPT-Image-1.5 *(DEPRECATED — Shutdown Dec 1, 2026)*

> **Status:** ⚠️ DEPRECATED — OpenAI notified developers June 2, 2026 of deprecation and removal December 1, 2026. **Migrate to `gpt-image-2`.**

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Image** | $8.00 / MTok | $2.00 / MTok | $32.00 / MTok |
| **Text** | $5.00 / MTok | $1.25 / MTok | $10.00 / MTok |

---

### ⚠️ GPT-Image-1-mini *(DEPRECATED — Shutdown Dec 1, 2026)*

> **Status:** ⚠️ DEPRECATED — OpenAI notified developers June 2, 2026 of deprecation and removal December 1, 2026. **Migrate to `gpt-image-2`.**

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Image** | $2.50 / MTok | $0.25 / MTok | $8.00 / MTok |
| **Text** | $2.00 / MTok | $0.20 / MTok | — |

---

### Sora-2 *(Video Generation)*

> **Status:** ✅ Active — Video generation at 720p.

| Size | Price per second |
|---|---|
| 720p | $0.10 / second *(standard)* · $0.05 / second *(batch)* |

### Sora-2-Pro *(Video Generation — High Resolution)*

| Size | Price per second (standard) |
|---|---|
| 720p | $0.30 |
| 1024p | $0.50 |
| 1080p | $0.70 |

> Batch: 50% off all sizes.

---

### Transcription Models

| Model | Input | Output | Est. Cost |
|---|---|---|---|
| `gpt-4o-transcribe` | $2.50 / MTok | $10.00 / MTok | ~$0.006 / min |
| `gpt-4o-mini-transcribe` | $1.25 / MTok | $5.00 / MTok | ~$0.003 / min |

---

### Deep Research Models

| Model | Input | Output |
|---|---|---|
| `o3-deep-research` | $5.00 / MTok | $20.00 / MTok |
| `o4-mini-deep-research` | $1.00 / MTok | $4.00 / MTok |

---

### Computer Use

| Model | Input | Output |
|---|---|---|
| `computer-use-preview` | $1.50 / MTok | $6.00 / MTok |

---

### Codex / Specialized

| Model | Input (std) | Cached Input | Priority Input | Output (std) | Priority Output |
|---|---|---|---|---|---|
| `gpt-5.3-codex` | $1.75 / MTok | $0.175 / MTok | $3.50 / MTok | $14.00 / MTok | $28.00 / MTok |
| `chat-latest` (ChatGPT API) | $5.00 / MTok | $0.50 / MTok | — | $30.00 / MTok | — |

---

## 🔧 Tools Pricing

| Tool | Details | Pricing |
|---|---|---|
| **Web search** (all models) | All models incl. Image Web search | $10.00 / 1K calls + search content tokens at model rates |
| **Web search preview** (reasoning models) | `gpt-5`, `o-series` | $10.00 / 1K calls + search content tokens at model rates |
| **Web search preview** (non-reasoning) | Non-reasoning models (non-preview) | $25.00 / 1K calls; search content tokens free |
| **Containers** | Hosted Shell + Code Interpreter | $0.03 per 1GB / $1.92 per 64GB per 20-min session |
| **File search storage** | Vector store | $0.10 / GB per day (1 GB free) |
| **File search tool call** | Responses API | $2.50 / 1K calls |
| **Agent Kit** | ChatKit file/image storage | $0.10 / GB-day after 1 GB free |

---

## ⚠️ Legacy / Deprecated / Retired Models

### ⚠️ LEGACY — GPT-Realtime-1.5 *(Removed from pricing page June 2026)*

> **Status:** ⚠️ LEGACY — No longer listed on the live OpenAI pricing page (removed as of June 2026). Superseded by `gpt-realtime-2`. Last known pricing below.

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $32.00 / MTok *(last known)* | $0.40 / MTok | $64.00 / MTok |
| **Text** | $4.00 / MTok | $0.40 / MTok | $16.00 / MTok |
| **Image** | $5.00 / MTok | $0.50 / MTok | — |

> **Migration:** → `gpt-realtime-2`

---

### ⚠️ LEGACY — GPT-Realtime-Mini *(Removed from pricing page June 2026)*

> **Status:** ⚠️ LEGACY — No longer listed on the live OpenAI pricing page (removed as of June 2026). Last known pricing below.

| Modality | Input | Cached Input | Output |
|---|---|---|---|
| **Audio** | $10.00 / MTok *(last known)* | $0.30 / MTok | $20.00 / MTok |
| **Text** | $0.60 / MTok | $0.06 / MTok | $2.40 / MTok |
| **Image** | $0.80 / MTok | $0.08 / MTok | — |

> **Migration:** → `gpt-realtime-2`

---

### ⚠️ DEPRECATED — chatgpt-image-latest *(Shutdown Dec 1, 2026)*

| Field | Value |
|---|---|
| **Model ID** | `chatgpt-image-latest` |
| **Status** | ⚠️ DEPRECATED — Notified June 2, 2026; shutdown December 1, 2026 |
| **Migration** | → **`gpt-image-2`** |

---

### ⚠️ LEGACY — GPT-5.3 / Codex *(being phased out)*

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.3` / `gpt-5.3-codex` |
| **Status** | ⚠️ LEGACY — Still available as `gpt-5.3-codex` specialized model; base GPT-5.3 phasing out Jun 2026 |
| **Input price** | $1.75 / MTok (standard) · $3.50 / MTok (priority) |
| **Output price** | $14.00 / MTok (standard) · $28.00 / MTok (priority) |
| **Migration** | → **GPT-5.5** or **GPT-5.4** |

---

### ⚠️ LEGACY — GPT-5.2

| Field | Value |
|---|---|
| **Model ID** | `gpt-5.2` |
| **Status** | ⚠️ LEGACY — **All GPT-5.2 models retired from ChatGPT June 12, 2026 ❌** · GPT-5.2 Thinking variant RETIRED API June 5, 2026 |
| **Input price** | $1.75 / MTok |
| **Output price** | $14.00 / MTok |
| **Migration** | → **GPT-5.4** ($2.50/$15) or **GPT-5.5** ($5/$30) |

---

### ⚠️ LEGACY — GPT-5.1 *(RETIRED March 11, 2026)*

| Field | Value |
|---|---|
| **Model IDs** | `gpt-5.1`, `gpt-5.1-instant`, `gpt-5.1-thinking`, `gpt-5.1-pro` |
| **Status** | ⚠️ LEGACY — **RETIRED March 11, 2026** |
| **Migration** | → **GPT-5.5** family |

---

### ⚠️ LEGACY — GPT-4o

| Field | Value |
|---|---|
| **Model ID** | `gpt-4o` |
| **Status** | ⚠️ LEGACY — Superseded by GPT-4.1 |
| **Input price** | $2.50 / MTok |
| **Output price** | $10.00 / MTok |
| **Migration** | → **GPT-4.1** ($2/$8, 1M context) |

---

### ⚠️ LEGACY — GPT-4o mini

| Field | Value |
|---|---|
| **Model ID** | `gpt-4o-mini` |
| **Status** | ⚠️ LEGACY |
| **Input price** | $0.15 / MTok |
| **Output price** | $0.60 / MTok |
| **Migration** | → **GPT-5.4 nano** ($0.20/$1.25) or **GPT-4.1 nano** ($0.10/$0.40) |

---

### ⚠️ LEGACY — o1 *(Deep Reasoning)*

| Field | Value |
|---|---|
| **Model ID** | `o1` |
| **Status** | ⚠️ LEGACY — Very expensive, limited use cases |
| **Input price** | $15.00 / MTok |
| **Output price** | $60.00 / MTok |
| **Migration** | → **o3** ($2/$8) or **o3-pro** ($20/$80) |

---

### ⚠️ LEGACY — GPT-4 Turbo / GPT-3.5 Turbo *(RETIRED)*

| Model | Status |
|---|---|
| GPT-4 Turbo | ⚠️ RETIRED |
| GPT-3.5 Turbo | ⚠️ RETIRED |

---

## 💡 Cost Optimization Notes

| Feature | Savings |
|---|---|
| **Batch/Flex API** | 50% off all tokens (24 hr turnaround) |
| **Cached input tokens** | 50–90% off depending on model |
| **GPT-5.5 long-context** | Stay under ~270K input tokens to avoid 2× input / 1.5× output surcharge |
| **GPT-5.5 vs GPT-5.4 routing** | GPT-5.5 at $5/$30 is 2× the per-token cost of GPT-5.4 $2.50/$15 |
| **Regional processing** | +10% uplift for GPT-5.5/5.4 family data residency endpoints |
| **Fine-tuning platform** | OpenAI is winding down the fine-tuning platform — no longer accessible to new users |
| **Image models** | Migrate from `gpt-image-1.5` and `gpt-image-1-mini` to `gpt-image-2` before Dec 1, 2026 |
| **Realtime models** | Use `gpt-realtime-2` ($32/$64 audio); `gpt-realtime-whisper` ($0.017/min) for transcription only |
| **🆕 GPT-5.6 preview** | Restricted to ~20 trusted partners as of July 1, 2026; not yet available for general API access — stay on GPT-5.5 until GA (targeted end of July 2026) |

---

*Sources last verified: July 1, 2026 against `developers.openai.com/api/docs/pricing` and `openai.com/index/previewing-gpt-5-6-sol/` — GPT-5.5 $5/$30, GPT-5.4 $2.50/$15, o3 $2/$8, o4-mini $1.10/$4.40, GPT-4.1 $2/$8, GPT-4.1 mini $0.40/$1.60, GPT-4.1 nano $0.10/$0.40 all confirmed unchanged. 🆕 GPT-5.6 Sol/Terra/Luna added as restricted preview ($5/$30, $2.50/$15, $1/$6) — limited to ~20 partners pending US government review, targeting broader release by end of July 2026. Independently re-verified July 1, 2026 directly against the live OpenAI pricing page — every price point above matches exactly, no changes detected.*
