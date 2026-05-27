# PANTHEON STACK

The unified AI replacement stack. Five engines. One command.

## Architecture

```
┌─────────────────────────────────────────────────────────┐
│                    OPENHUMAN                            │
│              (Command Center — Desktop UI)              │
└──────────────────────┬──────────────────────────────────┘
                       │
         ┌─────────────┼─────────────┐
         │             │             │
    ┌────▼────┐   ┌────▼────┐  ┌────▼────┐
    │ MERCURY │   │  CORAL  │  │ METAGPT │
    │ (Always │   │(Self-   │  │(Strategy│
    │  -On    │   │ Evolve) │  │ Brain)  │
    │ Daemon) │   └────┬────┘  └────┬────┘
    └────┬────┘        │            │
         │        ┌────▼────┐       │
         │        │ AUTOGPT │◄──────┘
         │        │(Executor│
         │        │  Loop)  │
         │        └────┬────┘
         │             │
         └──────┬───────┘
                │
         ┌──────▼──────┐
         │ NEXUS RELAY │
         │  (Telegram) │
         └─────────────┘
```

## Layer Roles

| Layer | Repo | Role |
|-------|------|------|
| **Face** | OpenHuman | Desktop UI, memory tree, 118+ integrations |
| **Operator** | Mercury Agent | 24/7 daemon, Telegram bot, permission-hardened tools |
| **Evolution** | CORAL | Multi-agent self-improvement loop |
| **Strategy** | MetaGPT | Role-based reasoning, complex task decomposition |
| **Executor** | AutoGPT | Autonomous task execution loops |
| **Reporting** | Nexus Relay | Telegram status, all Primes report here |

## Deploy Order

### Step 1 — Mercury on Red Magic (RIGHT NOW)
One command in Termux. Already wired to your Telegram + Nexus Relay:
```bash
curl -fsSL https://raw.githubusercontent.com/kevinleestites2-dev/mercury-agent/main/redmagic_bootstrap.sh -o bootstrap.sh && bash bootstrap.sh
```

### Step 2 — CORAL Evolution Engine (GitHub Actions)
```bash
curl -fsSL https://raw.githubusercontent.com/Human-Agent-Society/CORAL/main/install.sh | sh
coral init pantheon-task
coral start -c pantheon-task/task.yaml
```

### Step 3 — MetaGPT + AutoGPT (GitHub Actions workflows in this repo)

### Step 4 — OpenHuman (when Nexus laptop is ready)
Download: https://tinyhumans.ai/openhuman

## Repos
- https://github.com/kevinleestites2-dev/mercury-agent
- https://github.com/kevinleestites2-dev/mercury-agent-skills
- https://github.com/kevinleestites2-dev/CORAL
- https://github.com/kevinleestites2-dev/MetaGPT
- https://github.com/kevinleestites2-dev/AutoGPT
- https://github.com/kevinleestites2-dev/openhuman
