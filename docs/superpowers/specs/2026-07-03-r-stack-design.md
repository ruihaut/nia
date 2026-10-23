# r-stack — Design Specification

- **Date:** 2026-07-03
- **Status:** Design approved in dialogue; pending written-spec review before planning.
- **Language note:** This repository's deliverables (agents, commands, docs, artifacts) are written in **English**. Working conversation with the maintainer happens in French.

---

## 1. Purpose

**r-stack** is a **Claude Code–native template repository** that bootstraps a complete, adaptable AI **agent team** for any software/product project.

You start a new project from this template, run `/bootstrap`, and a "general director" (DG) interviews you to capture the product vision. From that vision the DG assembles a right-sized team — directors and specialists selected from a catalog — **specializes every agent to the specific project**, and drives delivery with a lightweight SCRUM loop.

The differentiator versus generic template repos: **agents do not stay generic.** After the vision is understood, a *specialization pass* rewrites each selected agent (and the DG itself) into a project-specific version. The team is tailored, and keeps improving itself.

## 2. Goals & non-goals

**Goals**
- One template → one project repo (clone / "Use this template"), then `/bootstrap` tailors it in place.
- A hierarchical team: **DG → directors → specialists**, adaptable per project from a catalog.
- Every agent operates under a shared discipline (Karpathy principles + KISS + goal-focus + continuous improvement).
- Lightweight SCRUM with durable, git-versioned markdown artifacts.
- Maintainer stays in control via milestone gates; the team is autonomous between gates.

**Non-goals**
- Not a programmatic multi-agent SDK application.
- Not a plugin/marketplace package (the repo *is* the team).
- No heavy infrastructure (no build step, no external DB, no telemetry, no browser automation).
- No mandatory local runtime dependency (pure markdown + Claude-native + one optional MCP).

## 3. Core principles

Embedded in `CLAUDE.md` and inherited by every agent.

1. **Karpathy discipline** (source: `andrej-karpathy-skills`):
   - *Think Before Coding* — surface assumptions, ask for clarification.
   - *Simplicity First* — minimal, problem-focused solutions.
   - *Surgical Changes* — modify only what was requested.
   - *Goal-Driven Execution* — turn tasks into verifiable success criteria; loop until met.
2. **KISS** — keep it simple; reject "boil the ocean."
3. **Keep the end goal in mind** — every action traces back to the project's *finalité* (the `VISION.md` north star).
4. **Continuous improvement** — retros feed back into the product *and* into the agents themselves (`/specialize`).

## 4. Decisions (locked)

| Dimension | Decision |
|---|---|
| Substrate | Claude Code–native scaffold (`.claude/agents`, `.claude/commands`, `.claude/skills`, `CLAUDE.md`) |
| Reuse model | Template instantiated per project (copy → `/bootstrap` → in-place specialization) |
| Adaptability | Catalog of generic director/specialist templates; DG activates the relevant subset (+ ad hoc) |
| SCRUM depth | Pragmatic / lightweight (prioritized backlog, short sprints, review + retro) |
| SCRUM artifacts | **Markdown, versioned in the repo** |
| Language | **English** for all deliverables |
| Governance | **Milestone gates**: Vision sign-off · roster validation · sprint review |
| Topology | **Agent Teams hybrid**: DG = lead session · directors = teammates (own sessions) · specialists = subagents spawned by each director |
| PO / SM | DG holds the Product Owner function; SCRUM ceremony is codified in slash commands (no dedicated SM agent) |
| Design stack | **Max craft, zero local runtime**: frontend-design (plugin, baseline) + impeccable (vendored **guidance-only**) |
| Dev tooling | Context7 MCP (remote HTTP) as default for dev specialists |

## 5. Architecture / execution topology

The org hierarchy maps onto Claude Code's **Agent Teams** feature (experimental) plus subagents:

