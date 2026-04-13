# 🔵 Mistral AI — Model Cards

> **Last updated:** 2026-04-13  
> **Source:** https://devtk.ai/en/blog/mistral-api-pricing-guide-2026/ · https://pricepertoken.com/pricing-page/provider/mistral-ai · https://mistral.ai/pricing · https://docs.mistral.ai/deployment/ai-studio/pricing  
> **Scraped / verified:** 2026-04-13  

All prices are **USD per million tokens (MTok)**. Mistral offers a **free experimentation tier** (rate-limited) — no credit card required to start. API and consumer (Le Chat) subscriptions are billed **separately**.

> **Mistral's key differentiators:** Native EU data residency (GDPR by default), cheapest output pricing in mid-tier, Apache 2.0 open-weight models for self-hosting.

> ⚠️ **Pricing note — Mistral Large 3:** Some January–February 2026 sources list Large 3 at $2.00/$6.00 (devtk.ai, burnwise.io). More recent provider listings (pricepertoken.com, inworld.ai, Apr 2026) list the `mistral-large-3-2512` version at **$0.50/$1.50**, suggesting a significant price cut for the December 2025 release. The cards below reflect the $0.50/$1.50 rate; verify on the official Mistral console before large-scale deployment.

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
| **Notable** | Exceptionally cheap output pricing vs peers; GDPR-compliant EU hosting by default; no prompt caching available; 262K context window |

---

### Mistral Medium 3

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-medium-latest` |
| **Released** | May 7, 2025 |
| **Status** | ✅ Active — Balanced |
| **Input price** | $0.40 / MTok |
| **Output price** | $2.00 / MTok |
| **Context window** | 131,072 tokens |
| **Max output** | 8,192 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Text, Function Calling, JSON mode |
| **Notable** | Balanced cost and capability; ideal for general chat, summarization, code review |

---

### Mistral Small 3.1

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `mistral-small-latest` |
| **Status** | ✅ Active — Budget / High-Volume |
| **Input price** | $0.20 / MTok |
| **Output price** | $0.60 / MTok |
| **Context window** | 128,000 tokens |
| **Max output** | 4,096 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Text, Function Calling |
| **Notable** | Competitive at the budget tier (between Gemini Flash at $0.15/M and DeepSeek V3.2 at $0.27/M on input); strong for high-throughput classification, extraction, routing |

---

### Codestral

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `codestral-latest` |
| **Status** | ✅ Active — Specialized (Code) |
| **Input price** | $1.00 / MTok |
| **Output price** | $3.00 / MTok |
| **Context window** | 128,000 tokens |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Code generation, code completion, code refactoring |
| **Notable** | Purpose-built code model; strong for fill-in-the-middle (FIM) tasks; powers Mistral Vibe coding agent |

---

### Devstral 2 *(Coding Agent)*

| Field | Value |
|---|---|
| **Provider** | Mistral AI |
| **Model ID** | `devstral-2-latest` |
| **Status** | ✅ Active — Agentic Coding |
| **Availability** | API (Mistral AI Studio) |
| **Capabilities** | Advanced agentic coding, CI/CD automation, multi-file reasoning |
| **Notable** | Purpose-built for autonomous coding agents and developer workflows |

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

### ⚠️ LEGACY — Mistral Large 2 (2407)

| Field | Value |
|---|---|
| **Model ID** | `mistral-large-2407` |
| **Status** | ⚠️ LEGACY — Superseded by Large 3 |
| **Last price** | $2.00 input / $6.00 output per MTok |
| **Context window** | 128,000 tokens |
| **Migration** | Upgrade to **Mistral Large 3 (2512)** — 262K context, lower price |

---

### ⚠️ LEGACY — Mistral Small 3 (older)

| Field | Value |
|---|---|
| **Status** | ⚠️ LEGACY — Superseded by Small 3.1 |
| **Migration** | Upgrade to **Mistral Small 3.1** ($0.20/$0.60) |

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
| **Model routing** | 60/25/15 split (Small/Medium/Large) vs all-Large can reduce costs by 70–80% |

---

## 💬 Le Chat Consumer Plans *(separate from API billing)*

| Plan | Price | Notes |
|---|---|---|
| **Free** | $0/mo | Rate-limited messages, mid-tier models, web search, image generation |
| **Pro** | $14.99/mo | More messages, extended thinking, deep research, 15GB storage, Mistral Vibe CLI — **does NOT include API credits** |
| **Team** | $24.99/user/mo | Up to 30GB storage per user, domain verification, data export, collaborative workspace |
| **Enterprise** | Custom | SSO, audit logs, white label, custom models; contact sales |

> ⚠️ Le Chat Pro does **not** include API access. Consumer and developer API billing are entirely separate. Team plan confirmed at $24.99/user/month on mistral.ai/pricing (verified Apr 13, 2026).

---

*Sources last verified: April 13, 2026 against mistral.ai/pricing, devtk.ai/en/blog/mistral-api-pricing-guide-2026/, and pricepertoken.com/pricing-page/provider/mistral-ai*
