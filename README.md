<div align="center">

# Asman Mirza

**Engineer · Architect · Founder**

*Building the infrastructure layer that should already exist*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/asman3m)
[![X](https://img.shields.io/badge/X-%23000000.svg?style=flat&logo=x&logoColor=white)](https://x.com/asman_mirza)
[![Email](https://img.shields.io/badge/Email-%23EA4335.svg?style=flat&logo=gmail&logoColor=white)](mailto:rambo007.am@gmail.com)

</div>

---

I lead teams by day and build ecosystems by night.

My stack runs from Android NDK to bare-metal Rust services — no abstraction layer is too high, no system too low. I've fine-tuned LLMs, written custom WebRTC SFU servers, shipped OS-level Android tooling, architected microservice migrations for Fortune 500 energy infrastructure, designed post-quantum cryptography platforms, and somewhere in between, started questioning whether transformers are the right architecture at all.

Primary languages: **Kotlin · Rust**. Secondary religion: making things fast.

---

## 🏗️ What I'm Shipping *(always evolving)*

> Not side projects. A connected vision: own every layer of the AI development lifecycle — and secure it while you're at it.

---

### 🔥 [Runlit](https://runlit.dev) · [github.com/runlit-dev](https://github.com/runlit-dev) — *The trust layer below your AI IDE*

AI writes fast. Runlit keeps score. An eval layer that catches what code review misses — hallucinated APIs, intent mismatches, security vulnerabilities, and compliance violations — **before** they reach production.

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

139 rules. 12 provider-specific packs (OpenAI, Anthropic, LangChain, Stripe...). 30-second GitHub App install. Merge-blocking. MIT-licensed rules.

> **1.7×** more issues in AI-generated code. **45%** of AI tasks introduce security vulnerabilities. **75%** of enterprise engineers will use AI coding tools by 2028. Runlit exists because those three numbers are a collision course.

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

### 🔐 [QShield](https://github.com/asman1337/qshield) — *Quantum-safe by default.*

The full-stack post-quantum cryptography migration platform. Secures all four layers — transport, authentication, secrets storage, and credentials — under one open core, before quantum computers make today's encryption obsolete.

> 1Password secures passwords. Cloudflare secures transport. Nobody secures all four layers under one brand with one open core. **QShield is that platform.**

Built in Rust. Aligned to NIST FIPS 203 (ML-KEM), FIPS 204 (ML-DSA), and FIPS 205 (SLH-DSA). India-first. Enterprise and government-ready. Harvest-now-decrypt-later attacks are already happening — the migration window is open and won't stay that way.

| Product | What it does |
|---|---|
| **QShield Core** | Open-source PQC library — ML-KEM, ML-DSA, hybrid classical+PQC. Rust-native with Python, Node, Go, Java bindings |
| **QShield Proxy** | Drop-in PQC-hybrid TLS termination. Zero application code changes |
| **QShield Vault** | PQC-first zero-knowledge secrets manager. Browser, desktop, mobile |
| **QShield Auth** | Drop-in Auth0/Clerk replacement issuing ML-DSA-signed JWTs |
| **QShield Enterprise** | Codebase scanning, PQC readiness scoring, CERT-In / RBI / SEBI compliance reports |

`Rust` `ML-KEM` `ML-DSA` `SLH-DSA` `PyO3` `NAPI-RS` `WASM` `Tauri 2` `Flutter` `Apache 2.0`

---

## 🧬 Research

### NEXUS / NOOR — *A post-transformer cognitive architecture*

> **Neural Execution & Understanding System.** Not an LLM variant. A new architecture class.

NEXUS addresses fundamental flaws in the transformer architecture. NOOR is the first model family built on it — scaling bottom-up with intention, not brute force:

| Model | Params | Context | Status |
|---|---|---|---|
| **NOOR Nano** | 29M | 512 | v0.4 training |
| **NOOR Micro** | 80–120M | 2048 | Next |
| NOOR Mini | ~350M | TBD | Planned |
| NOOR Small | ~1B | TBD | Planned |

Also running **Grafts** — NEXUS modules injected into existing open-source backbones (Qwen-NOOR, Gemma-NOOR) as experimental sidelines.

*This is what happens when you spend enough time staring at transformer limitations that you decide to do something about it.*

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
- Built and fine-tuned a **generative AI training platform** for HCTRA — Meta Llama 3, Rust + Python, custom fine-tuning pipeline.

---

## 📊 Stats

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=asman1337&theme=radical&hide_border=true)](https://github.com/asman1337)

</div>

---

<div align="center">
<sub>The gap between "AI writes it" and "safe to ship" — and between "encrypted today" and "secure tomorrow" — those are the problems worth solving.</sub>
</div>