```
                          MAINTAINER (sponsor / "board")
                                 │  validates at milestones
                                 ▼
   ┌──────────────────────────────────────────────────────────┐
   │  DG — LEAD (main session)                                  │
   │  • vision keeper + Product Owner function (owns backlog)   │
   │  • runs the /bootstrap interview, holds milestone gates    │
   │  • spawns & coordinates directors                          │
   └───────────────┬───────────────┬──────────────┬────────────┘
                   │  SendMessage + shared task list (they talk to each other)
        ┌──────────▼───┐   ┌────────▼─────┐   ┌────▼──────────┐
        │ Dev Director │   │ Design Dir.  │   │ Marketing Dir.│   ← TEAMMATES
        │ (own session)│   │ (own session)│   │ (own session) │     (own context)
        └──────┬───────┘   └──────┬───────┘   └──────┬────────┘
               │ Task tool        │                  │
        ┌──────▼─────┐     ┌──────▼─────┐      ┌──────▼──────┐
        │ specialist │ …   │ specialist │      │ specialist  │   ← SUBAGENTS
        │ (backend)  │     │ (ui-ux)    │      │ (copywriter)│     (report to their director)
        └────────────┘     └────────────┘      └─────────────┘

  Durable memory (versioned in repo):
  VISION.md · team/roster.md · scrum/backlog.md · scrum/sprints/* · scrum/retros/*
  → the team is EPHEMERAL; it re-hydrates from these files every session
```

**Rationale & platform mapping**
- **DG = lead** because the lead is the only session that spawns/coordinates teammates and keeps a holistic view. It also carries the PO function.
- **Directors = teammates** (each its own Claude Code session/context) because they benefit from independent context and, unlike subagents, can **message each other and the DG** and share a task list — a real "management committee."
- **Specialists = subagents** because Agent Teams **forbids nested teams** (a teammate cannot spawn teammates), but a teammate **can** spawn subagents (foreground). Directors thus manage specialists as subagents that report back.

**Two runtime modes, one stable core**
- Stable core = catalog + `CLAUDE.md` + commands + skills.
- **Teams mode** (default, flag on): directors are teammates as above.
- **Solo mode** (graceful fallback if the experimental flag is unavailable): the DG orchestrates the *same* agent definitions as ordinary subagents. Nothing is rewritten.

**Milestone gates (maintainer):** ① sign off `VISION.md` · ② validate `team/roster.md` · ③ sprint review. Between gates the team runs autonomously.

## 6. Repository structure

```
r-stack/                          # the template; becomes the project repo after clone
├── VISION.md                     # ★ produced by the interview — the finalité / north star (read by all)
├── CLAUDE.md                     # STABLE: principles (Karpathy + KISS/goal/improvement),
│                                 #   team mechanics, SCRUM rules
│                                 #   + <!-- BEGIN/END GENERATED: DG PROFILE --> = the specialized DG
├── README.md
│
├── catalog/                      # GENERIC templates — the library (never mutated per project)
│   ├── director-general.md       #   source for the specialized DG block
│   ├── directors/                #   dev, design, marketing (default) + product, data, growth, ops, content (optional)
│   └── specialists/              #   backend, frontend, fullstack, qa, devops, code-reviewer,
│                                 #   adversarial-reviewer, ui-ux, design-system, copywriter, seo, ...
│
├── .claude/
│   ├── settings.json             # CLAUDE_CODE_EXPERIMENTAL_AGENT_TEAMS=1, teammateMode=in-process, permissions
│   ├── agents/                   # ACTIVE team — SPECIALIZED, generated by /bootstrap (empty in template)
│   ├── commands/                 # SCRUM process-as-code + lifecycle
│   │   ├── bootstrap.md · specialize.md
│   │   ├── sprint-plan.md · review.md · retro.md · status.md
│   └── skills/                   # vendored, self-contained skills (see §7)
│       ├── karpathy/ · agent-designer/ · write-a-skill/
│       ├── self-improving-agent/ · skill-security-auditor/
│       └── impeccable/           # guidance-only (SKILL.md + reference/; no scripts/)
│
├── .mcp.json                     # Context7 MCP (remote HTTP; key via env; anonymous fallback)
│
├── team/
│   └── roster.md                 # active agents for THIS project + justification (incl. deliberate exclusions)
│
├── scrum/
│   ├── backlog.md                # prioritized product backlog
│   ├── sprints/  → sprint-NN.md  # sprint goal + stories + owners + definition-of-done
│   └── retros/   → retro-NN.md    # improvement decisions (product AND team)
│
└── docs/
    ├── INTEGRATIONS.md           # optional plugins to install, MCP notes, privacy notes, prerequisites
    └── superpowers/specs/        # this design doc
```

