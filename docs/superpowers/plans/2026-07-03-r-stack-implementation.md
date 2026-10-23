# r-stack Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build the r-stack template — a Claude Code–native repository that bootstraps an adaptable AI agent team (DG lead + director teammates + specialist subagents) with lightweight SCRUM and a per-project specialization pass.

**Architecture:** Pure markdown + Claude-native artifacts. The repo ships a *generic* `catalog/` of agent templates, a set of vendored/authored `.claude/skills/`, process-as-code `.claude/commands/`, and a principles-bearing `CLAUDE.md`. A `/bootstrap` command interviews the maintainer, writes `VISION.md`, selects a roster, then *specializes* each selected agent into `.claude/agents/`. Team runtime uses the experimental Agent Teams feature (directors = teammates), degrading gracefully to subagents.

**Tech Stack:** Markdown, YAML frontmatter, Claude Code (agents/commands/skills/settings), Agent Teams (experimental), Context7 MCP (remote HTTP, optional). PowerShell is used **only** for a build-time lint script — the template itself has no runtime dependency.

**Reference spec:** `docs/superpowers/specs/2026-07-03-r-stack-design.md` (authoritative; read it before executing).

## Global Constraints

Every task's requirements implicitly include this section. Values copied verbatim from the spec.

- **Language:** English for all deliverables (agents, commands, docs, artifacts).
- **Zero local runtime dependency:** no Node.js, no Python. Pure markdown + Claude-native + one optional MCP (Context7).
- **Licenses:** vendor only MIT/Apache and pin the source commit; proprietary `frontend-design` is *installed via plugin*, never vendored; run the security-audit checklist on any verbatim-vendored third-party skill.
- **Platform / feature floor:** Claude Code ≥ v2.1.178; `CLAUDE_CODE_EXPERIMENTAL_AGENT_TEAMS=1` in `.claude/settings.json`; teammate mode `in-process` (Windows-compatible).
- **Durable memory rule:** markdown artifacts are authoritative; the Agent Teams shared task list is an ephemeral working mirror.
- **Karpathy discipline in every agent:** Think Before Coding · Simplicity First · Surgical Changes · Goal-Driven Execution.
- **Catalog isolation:** `catalog/` (generic) lives OUTSIDE `.claude/agents/` so it is never auto-loaded as the active team.
- **Idempotent commands:** `/bootstrap` and `/specialize` detect existing state and never silently overwrite.
- **Commits:** conventional-commit subjects; every commit message ends with the trailer `Co-Authored-By: Claude Opus 4.8 <noreply@anthropic.com>`.
- **Prose-file note:** For prose-heavy files (command bodies, agent bodies), the structural spec in each task (frontmatter, sections, required behaviors, artifact names, gate points) is authoritative and complete; author the final English prose to fulfill it. Config/schema/small files give literal content that must be reproduced exactly.

---

## File Structure

**Create:**
- `CLAUDE.md` — principles + team mechanics + SCRUM rules + generated-DG-block markers.
- `VISION.md` — north-star template (filled by `/bootstrap`).
- `.mcp.json` — Context7 MCP.
- `.claude/settings.json` — Agent Teams flag, teammate mode, permissions.
- `.claude/agents/.gitkeep` — active team dir (empty; filled by bootstrap).
- `.claude/commands/{bootstrap,specialize,sprint-plan,review,retro,status}.md` — process-as-code.
- `.claude/skills/{karpathy,agent-designer,write-a-skill,self-improving-agent,skill-security-auditor}/SKILL.md` — authored skills.
- `.claude/skills/impeccable/` — vendored guidance-only (SKILL.md + reference/ + NOTICE).
- `catalog/_TEMPLATE.md` — shared agent-definition template + schema.
- `catalog/director-general.md` — generic DG template.
- `catalog/directors/{dev,design,marketing}-director.md` — base-trio directors.
- `catalog/specialists/{backend,frontend,qa,code-reviewer,ui-ux,copywriter}.md` — core specialists.
- `team/roster.md` — roster template.
- `scrum/backlog.md`, `scrum/sprints/.gitkeep`, `scrum/retros/.gitkeep` — SCRUM artifacts.
- `docs/INTEGRATIONS.md` — optional plugins, MCP notes, privacy, prerequisites.
- `tests/lint.ps1`, `tests/CHECKLIST.md` — build-time QA.

**Modify:**
- `README.md` — template overview, prerequisites, quickstart.

**v1 scope decision (resolves spec open item):** author base-trio directors + 6 core specialists only. Optional directors (product/data/growth/ops/content) and extra specialists are deferred — the catalog is extensible by design.

---

## Phase A — Skeleton & principles

### Task 1: Repo skeleton, settings, directories

**Files:**
- Create: `.claude/settings.json`
- Create: `.claude/agents/.gitkeep`, `scrum/sprints/.gitkeep`, `scrum/retros/.gitkeep`
- Modify: `README.md`

**Interfaces:**
- Produces: the `.claude/` machinery root and `settings.json` enabling Agent Teams + in-process mode, consumed by every later task and at runtime.

- [ ] **Step 1: Write the verification check**

Run: `Test-Path .claude/settings.json, .claude/agents, scrum/sprints, scrum/retros`
Expected: four `False` lines (nothing created yet).

- [ ] **Step 2: Create `.claude/settings.json` with exactly this content**

