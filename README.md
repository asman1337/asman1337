<div align="center">

# Asman Mirza

**Engineer · Architect · Founder**

*Building the infrastructure layer that should already exist*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/asman3m)
[![X](https://img.shields.io/badge/X-%23000000.svg?style=flat&logo=x&logoColor=white)](https://twitter.com/asman1337)
[![Email](https://img.shields.io/badge/Email-%23EA4335.svg?style=flat&logo=gmail&logoColor=white)](mailto:rambo007.am@gmail.com)

</div>

---

I lead teams by day and build ecosystems by night.

My stack runs from Android NDK to bare-metal Rust services — no abstraction layer is too high, no system too low. I've fine-tuned LLMs, written custom WebRTC SFU servers, shipped OS-level Android tooling, architected microservice migrations for Fortune 500 energy infrastructure, and somewhere in between, started building the AI tooling I couldn't find anywhere else.

Primary languages: **Rust · Go · Kotlin**. Secondary religion: making things fast.

---

## 🏗️ What I'm Shipping *(always evolving)*

> Not side projects. A connected vision: own every layer of the AI development lifecycle.

---

### 🔥 [Runlit](https://runlit.dev) · [github.com/runlit-dev](https://github.com/runlit-dev) — *The trust layer below your AI IDE*

AI writes fast. Runlit keeps score. An eval layer that sits below your AI IDE and catches what code review misses — hallucinated APIs, intent mismatches, security vulnerabilities, and compliance violations — **before** they reach production.

```bash
$ runlit check --pr 2847
→ scanning 147 lines (AI attribution: Cursor/claude-sonnet)
  hallucination     0 phantom APIs found          ✓  1.00
  intent            matches spec, minor drift      ✓  0.91
  security          no critical issues             ✓  0.97
  compliance        1 medium finding (PCI 6.2.4)   ⚠  0.88
  eval.score        94 / 100
✓ CLEARED — merge when ready.
```

139 rules. 12 provider-specific packs (OpenAI, Anthropic, LangChain, Stripe...). Installs in 30 seconds via GitHub App. Blocks merges when score drops below threshold. MIT-licensed rules.

> The numbers making this necessary: **1.7×** more issues in AI-generated code. **45%** of AI tasks introduce security vulnerabilities. **75%** of enterprise engineers will use AI coding tools by 2028.

`Rust` `GitHub App` `GitLab` `Azure DevOps` `Bitbucket` `CLI` `GitHub Actions`

---

### ⚡ [Routra](https://routra.dev) · [github.com/routra-dev](https://github.com/routra-dev) — *One API. Every GPU Cloud.*

Intelligent LLM routing layer between your app and 10+ GPU providers. Scores every provider every 30s on price, latency, uptime, and queue depth. Routes to the cheapest option that meets your SLA — `<8ms` overhead, `<200ms` auto-failover.

```python
# Before
client = openai.OpenAI(api_key="sk-...")

# After. That's it.
client = openai.OpenAI(api_key="rtr-...", base_url="https://api.routra.dev/v1")
```

> Typical savings: **60% of inference spend.** Adaptive ML routing via LinUCB bandit — learns per model, region, and time-of-day.

`Rust` `Axum` `OpenAI-compatible` `Python SDK` `TypeScript SDK` `Go SDK` `Rust SDK` `CLI`

---

### 🖥️ [Zylora](https://zylora.dev) · [github.com/zylora-dev](https://github.com/zylora-dev) — *Serverless GPU. Zero DevOps.*

Decorate a function. Get a production HTTPS endpoint backed by GPU hardware. No Docker, no YAML, no DevOps hire. Not Python-first — full feature parity across Python, TypeScript, Go, and Rust. Same mental model, idiomatic syntax per language.

`Serverless` `GPU` `Python` `TypeScript` `Go` `Rust` `Multi-Language SDK`

---

### 🤖 [QCHO](https://qcho.ai) · [github.com/qcho-ai](https://github.com/qcho-ai) — *Ambient AI for your entire digital life*

Not a chatbot. A background-capable multi-agent operating layer — voice-first, connector-driven, deeply personalised via persistent per-user memory (`imprint.bit`). Orchestrates Gmail, Calendar, Notion, Slack, GitHub, and custom MCP servers. Every external dependency behind a swappable adapter trait.

```
SENSA (intent) → ORACLE (task decompose + DAG) → Agent Mesh → Connectors → ECHO (response)
```

`Rust` `Axum` `Tauri 2` `Next.js 16` `Claude (Anthropic)` `pgvector` `Whisper` `ElevenLabs`

---

### ☁️ [Nuclyr](https://nuclyr.cloud) · [github.com/nuclyr](https://github.com/nuclyr) — *Multi-Cloud. Made for India.*

Route storage, compute, and data workloads across AWS, GCP, and Azure — automatically. Built for Indian businesses: INR billing, UPI/Razorpay, GST invoices, DPDP compliance scanning. Phase 1 shipped: gRPC-first architecture, AES-256-GCM per-tenant encryption, Rust adapters, full SDK surface.

`Rust` `gRPC` `Protobuf` `Next.js` `PostgreSQL 18` `Redis` `Razorpay`

---

## 🛠️ Core Stack

**Systems & Backend**

![Rust](https://img.shields.io/badge/Rust-%23000000.svg?style=flat&logo=rust&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-%230095D5.svg?style=flat&logo=kotlin&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-%2300599C.svg?style=flat&logo=c%2B%2B&logoColor=white)
![Java](https://img.shields.io/badge/Java-%23ED8B00.svg?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-%236DB33F.svg?style=flat&logo=spring&logoColor=white)
![Ktor](https://img.shields.io/badge/Ktor-%23087CFA.svg?style=flat&logo=kotlin&logoColor=white)

**AI & Infra**

![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=flat&logo=amazon-aws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-%230db7ed.svg?style=flat&logo=docker&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-%23231F20.svg?style=flat&logo=apachekafka&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-%23244c5a.svg?style=flat&logo=google&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-%23316192.svg?style=flat&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-%23DC382D.svg?style=flat&logo=redis&logoColor=white)

**Mobile & Multiplatform**

![Android NDK](https://img.shields.io/badge/Android%20NDK-%2320232a.svg?style=flat&logo=android&logoColor=%23a4c639)
![KMP](https://img.shields.io/badge/Kotlin%20Multiplatform-%230095D5.svg?style=flat&logo=kotlin&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-%234285F4.svg?style=flat&logo=jetpackcompose&logoColor=white)

---

## 📌 By Day

- **Application Lead @ Vendeep / NRG Energy** *(2022 – present)* — Leading a 25-person team modernizing legacy enterprise portlets into microservices. 145+ APIs migrated across Spring Boot, FastAPI, and Salvo. Still running.
- **Senior Android + Reverse Engineering @ Innobuzz** *(2020 – 2022)* — NDK-level engineering, custom OS injection, Android security tooling at the system layer.
- Delivered 4 production phases for **HCTRA** (Harris County Toll Road Authority, Houston) — Kafka streaming, Oracle GoldenGate, millions of daily toll transactions.
- Built and fine-tuned a **generative AI employee training platform** for HCTRA — Meta Llama 3, Rust + Python, custom fine-tuning pipeline.

---

## 🔭 What's next

- Quantum Computing & Quantum ML — Qiskit coursework done, actively watching the space mature
- Rust as the *default*, not the exception, for production-critical paths
- Multi-agent coordination patterns — memory architecture, adaptive routing, DAG orchestration at scale

---

## 📊 Stats
 
<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=asman1337&theme=radical&hide_border=true)](https://github.com/asman1337)

</div>

---

<div align="center">
<sub>The gap between "AI writes it" and "safe to ship" — that's the problem worth solving.</sub>
</div>
