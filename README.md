# r-stack

r-stack is a Claude Code–native template that bootstraps a complete, adaptable AI **agent team** for any project. Rather than shipping a fixed set of agents, it ships a *generic catalog* of roles plus a `/bootstrap` command: a Director-General interviews you to capture the product vision, assembles a small and effective team from the catalog, and then **specializes every agent — including itself —** to your specific project. The team runs lightweight SCRUM and follows a short set of disciplines: keep it simple, keep the end goal in mind, make surgical changes, and improve continuously.

## How it works

**Topology:** a **Director-General** (lead session, also Product Owner) coordinates **directors** (Agent Teams teammates), who spawn **specialists** (subagents) for scoped work. With the Agent Teams flag off, the same definitions run as subagents in **Solo mode**.

**The loop:**

```
/bootstrap → interview → VISION.md (gate ①) → roster (gate ②) → specialize every agent → seed backlog
    ↓
/sprint-plan → work → /status → /review (gate ③) → /retro → (repeat)
```

The specialization pass is the point: a bootstrapped r-stack is not generic — each agent is rewritten around your finalité, domain, users, and constraints.

## What's in the box

- **`catalog/`** — generic, editable role templates: the Director-General, base-trio directors (dev, design, marketing), and core specialists (backend, frontend, qa, code-reviewer, ui-ux, copywriter). It lives outside `.claude/agents/` so it is never auto-loaded as the active team.
- **`.claude/skills/`** — `karpathy` (the four disciplines), the meta-engine (`agent-designer`, `write-a-skill`, `self-improving-agent`, `skill-security-auditor`), and `impeccable` (design craft, guidance-only).
- **`.claude/commands/`** — `/bootstrap`, `/specialize`, and the SCRUM loop (`/sprint-plan`, `/status`, `/review`, `/retro`).
- **Durable memory** — `VISION.md`, `team/roster.md`, and `scrum/` (backlog, sprints, retros). Markdown is the source of truth; the Agent Teams task list is only a mirror.

## Prerequisites

- **Claude Code ≥ v2.1.178.**
- **Agent Teams (experimental)** — already enabled in `.claude/settings.json` via `CLAUDE_CODE_EXPERIMENTAL_AGENT_TEAMS=1`, with `teammateMode: in-process` (works on Windows). If the flag is off, r-stack degrades gracefully to **Solo mode** (specialists run as subagents from the lead session).
- **No runtime dependencies** — no Node.js, no Python. Everything is markdown + Claude-native.
- **Optional:** a `CONTEXT7_API_KEY` for higher Context7 documentation limits; the Anthropic `frontend-design` plugin for maximal design quality. See `docs/INTEGRATIONS.md`.

## Quickstart

1. Use this template (or clone the repo).
2. Open the folder in Claude Code.
3. Run `/bootstrap` and answer the Director-General's questions.

The DG writes your `VISION.md`, proposes a team roster, specializes each agent to your project, and seeds the SCRUM backlog. From there, run `/sprint-plan` to start delivering.

## More

- Design spec: `docs/superpowers/specs/2026-07-03-r-stack-design.md`
- Integrations & privacy: `docs/INTEGRATIONS.md`
- Build-time checks: `tests/lint.ps1`, `tests/CHECKLIST.md`