```json
{
  "env": {
    "CLAUDE_CODE_EXPERIMENTAL_AGENT_TEAMS": "1"
  },
  "teammateMode": "in-process",
  "permissions": {
    "allow": [
      "Read",
      "Edit",
      "Write",
      "Grep",
      "Glob"
    ],
    "deny": []
  }
}
```

- [ ] **Step 3: Create the directory keepers**

Create empty files: `.claude/agents/.gitkeep`, `scrum/sprints/.gitkeep`, `scrum/retros/.gitkeep`.

- [ ] **Step 4: Rewrite `README.md`**

Replace the two-line stub with: project name, one-paragraph purpose (a Claude Code template that bootstraps an adaptable agent team), a "Prerequisites" section (Claude Code ≥ v2.1.178; Agent Teams experimental flag already set in settings; no runtime deps; optional Context7 key; optional `frontend-design` plugin), and a "Quickstart" section (`1. Use this template / clone. 2. Open in Claude Code. 3. Run /bootstrap.`). Keep it under 60 lines.

- [ ] **Step 5: Run verification**

Run: `Test-Path .claude/settings.json; (Get-Content .claude/settings.json -Raw | Select-String 'CLAUDE_CODE_EXPERIMENTAL_AGENT_TEAMS') -ne $null`
Expected: `True` then `True`.

- [ ] **Step 6: Commit**

```bash
git add .claude/settings.json .claude/agents/.gitkeep scrum/sprints/.gitkeep scrum/retros/.gitkeep README.md
git commit -m "feat: scaffold repo skeleton and Claude Code settings"
```

---

### Task 2: `CLAUDE.md` — principles, team mechanics, SCRUM rules

**Files:**
- Create: `CLAUDE.md`

**Interfaces:**
- Produces: the always-loaded project instructions. Must contain the 4 Karpathy principle anchors, the KISS/finalité/continuous-improvement principles, the team topology summary, the SCRUM rules, and the exact markers `<!-- BEGIN GENERATED: DG PROFILE -->` / `<!-- END GENERATED: DG PROFILE -->` (consumed by `/bootstrap` Phase 4 and `/specialize`).

- [ ] **Step 1: Write the verification check**

Run: `Test-Path CLAUDE.md`
Expected: `False`.

- [ ] **Step 2: Author `CLAUDE.md`** with these required sections (English prose fulfilling this structure):

1. `# r-stack — Operating Manual` intro (1 paragraph).
2. `## Principles` — a subsection listing verbatim the four anchors **Think Before Coding**, **Simplicity First**, **Surgical Changes**, **Goal-Driven Execution** (one line each), then **KISS**, **Keep the end goal in mind** (points to `VISION.md`), **Continuous improvement** (retros feed product + agents).
3. `## How this team works` — the topology: DG = lead (also PO); directors = Agent Teams teammates; specialists = subagents spawned by directors; graceful fallback to Solo (subagent) mode when the experimental flag is off. State the durable-memory rule (markdown authoritative; task list is a mirror; re-hydrate on new session).
4. `## SCRUM rules` — pragmatic loop: `/sprint-plan → work → /status → /review (gate) → /retro`; no ceremonial standup; milestone gates ① Vision ② roster ③ sprint review.
5. `## Project profile` — containing exactly:

```markdown
<!-- BEGIN GENERATED: DG PROFILE -->
_Not yet bootstrapped. Run `/bootstrap` to specialize the Director-General for this project._
<!-- END GENERATED: DG PROFILE -->
```

- [ ] **Step 3: Run verification**

Run:
```powershell
$c = Get-Content CLAUDE.md -Raw
'Think Before Coding','Simplicity First','Surgical Changes','Goal-Driven','BEGIN GENERATED: DG PROFILE','END GENERATED: DG PROFILE' | ForEach-Object { "$_ => " + ($c -match [regex]::Escape($_)) }
```
Expected: six lines each ending `=> True`.

- [ ] **Step 4: Commit**

```bash
git add CLAUDE.md
git commit -m "feat: add CLAUDE.md with principles, team mechanics, and SCRUM rules"
```

---

## Phase B — Durable-memory templates & integrations

### Task 3: Durable-memory templates (VISION, roster, backlog)

**Files:**
- Create: `VISION.md`, `team/roster.md`, `scrum/backlog.md`

**Interfaces:**
- Produces: the artifact skeletons `/bootstrap` and the SCRUM commands fill in. Section headings below are the contract those commands write against.

- [ ] **Step 1: Verify absence**

Run: `Test-Path VISION.md, team/roster.md, scrum/backlog.md`
Expected: three `False`.

- [ ] **Step 2: Create `VISION.md`** with these exact headings (content = a one-line italic placeholder under each, to be filled by `/bootstrap`):

```markdown
# Vision — <project name>

> Status: template. `/bootstrap` fills this in and you sign it off (gate ①).

## Problem
_What problem, for whom (target users)._

## Finalité (definition of success)
_Measurable success criteria. The one thing that must be true._

## Scope
_In scope._

## Non-goals
_Explicitly out of scope (KISS)._

## Constraints
_Timeline, stack, budget, platform, existing assets._

## Domain & vocabulary
_Key domain terms and tone/brand._

## Risks
_Known risks and unknowns._
```