**Two invariants**
- `catalog/` (generic) lives **outside** `.claude/agents/`, so Claude Code never loads generic templates as the active team. Only specialized agents in `.claude/agents/` are used.
- The generic↔specific boundary is **physical** (two directories) → the specialization pass is traceable in git and re-runnable.

## 7. Agent catalog, skills & integrations

### 7.1 Integration philosophy — three tiers (driven by license + KISS + self-containment)

| Tier | When | Examples | Location |
|---|---|---|---|
| **Vendored** (copied in) | Permissive license (MIT/Apache) + self-contained | karpathy, selected alireza skills, impeccable (guidance-only) | `.claude/skills/` (universal) or `catalog/` (role templates) |
| **Optional plugin** (referenced, installed on demand) | Proprietary or heavy; better tracked upstream | **frontend-design (Anthropic)** — proprietary, never vendored | documented in `docs/INTEGRATIONS.md` |
| **MCP** (external live service) | Real-time data | **Context7** | `.mcp.json` (key via env, optional) |

**Two non-negotiable guardrails** (we pull third-party code into a template):
- **License:** vendor only **MIT/Apache**, and **pin the source commit**. Proprietary (frontend-design) is **installed**, not copied.
- **Security:** every third-party skill passes through **`skill-security-auditor`** before adoption. This is a process step, not optional.

### 7.2 Catalog composition (seeds from explored sources)

| Role (catalog) | Seed source | Default? |
|---|---|---|
| **Directors** (teammates) | | |
| dev-director | alireza `senior-architect` / `startup-cto` | ✅ base trio |
| design-director | frontend-design + `product-strategist` | ✅ base trio |
| marketing-director | alireza `marketing-skill` (trimmed) | ✅ base trio |
| product / data / growth / ops / content-director | corresponding alireza personas | ⚪ optional (DG activates on need) |
| **Specialists** (subagents) | | |
| backend · frontend · fullstack · qa · devops | alireza `senior-*` role skills | via dev-director |
| code-reviewer · adversarial-reviewer | alireza | via dev-director |
| ui-ux · design-system | frontend-design + impeccable · `ui-design-system` | via design-director |
| copywriter · seo · content · growth-analyst | alireza marketing (trimmed) | via marketing-director |

> The DG holds the PO function → no product-director by default (activatable for backlog-heavy projects).

### 7.3 Skills wiring (who gets what)

- **Universal discipline (every agent, incl. DG):** **karpathy** (vendored) + the 4 principles written into `CLAUDE.md`. This is the guarantee that "every agent has Karpathy."
- **Meta engine (powers `/bootstrap` + `/specialize`):** `agent-designer` (how to write good agents) + `write-a-skill` + `self-improving-agent` (re-specialization = continuous improvement) + `skill-security-auditor` (the gate). Vendored. The specialization pass leans on proven methodology, not improvisation.
- **Dev (optional, for dev specialists):** `spec-driven-workflow`, `tdd-guide`, `focused-fix` — Karpathy-compatible reinforcements, activated for code-heavy projects.
- **SCRUM:** methodology from `scrum-master` / `agile-product-owner` is **absorbed into the commands** (`/sprint-plan`, `/review`, `/retro`) — no SM agent.
- **Design craft (max, zero runtime):** `frontend-design` (installed plugin, baseline aesthetic judgment) + `impeccable` **guidance-only** (vendored: `SKILL.md` + `reference/` only; `scripts/` dropped; Node `allowed-tools` neutralized in frontmatter). The `craft`/`critique`/`audit` commands become methodology the agent applies by hand.

### 7.4 Dev tooling — Context7

Default MCP in `.mcp.json` (remote HTTP variant; `CONTEXT7_API_KEY` via env expansion; anonymous fallback with lower limits). Dev specialists get always-current library docs via `resolve-library-id` → `query-docs` (triggered by "use context7"). Privacy note in `INTEGRATIONS.md`: queries go to a third party (mcp.context7.com / Upstash) — low sensitivity for public-library lookups.

### 7.5 Deliberately skipped (KISS filter — "not everything is worth taking")

