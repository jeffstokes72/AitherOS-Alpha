<div align="center">

<img src="assets/aitheros-logo.jpg" alt="AitherOS" width="200" />

# AitherOS

**An Agentic Operating System — not a chatbot with tools.**

118 microservices · 16 specialist agents · Six-pillar cognitive architecture
Pain-driven recovery · Self-improving feedback loops · Running on real hardware

[![Status](https://img.shields.io/badge/status-alpha-blueviolet?style=flat-square)](https://aitherium.com/demo)
[![Built By](https://img.shields.io/badge/built%20by-one%20person-cyan?style=flat-square)](#)
[![Services](https://img.shields.io/badge/services-118-blue?style=flat-square)](#architecture)
[![Agents](https://img.shields.io/badge/agents-16-purple?style=flat-square)](#agents)

**🚧 Alpha — Coming Soon 🚧**

[What Is This?](#what-is-this) •
[Architecture](#architecture-at-a-glance) •
[Agents](#the-agents) •
[Roadmap](#current-status--roadmap) •
[Stay Updated](#stay-updated)

</div>

---

## What Is This?

AitherOS is a full-stack **agentic operating system** built solo from the ground up. It's not an AI wrapper, not a prompt chain, not a demo — it's 118 FastAPI microservices running across 18 service groups with 16 specialist AI agents that actually coordinate, remember, feel pain, and improve themselves.

> *From Greek αἰθήρ (Aither) — the primordial god of light and the upper air. The invisible medium that makes creation possible.*

**This repo is the public preview.** The source code is being prepared for alpha release. Star and Watch to get notified when it drops.

---

## Architecture at a Glance

```
┌─────────────────────────────────────────────────────────┐
│                    AitherVeil (UI)                       │
│               Next.js Dashboard · Port 3000             │
├─────────────────────────────────────────────────────────┤
│                  Six Cognitive Pillars                   │
│  Perception · Memory · Cognition · Action · Social · Meta│
├─────────────────────────────────────────────────────────┤
│              118 FastAPI Microservices                   │
│         Ports 3000–8783 · 18 Service Groups             │
├─────────────────────────────────────────────────────────┤
│                  16 Specialist Agents                    │
│   Demiurge · Atlas · Lyra · Saga · Forge · Hera · ...   │
├─────────────────────────────────────────────────────────┤
│              AitherZero (PowerShell 7+)                  │
│        109 cmdlets · 268 automation scripts              │
├─────────────────────────────────────────────────────────┤
│     Pain System · Chaos Engineering · Memory Tiers       │
│   Circuit breakers · Self-healing · L0–L4 persistence    │
└─────────────────────────────────────────────────────────┘
```

For a deeper dive, see [ARCHITECTURE.md](docs/ARCHITECTURE.md).

---

## What Makes It an "Agentic OS"

This isn't prompt automation. It's a living system.

| Requirement | How AitherOS Does It |
|---|---|
| **Persistent Identity** | Each agent has memory, personality, its own port, and domain expertise |
| **Autonomous Action** | Agents act without prompting — scheduled routines, self-healing, proactive tasks |
| **Multi-Agent Coordination** | 16 agents coordinate via event bus, not serial chains |
| **Environmental Awareness** | Pain system, health monitoring, resource sensing across all services |
| **Self-Improvement** | Chaos engineering (Seven Sins), evolution feedback loops |
| **Human Governance** | Humans set policy. AI executes. Always. |

---

## The Agents

| Agent | What It Does |
|---|---|
| 🏛️ **Atlas** | Maintains roadmap, orchestrates Lyra + Demiurge |
| 🔨 **Demiurge** | The Divine Craftsman — intent → working code |
| 📚 **Lyra** | Research librarian — deploys scouts and neurons |
| 📖 **Saga** | Epic storyteller with narrative generation |
| 🎮 **Prometheus** | Tick-based simulation engine |
| ⚒️ **Forge** | Sub-agent spawning and research orchestration |
| 📰 **Vera** | Interactive content editor |
| 📢 **Hera** | System-wide news wire and broadcast |
| 🤖 **AitherAgent** | Unified orchestrator across all agents |
| 🏗️ **ServicesManager** | Master of infrastructure |
| 👁️ **GenesisAgent** | Lifecycle management, zombie cleanup, LLM fallback |
| 🔧 **InfraAgent** | OpenTofu/Terraform DevOps automation |
| ⚡ **AutomationAgent** | PowerShell automation and script execution |
| 🎬 **Director** | Creative direction and media production |
| 📊 **Executive** | Testing + documentation metrics |
| 🧪 **Testing** | Automated test runner (pytest/Pester) |

---

## Service Groups

18 groups covering the full spectrum:

`agents` · `automation` · `bootloader` · `cognition` · `communication` · `core` · `creative` · `gpu` · `infrastructure` · `mcp` · `memory` · `mesh` · `orchestration` · `perception` · `security` · `social` · `training` · `ui`

---

## Cool Stuff Worth Highlighting

### 🩸 Pain System
Services report pain on a 0–10 scale. High pain triggers automatic recovery, circuit breakers, and cascading alerts. Not metaphorical — it's how the system self-heals.

### 😈 Seven Sins of Chaos
Intentional fault injection — Wrath, Sloth, Greed, Envy, Pride, Gluttony, Lust — each with configurable aggression levels. Resilience isn't optional.

### 🌊 Elementals
Four specialized AI personalities (Ignis/Fire, Aqua/Water, Terra/Earth, Aether/Air) with distinct temperaments and lineages.

### 🧠 Five-Tier Memory
L0 (volatile registers, μs) → L1 (working memory, seconds) → L2 (episodic, minutes) → L3 (long-term, days) → L4 (archival, permanent).

### ⚙️ 268 Automation Scripts
Numbered 0000–9999, covering everything from environment setup to chaos testing to deep cleaning.

---

## Tech Stack

| Layer | Tech |
|---|---|
| **Services** | Python 3.12, FastAPI, Docker Compose |
| **Automation** | PowerShell 7+, 109 cmdlets |
| **Dashboard** | Next.js 14, React, Tailwind CSS, Framer Motion |
| **AI** | Multi-model (Ollama local, cloud fallback), tiered routing |
| **Infrastructure** | Docker, Genesis bootloader, health mesh |

---

## Current Status & Roadmap

🟡 **Alpha** — The system runs on real hardware daily. APIs are stabilizing, docs are being written, and the public build is being prepared.

See [ROADMAP.md](ROADMAP.md) for what's coming.

| Phase | Status |
|---|---|
| Core services running | ✅ Complete |
| 16 agents operational | ✅ Complete |
| Pain system + self-healing | ✅ Complete |
| AitherVeil dashboard | ✅ Complete |
| Docker Compose deployment | ✅ Complete |
| Public alpha release | 🔜 Coming Soon |
| Documentation site | 🔜 Coming Soon |
| Community contributions | 📋 Planned |

---

## Stay Updated

This repo will be the home of the public alpha. Here's how to follow along:

- ⭐ **Star** this repo to bookmark it
- 👁️ **Watch** for release notifications
- 🌐 Visit [aitherium.com/demo](https://aitherium.com/demo) for the demo page

---

## License

AitherOS is proprietary software. Alpha access details will be announced soon.

---

<div align="center">

**Built with obsession by one person.**

*The element of creation.*

</div>