- [ ] **Step 3: Create `team/roster.md`** with:

```markdown
# Team roster

> Status: template. `/bootstrap` fills this in and you validate it (gate ②).

## Active directors
_Name · why activated._

## Active specialists (by director)
_Director → specialists · why._

## Deliberately excluded
_Catalog roles NOT activated for this project · why (small, effective team)._
```

- [ ] **Step 4: Create `scrum/backlog.md`** with:

```markdown
# Product backlog

> Prioritized top-to-bottom. Owned by the DG (Product Owner function).

| # | Item | Priority | Status | Notes |
|---|------|----------|--------|-------|
| _—_ | _seeded by /bootstrap; refined at /sprint-plan_ | | | |
```

- [ ] **Step 5: Verify**

Run: `Select-String -Path VISION.md -Pattern 'Finalité'; Select-String -Path team/roster.md -Pattern 'Deliberately excluded'; Select-String -Path scrum/backlog.md -Pattern 'Product backlog'`
Expected: one match line for each file.

- [ ] **Step 6: Commit**

```bash
git add VISION.md team/roster.md scrum/backlog.md
git commit -m "feat: add durable-memory artifact templates (vision, roster, backlog)"
```

---

### Task 4: Context7 MCP + INTEGRATIONS doc

**Files:**
- Create: `.mcp.json`, `docs/INTEGRATIONS.md`

**Interfaces:**
- Produces: `.mcp.json` registering Context7 (consumed by dev specialists at runtime). `INTEGRATIONS.md` documents optional installs + privacy + prerequisites.

- [ ] **Step 1: Verify absence**

Run: `Test-Path .mcp.json, docs/INTEGRATIONS.md`
Expected: two `False`.

- [ ] **Step 2: Create `.mcp.json` with exactly this content**

```json
{
  "mcpServers": {
    "context7": {
      "url": "https://mcp.context7.com/mcp",
      "headers": {
        "CONTEXT7_API_KEY": "${CONTEXT7_API_KEY}"
      }
    }
  }
}
```

- [ ] **Step 3: Create `docs/INTEGRATIONS.md`** covering (English prose):
  - **Context7 (default MCP):** what it is; usage (`resolve-library-id` → `query-docs`, trigger "use context7"); the API key is optional (anonymous works, key raises limits) and read from the `CONTEXT7_API_KEY` env var; **privacy note** that queries go to a third party (mcp.context7.com / Upstash).
  - **frontend-design (optional plugin, proprietary — do not vendor):** install with `/plugin marketplace add anthropics/claude-code` then `/plugin install frontend-design@claude-code-plugins`.
  - **impeccable (vendored, guidance-only):** already in `.claude/skills/impeccable/`; Apache-2.0 (see NOTICE); Node scripts intentionally omitted.
  - **Prerequisites:** Claude Code ≥ v2.1.178; Agent Teams flag set in settings; in-process teammate mode on Windows; no runtime deps.

- [ ] **Step 4: Verify**

Run: `Get-Content .mcp.json -Raw | Select-String 'mcp.context7.com'; Select-String -Path docs/INTEGRATIONS.md -Pattern 'frontend-design@claude-code-plugins'`
Expected: one match each.

- [ ] **Step 5: Commit**

```bash
git add .mcp.json docs/INTEGRATIONS.md
git commit -m "feat: add Context7 MCP and integrations documentation"
```

---

## Phase C — Skills

### Task 5: Karpathy discipline skill

**Files:**
- Create: `.claude/skills/karpathy/SKILL.md`

**Interfaces:**
- Produces: a user- and agent-loadable skill encoding the 4 principles. Referenced by `CLAUDE.md` and every specialized agent.

- [ ] **Step 1: Verify absence**

Run: `Test-Path .claude/skills/karpathy/SKILL.md`
Expected: `False`.

- [ ] **Step 2: Author the skill.** Frontmatter (exact):

```markdown
---
name: karpathy
description: Use before and during any build task — the four disciplines (Think Before Coding, Simplicity First, Surgical Changes, Goal-Driven Execution) that keep agents honest, minimal, and goal-locked.
---
```

Body (English prose, original paraphrase — not verbatim upstream): one short section per principle with a concrete "do / avoid" bullet pair, plus a closing "Verification loop" paragraph (turn the task into checkable success criteria; loop until met). Keep under ~120 lines. Credit the inspiration (andrej-karpathy-skills) in one line at the bottom.

- [ ] **Step 3: Verify**

Run:
```powershell
$c = Get-Content .claude/skills/karpathy/SKILL.md -Raw
($c -match '(?s)^---.*name:\s*karpathy.*description:.*---') ; 'Think Before Coding','Simplicity First','Surgical Changes','Goal-Driven' | %{ $c -match [regex]::Escape($_) }
```
Expected: `True` then four `True`.

- [ ] **Step 4: Commit**

```bash
git add .claude/skills/karpathy/SKILL.md
git commit -m "feat: add karpathy discipline skill"
```

---

### Task 6: Meta-engine skills (agent-designer, write-a-skill, self-improving-agent, skill-security-auditor)

**Files:**
- Create: `.claude/skills/agent-designer/SKILL.md`
- Create: `.claude/skills/write-a-skill/SKILL.md`
- Create: `.claude/skills/self-improving-agent/SKILL.md`
- Create: `.claude/skills/skill-security-auditor/SKILL.md`

