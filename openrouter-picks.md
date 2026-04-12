# 🟣 OpenRouter Picks — Tier 2 Model Cards

> **Last updated:** 2026-04-12  
> **Source:** https://openrouter.ai/models · https://openrouter.ai (individual model pages) · Chatbot Arena leaderboard · real-usage rankings  
> **Scraped / verified:** 2026-04-12  

Tier 2 models are tracked via **OpenRouter** (openrouter.ai) — one best-performing model per provider. All prices are **OpenRouter prices** (USD per million tokens), which are typically at or near direct provider API rates.

> 💡 OpenRouter is a unified API gateway with 300+ models, OpenAI-compatible API, and per-token billing. No monthly fees. Free models available with rate limits (20 req/min, 200 req/day).

---

## OpenAI Open-Weight — `gpt-oss-120b`

| Field | Value |
|---|---|
| **Provider** | OpenAI (open-weight) |
| **Model ID (OpenRouter)** | `openai/gpt-oss-120b` |
| **Released** | August 5, 2025 |
| **Status** | ✅ Active |
| **Input price (OpenRouter)** | $0.039 / MTok |
| **Output price (OpenRouter)** | $0.19 / MTok |
| **Free tier** | Available (`openai/gpt-oss-120b:free`) — rate limited |
| **Context window** | 131,072 tokens |
| **Architecture** | 117B parameter Mixture-of-Experts (MoE); 5.1B active params per pass; optimized for single H100 GPU |
| **License** | Apache 2.0 (open weights, commercial use, fine-tuning allowed) |
| **Availability** | OpenRouter, Fireworks AI, Cerebras, Together AI, local deployment (Ollama, LM Studio) |
| **Notable** | Configurable reasoning depth; full chain-of-thought access; native tool use, function calling, structured output; 94.2% MMLU, 96.6% AIME |
| **Direct API** | Not available via direct OpenAI API — open-weight model only |

---

## DeepSeek — `deepseek/deepseek-v3.2`

| Field | Value |
|---|---|
| **Provider** | DeepSeek |
| **Model ID (OpenRouter)** | `deepseek/deepseek-v3.2` |
| **Released** | 2026 |
| **Status** | ✅ Active — Best value frontier model |
| **Input price (OpenRouter)** | $0.26 / MTok |
| **Output price (OpenRouter)** | $0.38 / MTok |
| **Context window** | 163,840 tokens |
| **Architecture** | Large MoE with DeepSeek Sparse Attention (DSA); scalable RL post-training |
| **Availability** | OpenRouter, direct API (api.deepseek.com) |
| **Notable** | GPT-5 class performance per benchmarks; gold medal on 2025 IMO and IOI; agentic tool-use; optional reasoning mode (toggle via API) |
| **Direct API note** | Direct API (api.deepseek.com): input $0.28/MTok, output $0.42/MTok. OpenRouter is slightly cheaper and adds global reliability layer. DeepSeek V4 also available ($0.30/$0.50 direct) — minor performance upgrade |

---

## Qwen (Alibaba) — `qwen/qwen3.6-plus`

| Field | Value |
|---|---|
| **Provider** | Alibaba Qwen |
| **Model ID (OpenRouter)** | `qwen/qwen3.6-plus` (paid) · `qwen/qwen3.6-plus:free` (free preview) |
| **Released** | April 2, 2026 |
| **Status** | ✅ Active — Current Top Qwen Model |
| **Input price (OpenRouter)** | **TBD** (free preview launched April 2, 2026; paid pricing not yet published — Qwen3.5 Plus was $0.26/MTok input) |
| **Output price (OpenRouter)** | **TBD** (Qwen3.5 Plus comparable: $1.56/MTok output) |
| **Context window** | 1,000,000 tokens |
| **Architecture** | Hybrid linear attention + sparse MoE; strong scalability |
| **Availability** | OpenRouter |
| **Notable** | #1 ranked for coding on OpenRouter (April 2026); 78.8% SWE-bench Verified; major gains over 3.5 in agentic coding, vibe coding, 3D scene generation; 400M+ completion tokens in first 2 days |
| **Data note** | The free preview collects prompt and completion data for model improvement — review Alibaba Qwen license for commercial use restrictions |

