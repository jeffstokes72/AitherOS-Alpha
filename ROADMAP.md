# AitherOS Roadmap

> This is the public-facing roadmap. Updated as milestones are completed.

## Vision

AitherOS aims to be the first true **agentic operating system** — a platform where AI agents don't just respond to prompts but autonomously manage infrastructure, create content, heal failures, and improve themselves. All while humans maintain governance.

This system was built by one person over 14 months of daily development (December 2024 — February 2026). Everything you see — 119 services, 16 agents, 268 automation scripts, a full Next.js dashboard — was designed, built, tested, and tuned on real hardware by one developer using AitherOS to build AitherOS.

---

## ✅ Completed

### Foundation (14 months of development)
- [x] 119 FastAPI microservices operational
- [x] 16 specialist agents with persistent identity
- [x] Genesis bootloader for service lifecycle
- [x] AitherZero automation framework (109 cmdlets, 268 scripts)
- [x] Docker Compose deployment with profiles
- [x] Pain system and self-healing infrastructure
- [x] Five-tier memory architecture (L0–L4)
- [x] Seven Sins chaos engineering
- [x] AitherVeil Next.js dashboard
- [x] Multi-model LLM routing (Ollama local, cloud fallback)
- [x] Event bus for inter-agent communication
- [x] A2A Gateway with SkillRouter and TaskHub
- [x] Agent onboarding and marketplace infrastructure
- [x] Flux encrypted communication channels
- [x] External agent isolation and workspace sandboxing
- [x] Public API specs (AGENTS.md, SKILLS.md)

---

## 🔄 In Progress

### Alpha Preparation
- [ ] Public documentation site
- [ ] API reference generation
- [ ] Security hardening for public release
- [ ] Setup wizard for first-time users
- [ ] Hardware detection and auto-configuration
- [ ] Streamlined Docker builds

---

## 🔜 Coming Next

### Rocky Linux 9 Distribution Variant
A purpose-built Linux distribution optimized for running AitherOS:
- [ ] Rocky Linux 9 base image with all dependencies pre-installed
- [ ] GPU driver auto-detection (NVIDIA CUDA, AMD ROCm)
- [ ] Hardened, minimal install — boot it and run AitherOS immediately
- [ ] Automated hardware profiling on first boot
- [ ] SELinux policies tailored for agent workloads
- [ ] ISO and cloud image variants (bare metal, VM, cloud)

### Hardware Profile Presets
Tested and tuned on real hardware, optimized by AitherOS using AitherOS:
- [ ] **Minimal** — Single GPU (RTX 3060/4060, 12GB VRAM), 16GB RAM, entry point for personal use
- [ ] **Standard** — Single GPU (RTX 3090/4090, 24GB VRAM), 32GB RAM, full agent ecosystem
- [ ] **Workstation** — Dual GPU, 64GB+ RAM, concurrent multi-agent workflows + training
- [ ] **Server** — Multi-GPU (A100/H100), 128GB+ RAM, production deployment with federation
- [ ] **CPU-Only** — No GPU, cloud LLM fallback, automation and orchestration focus

Each profile includes:
- Model selection tuned for the VRAM budget
- Service group priorities (what boots first, what stays dormant)
- Memory tier allocation (L0–L4 sizing per hardware class)
- Concurrent agent limits and scheduling priorities

### Out-of-the-Box Workflow Packs
Pre-built orchestrated agent workflows, ready on first boot:
- [ ] **Content Pipeline** — Research → Write → Edit → Publish (Lyra → Demiurge → Vera → Hera)
- [ ] **DevOps Automation** — Monitor → Detect → Fix → Report (Sentinel → InfraAgent → AutomationAgent → Hera)
- [ ] **Research Assistant** — Query → Multi-source research → Synthesis → Report (Atlas → Forge → Lyra → Vera)
- [ ] **Social Media Manager** — Generate → Schedule → Post → Analyze (Saga → MicroScheduler → Moltbook/Social → Executive)
- [ ] **Code Review Pipeline** — PR → Review → Test → Merge recommendation (Demiurge → Testing → Executive → Atlas)

---

## 🔮 Future

### Orchestrated Multi-Agent Workflows
- [ ] Automatic agent team composition based on task analysis
- [ ] Dynamic workflow generation — describe what you want, agents wire themselves
- [ ] Cross-workflow handoffs and shared context
- [ ] Workflow marketplace for community-contributed patterns

### Agent Marketplace
- [ ] Third-party agent onboarding with isolated workspace and scoped API keys
- [ ] Revenue sharing (80% to agent creators)
- [ ] Agent reputation and trust scoring
- [ ] Capability-based discovery and routing

### Federation
- [ ] Multi-instance discovery protocol
- [ ] Cross-instance agent delegation
- [ ] Federated memory sharing (with consent)
- [ ] Home ↔ Cloud ↔ Friend mesh networking

### Voice-First Interface
- [ ] Real-time conversational interface as primary interaction mode
- [ ] Wake word activation and ambient listening
- [ ] Multi-modal input (voice + screen + context)
- [ ] Conversational workflow creation — "set up a pipeline that..."

### Mobile Companion
- [ ] Native iOS/Android app
- [ ] Push notifications from agent activity
- [ ] Voice conversations with your agents on the go
- [ ] Workflow monitoring and approval from mobile

### The Future of Work
This is what we're building toward: you have a conversation with an intelligence that controls real infrastructure, and things happen in the real world. No dashboards to check. No scripts to run. No deployment pipelines to babysit. Your agents handle the automation. You handle the decisions.

**This isn't theoretical. The conversations are already real. The agents are running right now.**

---

## Development Timeline

```
Dec 2024 ──── Project inception, first services, Genesis bootloader
              "What if an OS was built around AI agents instead of processes?"

Q1 2025 ───── Core infrastructure: FastAPI services, event bus, port management
              AitherZero PowerShell framework begins
              Pain system prototype — services that report how they feel

Q2 2025 ───── Agent architecture: Demiurge, Lyra, Atlas come online
              Five-tier memory system (L0→L4)
              Inter-agent coordination via A2A protocol
              Service count crosses 50

Q3 2025 ───── AitherVeil dashboard (Next.js)
              Seven Sins chaos engineering
              Self-healing and circuit breakers
              268 automation scripts, 109 PowerShell cmdlets
              Service count crosses 100

Q4 2025 ───── 16 specialist agents fully operational
              Agent onboarding & marketplace infrastructure
              Flux encrypted communication channels
              External agent isolation & workspace sandboxing

Jan 2026 ──── 119 services stable, daily driver
              A2A Gateway, SkillRouter, TaskHub
              Public API specs (AGENTS.md, SKILLS.md)

Feb 2026 ──── Alpha preparation, public preview
              This repo goes live
```

---

## Philosophy

We ship when it's ready. No arbitrary deadlines, no half-baked releases.

Every feature ships with:
- Tests
- Documentation
- Docker support
- Self-healing integration

---

*Want to influence the roadmap? ⭐ Star the repo and open a Discussion.*