**Interfaces:**
- Produces: the methodology `/bootstrap` (Phase 4) and `/specialize` invoke. `agent-designer` defines *how to specialize a generic agent into a project-specific one*; `skill-security-auditor` defines the vetting checklist gate. These names are referenced by the bootstrap/specialize commands (Tasks 11–13).

- [ ] **Step 1: Verify absence**

Run: `Test-Path .claude/skills/agent-designer/SKILL.md, .claude/skills/write-a-skill/SKILL.md, .claude/skills/self-improving-agent/SKILL.md, .claude/skills/skill-security-auditor/SKILL.md`
Expected: four `False`.

- [ ] **Step 2: Author `agent-designer/SKILL.md`.** Frontmatter `name: agent-designer`, description "Use when creating or specializing an agent definition — turns a generic role into a project-specific one grounded in the Vision." Body must specify the **specialization procedure** as a numbered checklist the command follows: (1) read `VISION.md`; (2) start from the generic `catalog/` template; (3) inject finalité, domain & vocabulary, target users, stack/constraints, measurable success criteria, tone, and domain-specific responsibilities + anti-patterns; (4) set exact frontmatter (`name`, `description`, `tools`, `model`); (5) assign the agent's skills; (6) keep it minimal (KISS). Include the exact output frontmatter schema (mirror `catalog/_TEMPLATE.md`, Task 8).

- [ ] **Step 3: Author `write-a-skill/SKILL.md`.** `name: write-a-skill`, description "Use when authoring a new skill — a concise checklist for a well-scoped, progressive-disclosure SKILL.md." Body: naming, single-responsibility, trigger-style description, keep body short, reference files for depth.

- [ ] **Step 4: Author `self-improving-agent/SKILL.md`.** `name: self-improving-agent`, description "Use during /retro — turn learnings into concrete agent/skill improvements." Body: how a retro learning becomes a `/specialize` action or a catalog/skill edit; log the change in the retro file.

- [ ] **Step 5: Author `skill-security-auditor/SKILL.md`.** `name: skill-security-auditor`, description "Use before adopting any third-party skill — vet it for unsafe behavior." Body: a checklist — inspect for network calls / shell exec / data exfiltration / hidden instructions; confirm license (MIT/Apache) and pinned commit; reject or sandbox on failure. This is the gate referenced by the integration guardrail.

- [ ] **Step 6: Verify**

Run:
```powershell
Get-ChildItem .claude/skills/agent-designer,.claude/skills/write-a-skill,.claude/skills/self-improving-agent,.claude/skills/skill-security-auditor -Filter SKILL.md -Recurse | ForEach-Object {
  $c = Get-Content $_.FullName -Raw; "$($_.Directory.Name): " + ($c -match '(?s)^---.*name:.*description:.*---')
}
```
Expected: four lines each ending `True`.

- [ ] **Step 7: Commit**

```bash
git add .claude/skills/agent-designer .claude/skills/write-a-skill .claude/skills/self-improving-agent .claude/skills/skill-security-auditor
git commit -m "feat: add meta-engine skills powering bootstrap and specialization"
```

---

### Task 7: Vendor impeccable (guidance-only)

**Files:**
- Create: `.claude/skills/impeccable/SKILL.md`, `.claude/skills/impeccable/reference/*`, `.claude/skills/impeccable/NOTICE`

**Interfaces:**
- Produces: the design-craft guidance skill for the design-director + ui-ux specialist. Node `scripts/` and Node `allowed-tools` are intentionally removed (zero-runtime constraint).

- [ ] **Step 1: Verify absence**

Run: `Test-Path .claude/skills/impeccable/SKILL.md`
Expected: `False`.

- [ ] **Step 2: Fetch upstream at a pinned commit.** Use WebFetch on `https://github.com/pbakaus/impeccable` to resolve the latest release commit SHA; record it. Fetch `SKILL.md` and the `reference/*.md` files via `https://raw.githubusercontent.com/pbakaus/impeccable/<SHA>/.claude/skills/impeccable/<path>`.
  - **Fallback if fetch fails:** create `.claude/skills/impeccable/SKILL.md` with valid frontmatter (`name: impeccable`, description about distinctive, anti-slop UI craft) and a body noting "guidance vendored manually pending — see source", and add a task note. Do not block the build.

- [ ] **Step 3: Strip runtime coupling.** In the vendored `SKILL.md` frontmatter, remove any `allowed-tools` entries referencing `npx impeccable` or `node .../scripts/*`. Do not copy the `scripts/` directory. Keep `SKILL.md` + `reference/` only. Rewrite any "run `/impeccable <cmd>`" phrasing to "apply the <cmd> method manually".

- [ ] **Step 4: Add attribution.** Create `.claude/skills/impeccable/NOTICE` crediting Paul Bakaus, Apache-2.0, source URL + pinned SHA.

- [ ] **Step 5: Run the security-audit gate.** Apply the `skill-security-auditor` checklist to the vendored content; confirm no network/shell exec remains. Record the result in the commit body.

- [ ] **Step 6: Verify**

Run: `Test-Path .claude/skills/impeccable/SKILL.md, .claude/skills/impeccable/NOTICE; (Get-Content .claude/skills/impeccable/SKILL.md -Raw | Select-String 'npx impeccable') -eq $null`
Expected: `True`, `True`, then `True` (no npx reference remains).

