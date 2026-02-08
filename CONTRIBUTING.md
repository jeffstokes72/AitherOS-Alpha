# Contributing to AitherOS

> 🚧 **AitherOS is not yet accepting contributions.** This will change with the alpha release.

## When Can I Contribute?

We're preparing the codebase for public collaboration. Once the alpha is released, we'll open up:

- **Bug reports** — Found something broken? Let us know
- **Documentation** — Improve guides, fix typos, add examples
- **Agent plugins** — Build your own specialist agents
- **Automation scripts** — PowerShell 7+ scripts for the AitherZero library
- **Dashboard components** — React components for AitherVeil

## How to Prepare

1. **⭐ Star and 👁️ Watch** this repo for release notifications
2. **Read the [Architecture docs](docs/ARCHITECTURE.md)** to understand the system
3. **Check the [Roadmap](ROADMAP.md)** to see where we're headed
4. **Set up your environment** — You'll need:
   - Docker Desktop
   - PowerShell 7+
   - Node.js 18+
   - Python 3.12+
   - Ollama (for local LLMs)

## Code Standards (Preview)

When contributions open, we'll expect:

### Python (AitherOS services)
- FastAPI for all services
- Use `AitherService` integration class (no boilerplate)
- Ports from `services.yaml` — never hardcoded
- Lifecycle hooks via `setup_lifecycle()`

### PowerShell (AitherZero)
- Singular nouns for cmdlets (`Get-Service`, not `Get-Services`)
- Pipeline-friendly design (`ValueFromPipeline`)
- Always source `_init.ps1` in automation scripts
- No duplicate scripts — use parameters

### General
- Every feature needs tests
- Documentation is not optional
- Docker support required
- Follow existing patterns

---

*We believe documentation is love made visible to users. When we open contributions, we'll expect the same care.*