- **gstack:** "Boil the Ocean" ethos, heavy infra (ML classifier, Playwright, Supabase memory, Conductor), Bun+TS build, telemetry, global install. We keep **only its interview patterns** (§8).
- **alireza:** bulk `c-level-advisor`, `finance`, `compliance`, oversized marketing, gimmicks (`caveman`, `roast`…), browser/network-automation skills.
- **ui-ux-pro-max:** full install (Python dependency + 47 KB SKILL.md + bloat). Skipped; its data (palettes/pairings) is cherry-pickable on demand only, not a default (avoids a second runtime and skill-stacking redundancy).

### 7.6 Attribution & licensing

| Source | License | Handling |
|---|---|---|
| andrej-karpathy-skills | *verify before verbatim vendoring* | Principles paraphrased into `CLAUDE.md`; vendor skill text only if license permits |
| alirezarezvani/claude-skills | MIT | Vendor selected skills; pin commit; retain MIT + author credit; convert persona frontmatter (`color/emoji/vibe` → `name/description/tools/model`) |
| pbakaus/impeccable | Apache-2.0 | Vendor guidance-only; retain NOTICE/attribution (Paul Bakaus) |
| anthropics frontend-design | Proprietary (© Anthropic) | Install via plugin only; never vendored |
| garrytan/gstack | MIT | Borrow patterns; credit Garry Tan |
| Context7 (Upstash) | external service | MCP reference only; no code vendored |

## 8. The `/bootstrap` flow

The DG (lead) runs six phases. Interview patterns are borrowed from gstack's `office-hours`; specialization uses the meta engine.

```
Phase 0 — PREFLIGHT
  Scan context; detect Teams flag (else Solo mode); detect an in-progress bootstrap
  (existing VISION.md/roster → resume, never overwrite).

Phase 1 — VISION INTERVIEW  (one question at a time)
  • Mode framing: greenfield "Startup" vs "Builder" (existing repo)
  • Forcing questions: what / for whom · problem (job-to-be-done) · FINALITÉ =
    what success looks like (measurable) · constraints (timeline, stack, budget) ·
    non-goals (KISS gate) · domain, vocabulary, tone/brand · risks
  • "push twice": on key answers, one follow-up to get past the polished first answer
  • premise-agreement: DG states 3–5 inferred premises → maintainer confirms/corrects
  • mandatory alternatives: minimal / ideal / creative framings, to sharpen the target

Phase 2 — VISION.md  ───────────────────────────────  ⛳ GATE ①: maintainer signs off Vision
  Synthesis: problem · users · finalité & success criteria · scope + non-goals ·
  constraints · domain/vocabulary/tone · risks. (Iterate until approved.)

Phase 3 — ROSTER  ──────────────────────────────────  ⛳ GATE ②: maintainer validates the team
  From the Vision, DG selects directors + specialists from catalog/, justifying each
  inclusion AND exclusion (small, effective team) → team/roster.md

Phase 4 — SPECIALIZATION PASS  (the differentiator)
  Using agent-designer/write-a-skill, DG rewrites each selected agent into a
  project-specific version in .claude/agents/ (finalité, domain, users, stack,
  success criteria, tone, anti-patterns, assigned skills/tools) + generates the
  specialized DG block in CLAUDE.md. skill-security-auditor vets any newly vendored
  third-party skill. Parallelizable (each specialization is independent). Commit.

Phase 5 — INITIAL BACKLOG
  DG (PO function) drafts scrum/backlog.md: prioritized epics/stories from the Vision
  (light; refined at first sprint planning).

Phase 6 — SPAWN & HANDOFF
  Teams mode: DG spawns the selected directors as teammates (referenced by their
  specialized agent name) + seeds the shared task list. Solo mode: same definitions
  as subagents. Ready for /sprint-plan.
```

**Flow principles**
- **Idempotent / resumable:** `/bootstrap` detects existing state and offers to continue — never a silent overwrite (Karpathy "surgical").
- **Two gates before any production** (Vision, Roster).
- **`/specialize` is reusable:** re-run Phase 4 on a single agent (e.g. from a retro decision) → the team improves itself.

## 9. SCRUM loop