- [ ] **Step 7: Commit**

```bash
git add .claude/skills/impeccable
git commit -m "feat: vendor impeccable design skill (guidance-only, Apache-2.0)"
```

---

## Phase D — Catalog

### Task 8: Agent-definition template + Director-General template

**Files:**
- Create: `catalog/_TEMPLATE.md`, `catalog/director-general.md`

**Interfaces:**
- Produces: `catalog/_TEMPLATE.md` — the canonical frontmatter schema + body structure every catalog agent and every specialized agent follows. `catalog/director-general.md` — the generic DG source specialized into the `CLAUDE.md` DG PROFILE block.

- [ ] **Step 1: Verify absence**

Run: `Test-Path catalog/_TEMPLATE.md, catalog/director-general.md`
Expected: two `False`.

- [ ] **Step 2: Create `catalog/_TEMPLATE.md` with exactly this content**

```markdown
---
name: <kebab-case-role>
description: <one line — when to use this agent (trigger style)>
tools: Read, Grep, Glob, Edit, Write
model: inherit
---

# <Role title>

## Mission
<One sentence tying this role to the project finalité.>

## Responsibilities
- <bullet>

## How this role works here
<Project-specific context injected during specialization: domain, users, stack, tone.>

## Skills
- karpathy (always)
- <role-specific skills>

## Anti-patterns (avoid)
- <bullet>

## Definition of done
- <verifiable criteria — Goal-Driven>
```

- [ ] **Step 3: Create `catalog/director-general.md`.** Use the template. `name: director-general`, description "The DG — vision keeper, Product Owner function, holistic coordinator; specialized into CLAUDE.md." `tools: Read, Grep, Glob, Edit, Write`. Body specifies: owns `VISION.md` and backlog priorities; runs milestone gates; spawns/coordinates directors; keeps the holistic view; enforces KISS + finalité. Note that on specialization its body is written into the `CLAUDE.md` DG PROFILE block (it is the one catalog entry whose target is `CLAUDE.md`, not `.claude/agents/`).

- [ ] **Step 4: Verify**

Run:
```powershell
(Get-Content catalog/_TEMPLATE.md -Raw) -match '(?s)name:.*description:.*tools:.*model:'
(Get-Content catalog/director-general.md -Raw | Select-String 'director-general') -ne $null
```
Expected: `True` then `True`.

- [ ] **Step 5: Commit**

```bash
git add catalog/_TEMPLATE.md catalog/director-general.md
git commit -m "feat: add agent template schema and director-general template"
```

---

### Task 9: Base-trio directors

**Files:**
- Create: `catalog/directors/dev-director.md`, `catalog/directors/design-director.md`, `catalog/directors/marketing-director.md`

**Interfaces:**
- Consumes: `catalog/_TEMPLATE.md` structure.
- Produces: three generic director templates selectable by `/bootstrap`. Each is spawned as a *teammate* in Teams mode.

- [ ] **Step 1: Verify absence**

Run: `Test-Path catalog/directors/dev-director.md, catalog/directors/design-director.md, catalog/directors/marketing-director.md`
Expected: three `False`.

- [ ] **Step 2: Create `dev-director.md`** (full exemplar). Using the template: `name: dev-director`, description "Owns technical delivery — architecture, engineering plan, and coordinating dev specialists." `tools: Read, Grep, Glob, Edit, Write`. Responsibilities: translate Vision into a technical plan; break work into stories with the DG; spawn and coordinate dev specialists (backend, frontend, qa, code-reviewer) as subagents; uphold "Search Before Building"; escalate blockers to the DG. Skills: karpathy, spec-driven-workflow (when code-heavy). Anti-patterns: over-engineering, scope creep, editing beyond the story. DoD: increment meets the sprint goal and passes review.

- [ ] **Step 3: Create `design-director.md`.** `name: design-director`, description "Owns product design & UX direction and coordinates the ui-ux specialist." Distinctive content: sets aesthetic direction grounded in the Vision (uses `frontend-design` plugin if installed + `impeccable` guidance); brand vs product register; coordinates the ui-ux + design-system specialists. Skills: karpathy, impeccable. Anti-patterns: generic/templated UI, decoration over meaning.

- [ ] **Step 4: Create `marketing-director.md`.** `name: marketing-director`, description "Owns positioning, messaging, and go-to-market; coordinates copywriter/SEO specialists." Distinctive content: derives positioning from the finalité and target users; owns messaging; coordinates copywriter + (optional) seo. Skills: karpathy. Anti-patterns: hype disconnected from the product, vanity metrics.

- [ ] **Step 5: Verify**

Run:
```powershell
Get-ChildItem catalog/directors -Filter *.md | ForEach-Object {
  $c = Get-Content $_.FullName -Raw
  "$($_.Name): " + (($c -match '(?s)^---.*name:.*description:.*tools:.*model:.*---') -and ($c -match 'karpathy'))
}
```
Expected: three lines each ending `True`.

- [ ] **Step 6: Commit**

```bash
git add catalog/directors
git commit -m "feat: add base-trio director templates (dev, design, marketing)"
```

---

### Task 10: Core specialists

**Files:**
- Create: `catalog/specialists/{backend,frontend,qa,code-reviewer,ui-ux,copywriter}.md`

