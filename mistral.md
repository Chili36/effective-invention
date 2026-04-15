# 🔵 Mistral AI — Model Cards

> **Last updated:** 2026-04-15  
> **Source:** https://mistral.ai/pricing · https://pricepertoken.com/pricing-page/provider/mistral-ai (updated Apr 12, 2026) · https://devtk.ai/en/blog/mistral-api-pricing-guide-2026/ · https://docs.mistral.ai/deployment/ai-studio/pricing  
> **Scraped / verified:** 2026-04-15  

All prices are **USD per million tokens (MTok)**. Mistral offers a **free experimentation tier** (rate-limited) — no credit card required to start. API and consumer (Le Chat) subscriptions are billed **separately**.

> **Mistral's key differentiators:** Native EU data residency (GDPR by default), cheapest output pricing in mid-tier, Apache 2.0 open-weight models for self-hosting.

> ⚠️ **Pricing note — Mistral Large 3:** Some January–February 2026 sources list Large 3 at $2.00/$6.00 (devtk.ai, burnwise.io). More recent provider listings (pricepertoken.com, Apr 2026) list the `mistral-large-3-2512` version at **$0.50/$1.50**, suggesting a significant price cut for the December 2025 release. The cards below reflect the $0.50/$1.50 rate; verify on the official Mistral console before large-scale deployment.

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
| **Context window** | 262,144 tokens |
| **Max output** | 8,192 tokens |
| **Availability** | API (Mistral AI Studio / La Plateforme), Azure AI Foundry |
| **Capabilities** | Text, Vision, Function Calling, JSON mode |
| **Rate limits** | Paid tier; contact Mistral for enterprise limits |
| **Notable** | Exceptionally cheap output pricing vs peers; GDPR-compliant EU hosting by default; 262K context window |

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

### Mistral Small 4 *(Released March 3, 2026)*

> **🆕 NEW (Apr 15, 2026):** Mistral Small 4 was released March 3, 2026 and represents the current recommended Small-tier model. Small 3.1 is now superseded.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-small-latest` |
| **Released** | March 3, 2026 |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.15 / MTok |
| **Output price** | ~$0.60 / MTok *(verify on official console — may vary)* |
| **Context window** | 128,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Text, Function Calling, Agentic tasks, Coding, Multimodal (input) |
| **Notable** | Reasoning-optimized; improved agentic and coding performance over Small 3.x; `mistral-small-latest` now routes here; cheaper input than Small 3.1 ($0.20→$0.15) |

> ⚠️ **Pricing verification:** The $0.15/M input price is sourced from flowlyn.com (April 2026 pricing calculator). Always verify on the official Mistral console at console.mistral.ai before production deployment.

---

### Codestral 2508 *(Updated August 2025)*

> **🆕 UPDATE (Apr 15, 2026):** Codestral was updated to version 2508 in August 2025 with a significant price reduction from $1.00/$3.00 → $0.30/$0.90.

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `codestral-latest` |
| **Released** | August 2025 (version 2508; supersedes Codestral 2501) |
| **Status** | ✅ Active — Specialized (Code) |
| **Input price** | $0.30 / MTok |
| **Output price** | $0.90 / MTok |
| **Context window** | 128,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Code generation, code completion, fill-in-the-middle (FIM), code refactoring |
| **Notable** | Purpose-built code model; 70% cheaper than previous Codestral 2501 ($1.00/$3.00); powers Mistral Vibe coding agent |

---

### Devstral 2 *(Coding Agent)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `devstral-latest` |
| **Status** | ✅ Active — Agentic Coding (Flagship) |
| **Input price** | $0.40 / MTok |
| **Output price** | $2.00 / MTok |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Advanced agentic coding, CI/CD automation, multi-file reasoning |
| **Notable** | Purpose-built for autonomous coding agents and developer workflows; higher tier than Devstral Small |

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
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Coding agents, code generation, CI/CD automation |
| **Notable** | Ultra-affordable coding agent; open weights available |

---

### Voxtral Small 24B *(Audio / Speech)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `voxtral-small-latest` |
| **Released** | October 2025 (version 2507) |
| **Status** | ✅ Active — Specialized (Audio) |
| **Input price** | $0.10 / MTok |
| **Output price** | $0.30 / MTok |
| **Context window** | 128,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Audio processing, voice understanding, speech-to-text, audio analysis |
| **Notable** | Mistral's dedicated audio model; purpose-built for voice and speech workloads |

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
| **Notable** | Largest context window in the Ministral family |

---

## 🔓 Open-Weight / Self-Hosted Models

> These models are available for free self-hosting under **Apache 2.0** license. No API costs — only compute infrastructure.

| Model | Parameters | License | Best For |
|---|---|---|---|
| **Mixtral 8×22B** | 141B (MoE) | Apache 2.0 | Self-hosted complex reasoning, high-throughput |
| **Mixtral 8×7B** | 46.7B (MoE) | Apache 2.0 | General-purpose self-hosted tasks |
| **Mistral 7B** | 7B | Apache 2.0 | Edge deployment, on-device, low-resource |

> **Note:** Open-weight models do not receive commercial support and may lag behind API models in capability. Mixtral 8×7B on a single A100 GPU can compete with API costs above ~$500–1,000/month.

---

## ⚠️ Legacy Models

### ⚠️ LEGACY — Mistral Small 3.2 24B *(Superseded by Small 4)*

| Field | Value |
|---|---|
| **Model ID** | `mistral-small-3.2` |
| **Released** | June 2025 |
| **Status** | ⚠️ LEGACY — Superseded by Mistral Small 4 (March 2026) |
| **Last price** | $0.07 input / $0.20 output per MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Upgrade to **Mistral Small 4** — better capabilities; `mistral-small-latest` now routes to Small 4 |

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
| **Migration** | Upgrade to **Mistral Large 3 (2512)** — 262K context, lower price |

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

---

## 💬 Le Chat Consumer Plans *(separate from API billing)*

| Plan | Price | Notes |
|---|---|---|
| **Free** | $0/mo | Rate-limited messages, mid-tier models, web search, image generation |
| **Pro** | $14.99/mo | More messages, extended thinking, deep research, 15GB storage, Mistral Vibe CLI — **does NOT include API credits** |
| **Team** | $24.99/user/mo | Up to 30GB storage per user, domain verification, data export, collaborative workspace |
| **Enterprise** | Custom | SSO, audit logs, white label, custom models; contact sales |

> ⚠️ Le Chat Pro does **not** include API access. Consumer and developer API billing are entirely separate. Team plan confirmed at $24.99/user/month on mistral.ai/pricing (verified Apr 15, 2026).

---

*Sources last verified: April 15, 2026 against mistral.ai/pricing, pricepertoken.com/pricing-page/provider/mistral-ai (updated Apr 12, 2026), and devtk.ai/en/blog/mistral-api-pricing-guide-2026/*