```
/sprint-plan   DG (PO) + directors: sprint goal (a slice of the finalité),
               INVEST stories assigned → scrum/sprints/sprint-NN.md
               then seed the shared task list from those stories (Teams mode)
/… work …      Directors (teammates) claim tasks, spawn specialists (subagents),
               produce increments; message each other + escalate to DG on blockers
               (stop-gates); Karpathy discipline + "Search Before Building"
               (reuse/check existing work before writing anything new).
/status        DG holistic view: sprint + task list → progress summary (for maintainer)
/review        ⛳ GATE ③: demo increment vs goal+Vision (Karpathy verify loop),
               update scrum/backlog.md → maintainer validates end of sprint
/retro         product AND team improvements → scrum/retros/retro-NN.md (markdown,
               no telemetry). May trigger /specialize → the team improves itself.
```

No ceremonial `/standup`: teammates communicate continuously; `/status` suffices (KISS).

### 9.1 Task-list ↔ markdown reconciliation (key robustness rule)

**Rule: markdown is authoritative; the shared task list is a working mirror.**

| | `scrum/*.md` | shared task list (`~/.claude/tasks/`) |
|---|---|---|
| Nature | **Durable**, git-versioned | **Ephemeral**, live, in-session |
| Role | Source of truth | Real-time coordination |

- `/sprint-plan` writes **markdown first**, then seeds the task list.
- `/review` and `/status` **flush state back to markdown**.
- New session / `/resume`: teammates are gone (known limitation) → the DG **re-hydrates** from markdown, re-spawns directors, re-seeds the task list. **Nothing is lost.**

## 10. Robustness / error handling

- **Ephemeral team** → markdown re-hydration (§9.1).
- **Teams unavailable / flag off** → **Solo mode** (subagents), same definitions. Graceful degradation.
- **Task-status lag** (known Agent-Teams issue) → `/status` & `/review` reconcile against real artifacts; DG can correct manually.
- **Windows** → in-process mode (no split panes); documented. (Split panes need tmux/iTerm2, unsupported on Windows Terminal / VS Code.)
- **Token budget** → 3–5 directors max; specialists as subagents (summarized, cheaper); DG caps concurrent teammates.
- **Third-party skill risk** → `skill-security-auditor` gate + pinned commits + license discipline.
- **Idempotent commands** → `/bootstrap` & `/specialize` detect existing state; never silent overwrite.

## 11. Testing / verification

A template → "testing" means verifying the machinery loads and flows produce correct state. Kept light (KISS):

- **Smoke test:** scripted dry-run — `/bootstrap` on a fixture project (canned answers) → assert `VISION.md`, `roster.md`, `.claude/agents/*.md`, `backlog.md` are produced and well-formed + DG block present in `CLAUDE.md`.
- **Definition lint:** every agent (catalog + generated) has valid frontmatter; commands parse; each skill has a `SKILL.md`.
- **Karpathy guarantee:** `CLAUDE.md` embeds the 4 principles + every generated agent inherits them.
- **Degradation check:** Solo mode works with the flag disabled.
- **Tooling:** the repo's `verify` skill to run one real bootstrap on a throwaway sample and observe outputs. No heavy harness.

## 12. Prerequisites & dependencies

- **Claude Code ≥ v2.1.178** (Agent Teams no-setup behavior) with `CLAUDE_CODE_EXPERIMENTAL_AGENT_TEAMS=1` in `.claude/settings.json` (`env`). Feature is **experimental** and may change.
- **No local runtime dependency** (pure markdown + Claude-native). Node.js/Python explicitly avoided.
- **Optional:** a free Context7 API key (raises rate limits; anonymous works). The `frontend-design` plugin installed on demand.
- **Platform:** in-process teammate mode (works everywhere, incl. Windows).

## 13. Open items (resolve during implementation)

- Verify the license of `andrej-karpathy-skills` before vendoring text verbatim; otherwise paraphrase the 4 principles into `CLAUDE.md` (ideas are not copyrightable; wording may be).
- Confirm Context7 tool name at runtime (`query-docs` vs older `get-library-docs`).
- Pin exact source commits for every vendored third-party skill.
- Decide the exact initial catalog inventory to author in v1 vs defer (base trio + core specialists first).

## 14. Attribution

This design borrows patterns and/or code from: `andrej-karpathy-skills`, `alirezarezvani/claude-skills` (MIT), `pbakaus/impeccable` (Apache-2.0), `anthropics/claude-code` frontend-design (proprietary — referenced only), `garrytan/gstack` (MIT), and Context7 by Upstash. Respective licenses and attributions are retained where code is vendored (§7.6).