**Interfaces:**
- Consumes: `catalog/_TEMPLATE.md`.
- Produces: six generic specialist templates. Spawned as *subagents* by their director.

- [ ] **Step 1: Verify absence**

Run: `Test-Path catalog/specialists/backend.md, catalog/specialists/frontend.md, catalog/specialists/qa.md, catalog/specialists/code-reviewer.md, catalog/specialists/ui-ux.md, catalog/specialists/copywriter.md`
Expected: six `False`.

- [ ] **Step 2: Create `backend.md`** (full exemplar). `name: backend`, description "Implements server-side/data logic for a scoped story." `tools: Read, Grep, Glob, Edit, Write`. Responsibilities: implement the assigned story only (Surgical); use `context7` for current library docs; write/adjust tests; report back to the dev-director. Skills: karpathy, tdd-guide (when code-heavy). Anti-patterns: touching unrelated files, speculative abstraction. DoD: story's acceptance criteria met, tests green.

- [ ] **Step 3: Create the other five** using the template with these distinctive values:
  - `frontend.md` — `name: frontend`, desc "Implements client-side UI for a scoped story"; uses `context7`; collaborates with ui-ux for design intent; skills karpathy, tdd-guide.
  - `qa.md` — `name: qa`, desc "Designs and runs tests, finds defects for a scoped story"; skills karpathy; focus on verifiable success criteria.
  - `code-reviewer.md` — `name: code-reviewer`, desc "Reviews a diff for correctness and simplicity"; skills karpathy; anti-pattern: rubber-stamping.
  - `ui-ux.md` — `name: ui-ux`, desc "Executes UI/UX craft for a scoped story"; skills karpathy, impeccable; applies impeccable methods manually + frontend-design direction; anti-pattern: AI-slop patterns.
  - `copywriter.md` — `name: copywriter`, desc "Writes product/marketing copy in the project voice"; skills karpathy; grounds copy in the Vision tone.

- [ ] **Step 4: Verify**

Run:
```powershell
Get-ChildItem catalog/specialists -Filter *.md | ForEach-Object {
  $c = Get-Content $_.FullName -Raw
  "$($_.Name): " + (($c -match '(?s)^---.*name:.*description:.*---') -and ($c -match 'karpathy'))
}
```
Expected: six lines each ending `True`.

- [ ] **Step 5: Commit**

```bash
git add catalog/specialists
git commit -m "feat: add core specialist templates"
```

---

## Phase E — Commands (process-as-code)

### Task 11: `/bootstrap` command

**Files:**
- Create: `.claude/commands/bootstrap.md`

**Interfaces:**
- Consumes: `catalog/*`, the meta-engine skills (`agent-designer`, `skill-security-auditor`), `CLAUDE.md` DG markers, and the artifact templates.
- Produces: on completion — a filled `VISION.md`, `team/roster.md`, specialized files in `.claude/agents/`, a specialized `CLAUDE.md` DG PROFILE block, a seeded `scrum/backlog.md`, and (Teams mode) spawned director teammates.

- [ ] **Step 1: Verify absence**

Run: `Test-Path .claude/commands/bootstrap.md`
Expected: `False`.

- [ ] **Step 2: Author `bootstrap.md`.** Frontmatter: `description: Interview the maintainer, capture the vision, assemble and specialize the team.` Body must encode the 6 phases from the spec §8 as explicit instructions to the DG:
  - **Phase 0 Preflight:** scan context; check the Agent Teams flag (else announce Solo mode); if `VISION.md`/`team/roster.md` already contain non-template content, STOP and offer to resume — never overwrite (idempotency).
  - **Phase 1 Interview:** ask questions ONE at a time via `AskUserQuestion`; cover what/for-whom, problem, finalité (measurable), constraints, non-goals, domain/vocabulary/tone, risks; apply "push twice" on key answers; state 3–5 premises for confirmation; offer minimal/ideal/creative alternatives.
  - **Phase 2 VISION.md → GATE ①:** write `VISION.md`; require explicit maintainer sign-off; iterate.
  - **Phase 3 Roster → GATE ②:** select directors + specialists from `catalog/`, justify inclusions AND exclusions; write `team/roster.md`; require validation.
  - **Phase 4 Specialization:** invoke `agent-designer` methodology to rewrite each selected agent into `.claude/agents/<name>.md`; write the DG body into the `CLAUDE.md` DG PROFILE block between the markers; run `skill-security-auditor` on any newly vendored skill; commit.
  - **Phase 5 Backlog:** seed `scrum/backlog.md` from the Vision.
  - **Phase 6 Spawn:** Teams mode — spawn selected directors as teammates referenced by their specialized agent name, seed the shared task list; Solo mode — note the same definitions will be used as subagents. Hand off to `/sprint-plan`.

- [ ] **Step 3: Verify**

Run:
```powershell
$c = Get-Content .claude/commands/bootstrap.md -Raw
'Phase 0','Phase 1','GATE','agent-designer','DG PROFILE','AskUserQuestion' | ForEach-Object { "$_ => " + ($c -match [regex]::Escape($_)) }
```
Expected: six lines each ending `True`.

- [ ] **Step 4: Commit**

```bash
git add .claude/commands/bootstrap.md
git commit -m "feat: add /bootstrap command (interview, vision, roster, specialization)"
```

