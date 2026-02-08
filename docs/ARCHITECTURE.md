# AitherOS Architecture

> Detailed architecture documentation is coming with the alpha release. This is a high-level overview.

## System Overview

AitherOS is composed of two major subsystems:

### AitherZero — The Automation Layer

PowerShell 7+ cross-platform automation framework.

- **109 cmdlets** for infrastructure management
- **268 numbered scripts** (0000–9999) for systematic automation
- **Playbook engine** for orchestrating multi-step operations
- **Module system** with public/private function separation

### AitherOS — The Intelligence Layer

Python 3.12 microservices architecture with AI-native design.

- **118 FastAPI services** across 18 service groups
- **16 specialist agents** with persistent identity and memory
- **Genesis bootloader** for service lifecycle management
- **Event bus** for inter-service communication

## Six Cognitive Pillars

The service architecture is organized around six cognitive pillars:

| Pillar | Purpose | Example Services |
|---|---|---|
| **Perception** | Sensing the environment | Health monitors, resource sensors, pain system |
| **Memory** | Storing and retrieving knowledge | Five-tier memory (L0–L4), Chronicle, episodic store |
| **Cognition** | Thinking and reasoning | LLM routing, model selection, inference pipelines |
| **Action** | Executing in the world | Automation agents, Demiurge, infrastructure management |
| **Social** | Communicating externally | Moltbook, LinkedIn, content publishing |
| **Meta** | Self-awareness and improvement | Chaos engineering, evolution, self-healing |

## Service Communication

```
                    ┌──────────────┐
                    │  AitherVeil  │  (Dashboard UI)
                    │  Port 3000   │
                    └──────┬───────┘
                           │
                    ┌──────┴───────┐
                    │   AitherNode │  (API Gateway)
                    │  Port 8080   │
                    └──────┬───────┘
                           │
              ┌────────────┼────────────┐
              │            │            │
     ┌────────┴──┐  ┌──────┴────┐  ┌───┴────────┐
     │  Genesis  │  │  Agents   │  │  Services  │
     │ Port 8001 │  │ 8140-8783 │  │ 8081-8139  │
     └───────────┘  └───────────┘  └────────────┘
```

- **REST APIs** between services (FastAPI + httpx)
- **Event bus** for pub/sub messaging
- **Pain signals** propagate through the health mesh
- **Genesis** manages lifecycle for all services

## Deployment Model

```
┌──────────────────────────────────────┐
│          Docker Compose              │
│                                      │
│  ┌─────────┐  ┌─────────┐          │
│  │  Core   │  │  Agents  │  ...     │
│  │ Profile │  │ Profile  │          │
│  └─────────┘  └─────────┘          │
│                                      │
│  ┌─────────────────────────────┐    │
│  │   Shared: Ollama, Redis,    │    │
│  │   PostgreSQL, Volumes       │    │
│  └─────────────────────────────┘    │
└──────────────────────────────────────┘
```

Services are grouped into Docker Compose **profiles** so you can run only what you need:

| Profile | Services | Use Case |
|---|---|---|
| `core` | Genesis, Secrets, Chronicle, Pulse, Node, Veil | Minimum viable system |
| `agents` | All 16 specialist agents | Full agent coordination |
| `social` | Moltbook, LinkedIn, content services | Social media automation |
| `ml` | vLLM, training services | GPU-accelerated inference |
| `full` | Everything | The whole enchilada |

---

*Full architecture documentation, API references, and integration guides will ship with the alpha release.*
