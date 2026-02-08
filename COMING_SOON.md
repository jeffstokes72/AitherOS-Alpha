# 🚧 AitherOS Alpha — Coming Soon

## What's Coming

AitherOS is preparing for its first public alpha release. Here's what you'll get when it drops:

### Day-One Alpha Includes

- **Docker Compose one-liner** — `docker compose up` and you're running
- **Core services** — Genesis bootloader, Secrets, Chronicle, Pulse, Node
- **AitherVeil dashboard** — Next.js UI at `localhost:3000`
- **Local LLM support** — Ollama integration with tiered model routing
- **16 specialist agents** — Each with its own port, personality, and domain
- **Pain system** — Self-healing infrastructure out of the box
- **268 automation scripts** — PowerShell 7+ tooling for everything

### Hardware Requirements (Estimated)

| Tier | RAM | GPU | What You Get |
|---|---|---|---|
| **Minimal** | 8 GB | None | Core services, CPU inference |
| **Recommended** | 16 GB | 6 GB VRAM | Full stack, local LLM |
| **Full** | 32 GB+ | 12 GB+ VRAM | Everything, fast inference, all agents |

### Quick Preview of Setup

```powershell
# Clone
git clone https://github.com/Aitherium/aitheros-alpha.git
cd aitheros-alpha

# Setup (detects hardware, builds images)
pwsh -File ./setup-docker.ps1

# Pull a model
ollama pull llama3.2

# Launch
docker compose -f docker-compose.aitheros.yml --profile core up -d

# Open dashboard
# → http://localhost:3000
```

## Timeline

We're not giving dates — we're giving milestones. When each milestone is met, we ship.

| Milestone | Status |
|---|---|
| Core services stable | ✅ Done |
| Agent coordination working | ✅ Done |
| Docker deployment tested | ✅ Done |
| Documentation written | 🔄 In Progress |
| Security audit | 🔄 In Progress |
| Public alpha tag | 🔜 Next |

## How to Get Notified

1. **⭐ Star** this repository
2. **👁️ Watch** → Select "Releases only" for minimal noise
3. **🌐 Visit** [aitherium.com/demo](https://aitherium.com/demo)

---

*We'd rather ship late and solid than early and broken.*