---

### Task 12: `/specialize` command

**Files:**
- Create: `.claude/commands/specialize.md`

**Interfaces:**
- Consumes: `agent-designer` skill, `VISION.md`, `catalog/*`, existing `.claude/agents/*`.
- Produces: a re-specialized agent file (or the DG PROFILE block). Argument: an agent name (or `all`).

- [ ] **Step 1: Verify absence** — Run: `Test-Path .claude/commands/specialize.md` → `False`.

- [ ] **Step 2: Author `specialize.md`.** `description: Re-specialize one agent (or all) from the current Vision — used for continuous improvement.` Body: takes an agent name argument; reads `VISION.md` + the generic `catalog/` source + current retro learnings; applies `agent-designer`; rewrites the target in `.claude/agents/` (or the DG PROFILE block for `director-general`); shows a diff and requires confirmation before overwrite (idempotent, surgical); commits.

- [ ] **Step 3: Verify** — Run: `Get-Content .claude/commands/specialize.md -Raw | Select-String 'agent-designer','director-general'` → two matches.

- [ ] **Step 4: Commit**

```bash
git add .claude/commands/specialize.md
git commit -m "feat: add /specialize command for continuous agent improvement"
```

---

### Task 13: SCRUM commands (`/sprint-plan`, `/review`, `/retro`, `/status`)

**Files:**
- Create: `.claude/commands/sprint-plan.md`, `.claude/commands/review.md`, `.claude/commands/retro.md`, `.claude/commands/status.md`

**Interfaces:**
- Consumes: `scrum/backlog.md`, `VISION.md`, the roster, the shared task list.
- Produces: `scrum/sprints/sprint-NN.md`, updated backlog, `scrum/retros/retro-NN.md`; enforces the markdown-authoritative rule.

- [ ] **Step 1: Verify absence** — Run: `Test-Path .claude/commands/sprint-plan.md, .claude/commands/review.md, .claude/commands/retro.md, .claude/commands/status.md` → four `False`.

- [ ] **Step 2: Author `sprint-plan.md`.** `description: Plan a sprint — set the goal, select and assign INVEST stories.` Body: DG (PO) + directors pull top backlog items; define a sprint goal (a slice of the finalité); write INVEST stories with owners + definition-of-done to `scrum/sprints/sprint-NN.md` (markdown FIRST); then seed the shared task list from those stories (Teams mode).

- [ ] **Step 3: Author `status.md`.** `description: Holistic progress snapshot.` Body: read the current sprint file + shared task-list state; summarize progress for the maintainer; flag lagging/stale task statuses (reconcile against artifacts).

- [ ] **Step 4: Author `review.md`.** `description: Sprint review — demo the increment vs goal and Vision (gate ③).` Body: verify the increment against the sprint goal + `VISION.md` (Goal-Driven verify loop); update `scrum/backlog.md` (done + newly discovered items); flush live state back to markdown; require maintainer validation.

- [ ] **Step 5: Author `retro.md`.** `description: Retrospective — capture improvements for product AND team.` Body: what went well / to improve; write to `scrum/retros/retro-NN.md` (plain markdown, no telemetry); for team/agent improvements, invoke `self-improving-agent` and optionally trigger `/specialize`.

- [ ] **Step 6: Verify**

Run:
```powershell
Get-ChildItem .claude/commands -Filter *.md | Where-Object { $_.Name -in 'sprint-plan.md','review.md','retro.md','status.md' } | ForEach-Object {
  "$($_.Name): " + ((Get-Content $_.FullName -Raw) -match '(?s)^---.*description:.*---')
}
```
Expected: four lines each ending `True`.

- [ ] **Step 7: Commit**

```bash
git add .claude/commands/sprint-plan.md .claude/commands/review.md .claude/commands/retro.md .claude/commands/status.md
git commit -m "feat: add SCRUM loop commands (sprint-plan, status, review, retro)"
```

---

## Phase F — QA & finalize

### Task 14: Lint script + smoke-test checklist

**Files:**
- Create: `tests/lint.ps1`, `tests/CHECKLIST.md`

**Interfaces:**
- Consumes: the whole repo.
- Produces: an automated structural/frontmatter check + a manual smoke-test procedure.

- [ ] **Step 1: Verify absence** — Run: `Test-Path tests/lint.ps1, tests/CHECKLIST.md` → two `False`.

- [ ] **Step 2: Create `tests/lint.ps1` with exactly this content**