> 📝 **Pricing note:** Qwen3.6 Plus free preview ran from April 2–7, 2026. Paid pricing for the non-preview `qwen/qwen3.6-plus` model is TBD. If unavailable or not yet priced, use **Qwen3.5 Plus** (`qwen/qwen3.5-plus-02-15`) at $0.26/$1.56 per MTok with 1M context as a fallback.

---

## Nvidia — `nvidia/nemotron-3-super-120b-a12b`

| Field | Value |
|---|---|
| **Provider** | NVIDIA |
| **Model ID (OpenRouter)** | `nvidia/nemotron-3-super-120b-a12b` |
| **Released** | March 11, 2026 |
| **Status** | ✅ Active |
| **Input price (OpenRouter)** | $0.10 / MTok |
| **Output price (OpenRouter)** | $0.50 / MTok |
| **Free tier** | Available (`nvidia/nemotron-3-super-120b-a12b:free`) |
| **Context window** | 262,144 tokens (extended 1M token support for long-context tasks) |
| **Architecture** | 120B parameter hybrid Mamba-Transformer MoE; 12B active params; multi-token prediction (MTP) |
| **License** | NVIDIA Open License (open weights, datasets, recipes) |
| **Availability** | OpenRouter, NVIDIA NIM microservices, vLLM/SGLang/Ollama self-hosting |
| **Notable** | 50%+ higher token throughput vs other open models; leading results on AIME 2025, TerminalBench, SWE-Bench Verified; multi-agent and long-context coherence; Latent MoE (4 experts at cost of 1) |
| **Direct API** | NVIDIA NIM (nim.nvidia.com) — pricing may differ |

---

## MiniMax — `minimax/minimax-m2.7`

| Field | Value |
|---|---|
| **Provider** | MiniMax |
| **Model ID (OpenRouter)** | `minimax/minimax-m2.7` |
| **Released** | March 2026 |
| **Status** | ✅ Active — Current Flagship |
| **Input price (OpenRouter)** | $0.30 / MTok |
| **Output price (OpenRouter)** | $1.20 / MTok |
| **Context window** | 204,800 tokens |
| **Architecture** | 705B parameter model; multi-agent collaboration design |
| **Availability** | OpenRouter |
| **Notable** | Built for autonomous real-world productivity; 56.2% SWE-Pro, 57.0% Terminal Bench 2, 1495 ELO on GDPval-AA; supports Word/Excel/PowerPoint generation, live debugging, root cause analysis, financial modeling; #2 ranked coding model on OpenRouter (April 2026) |
| **Direct API note** | MiniMax has a direct API available — pricing may differ from OpenRouter |

---

## xAI (Grok) — `x-ai/grok-4.1-fast`

| Field | Value |
|---|---|
| **Provider** | xAI |
| **Model ID (OpenRouter)** | `x-ai/grok-4.1-fast` |
| **Released** | November 19, 2025 |
| **Status** | ✅ Active — Best Value xAI Model |
| **Input price (OpenRouter)** | $0.20 / MTok |
| **Output price (OpenRouter)** | $0.50 / MTok |
| **Context window** | 2,000,000 tokens |
| **Availability** | OpenRouter, direct xAI API (console.x.ai) |
| **Notable** | xAI's best agentic tool-calling model; real-world use cases like customer support and deep research; 2M context window (largest in class); optional reasoning mode (enable/disable via API); vision support |
| **Direct API note** | xAI direct API (console.x.ai) — same pricing as OpenRouter. $25 free signup credits available. |

> 📝 **Also watch:** **Grok 4.20** (`x-ai/grok-4.20`) — released March 31, 2026 as xAI's newest premium flagship at **$2.00/$6.00** per MTok with a 2M context window. Best for highest-quality reasoning and the lowest hallucination rate claim. If Grok 4.20 proves superior in benchmarks, it will replace Grok 4.1 Fast as the tracked pick with a 🔄 REPLACED badge.

---

## 💡 OpenRouter Quick Notes

| Feature | Details |
|---|---|
| **API compatibility** | Fully OpenAI-compatible — change `base_url` to `https://openrouter.ai/api/v1` |
| **Billing** | Credit-based, no monthly minimums; pay-per-token |
| **Free models** | 27+ free models available (rate-limited: 20 req/min, 200 req/day) |
| **Rate limits** | Vary by model and account tier; add credits for higher throughput |
| **Fallback routing** | OpenRouter supports multi-provider routing for uptime |
| **Provider count** | 300+ models from all major providers |

---

*Sources verified April 12, 2026.*