```powershell
# tests/lint.ps1 — build-time structural + frontmatter lint (dependency-free).
$ErrorActionPreference = 'Stop'
$root = Split-Path -Parent $PSScriptRoot
$fail = @()

$required = @(
  'CLAUDE.md','VISION.md','README.md','.mcp.json','.claude/settings.json',
  '.claude/commands/bootstrap.md','.claude/commands/specialize.md',
  '.claude/commands/sprint-plan.md','.claude/commands/review.md',
  '.claude/commands/retro.md','.claude/commands/status.md',
  'team/roster.md','scrum/backlog.md',
  'catalog/_TEMPLATE.md','catalog/director-general.md',
  'catalog/directors/dev-director.md','catalog/directors/design-director.md','catalog/directors/marketing-director.md',
  'catalog/specialists/backend.md','catalog/specialists/frontend.md','catalog/specialists/qa.md',
  'catalog/specialists/code-reviewer.md','catalog/specialists/ui-ux.md','catalog/specialists/copywriter.md',
  '.claude/skills/karpathy/SKILL.md','.claude/skills/agent-designer/SKILL.md',
  '.claude/skills/write-a-skill/SKILL.md','.claude/skills/self-improving-agent/SKILL.md',
  '.claude/skills/skill-security-auditor/SKILL.md','.claude/skills/impeccable/SKILL.md'
)
foreach ($f in $required) { if (-not (Test-Path (Join-Path $root $f))) { $fail += "MISSING: $f" } }

$fmFiles = @()
$fmFiles += Get-ChildItem (Join-Path $root 'catalog') -Recurse -Filter *.md -ErrorAction SilentlyContinue | Where-Object { $_.Name -notlike '_*' }
$fmFiles += Get-ChildItem (Join-Path $root '.claude/commands') -Filter *.md -ErrorAction SilentlyContinue
$fmFiles += Get-ChildItem (Join-Path $root '.claude/skills') -Recurse -Filter SKILL.md -ErrorAction SilentlyContinue
foreach ($file in $fmFiles) {
  $c = Get-Content -Raw $file.FullName
  if ($c -notmatch '(?s)^\s*---.*?\bname:\s*\S+.*?\bdescription:\s*\S+.*?---' -and
      $c -notmatch '(?s)^\s*---.*?\bdescription:\s*\S+.*?---') {
    $fail += "BAD FRONTMATTER: $($file.FullName.Substring($root.Length+1))"
  }
}

$claude = Get-Content -Raw (Join-Path $root 'CLAUDE.md')
foreach ($a in @('Think Before Coding','Simplicity First','Surgical Changes','Goal-Driven','BEGIN GENERATED: DG PROFILE','END GENERATED: DG PROFILE')) {
  if ($claude -notmatch [regex]::Escape($a)) { $fail += "CLAUDE.md missing: $a" }
}

if ($fail.Count) { $fail | ForEach-Object { Write-Host "FAIL: $_" }; exit 1 }
Write-Host "LINT OK"; exit 0
```

- [ ] **Step 3: Create `tests/CHECKLIST.md`** — a manual smoke-test procedure: (1) run `pwsh tests/lint.ps1` → `LINT OK`; (2) in Claude Code, run `/bootstrap` with canned answers for a throwaway sample; (3) assert `VISION.md` filled, `team/roster.md` filled, `.claude/agents/*.md` created, `CLAUDE.md` DG PROFILE block populated, `scrum/backlog.md` seeded; (4) toggle the flag off and confirm Solo-mode messaging. Note to use the repo's `verify` skill for the live run.

- [ ] **Step 4: Run the lint (the test)**

Run: `pwsh -File tests/lint.ps1`
Expected: `LINT OK` and exit code 0.

- [ ] **Step 5: Commit**

```bash
git add tests/lint.ps1 tests/CHECKLIST.md
git commit -m "test: add structural lint and smoke-test checklist"
```

---

### Task 15: Finalize README & full verification

**Files:**
- Modify: `README.md`

**Interfaces:**
- Consumes: the whole repo.

- [ ] **Step 1: Expand `README.md`** with a "How it works" section (topology one-liner + the bootstrap → sprint loop), a "What's in the box" list (catalog, skills, commands), and a link to the spec + INTEGRATIONS.

- [ ] **Step 2: Run full lint**

Run: `pwsh -File tests/lint.ps1`
Expected: `LINT OK`.

- [ ] **Step 3: Confirm no stray active agents**

Run: `Get-ChildItem .claude/agents -Filter *.md -ErrorAction SilentlyContinue`
Expected: no `.md` files (only `.gitkeep`) — the template ships with an empty active team.

- [ ] **Step 4: Commit**

```bash
git add README.md
git commit -m "docs: finalize README with how-it-works and contents"
```

---

## Self-Review (completed by plan author)

**1. Spec coverage:** every spec section maps to a task — principles/CLAUDE.md → T2; repo structure → T1/T3; catalog → T8–T10; integrations (3 tiers, Context7, frontend-design, impeccable, security gate) → T4/T6/T7; bootstrap flow (6 phases, 3 gates) → T11; specialization pass → T11/T12; SCRUM loop + reconciliation → T13; robustness (Solo fallback, idempotency, re-hydration) → encoded in T2/T11/T13; testing → T14/T15; prerequisites → T1/T4/README. No gaps.

**2. Placeholder scan:** no "TBD/TODO/handle appropriately". Prose-heavy files use authoritative structural specs (declared in Global Constraints), not placeholders; config/schema files give literal content.

**3. Type/name consistency:** skill names (`karpathy`, `agent-designer`, `write-a-skill`, `self-improving-agent`, `skill-security-auditor`, `impeccable`), the DG markers (`BEGIN/END GENERATED: DG PROFILE`), artifact paths (`VISION.md`, `team/roster.md`, `scrum/backlog.md`, `scrum/sprints/sprint-NN.md`, `scrum/retros/retro-NN.md`), and command names (`bootstrap`, `specialize`, `sprint-plan`, `review`, `retro`, `status`) are used identically across the lint (T14), CLAUDE.md (T2), and the commands (T11–T13).
