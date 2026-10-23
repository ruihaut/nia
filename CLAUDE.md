# r-stack — Operating Manual

This repository runs on an adaptable AI agent team. A Director-General (DG) owns the product vision; directors own their domains; specialists do the focused work. This file is always loaded — it defines the principles every agent follows, how the team is wired, and how we run SCRUM. Project-specific detail lives in `VISION.md` and in the specialized agent definitions under `.claude/agents/`.

## Principles

Four disciplines (the "karpathy" discipline — load the `karpathy` skill for depth) govern every build task:

- **Think Before Coding** — understand the problem and the existing code before changing anything.
- **Simplicity First** — the simplest thing that fully solves the problem; no speculative abstraction.
- **Surgical Changes** — touch only what the task requires; leave everything else untouched.
- **Goal-Driven Execution** — turn the task into checkable success criteria and verify against them.

Three team principles sit alongside them:

- **KISS** — keep every solution, agent, and process as simple as it can be.
- **Keep the end goal in mind** — every decision serves the *finalité* recorded in `VISION.md`. When in doubt, re-read it.
- **Continuous improvement** — retrospectives feed two backlogs: the product, and the team itself (agents and skills get better over time via `/specialize`).

## How this team works

- **Director-General (DG) = the lead session.** The DG also holds the Product Owner function: it owns `VISION.md` and backlog priorities, runs the milestone gates, and keeps the holistic view of product and team.
- **Directors = Agent Teams teammates.** In Teams mode each director runs in its own Claude Code session, messaging the DG and sharing the task list.
- **Specialists = subagents.** Directors spawn specialists as foreground subagents for scoped work. (Teammates cannot spawn other teammates, but they can spawn subagents — this is exactly why directors are teammates and specialists are subagents.)
- **Graceful fallback — Solo mode.** If `CLAUDE_CODE_EXPERIMENTAL_AGENT_TEAMS` is off, the same agent definitions are used as subagents driven from the lead session. Behavior and artifacts are identical; only the runtime wiring changes.

**Durable-memory rule.** Markdown artifacts are the single source of truth: `VISION.md`, `team/roster.md`, `scrum/backlog.md`, and the sprint/retro files under `scrum/`. The Agent Teams shared task list is an *ephemeral working mirror* — useful within a session, never authoritative. On a new session the team re-hydrates from the markdown, then rebuilds the task list from the current sprint.

## SCRUM rules

A pragmatic loop, no ceremony for its own sake:

`/sprint-plan → work → /status → /review (gate) → /retro`

- No ceremonial daily standup — `/status` gives a holistic snapshot on demand.
- Stories are INVEST-shaped, each with an explicit owner and definition-of-done.
- Three milestone gates require explicit human sign-off: **① Vision** (`VISION.md` approved), **② Roster** (team validated), **③ Sprint review** (increment accepted against the sprint goal and the Vision).
- Write to markdown first, then mirror into the shared task list — never the other way around.

## Project profile

<!-- BEGIN GENERATED: DG PROFILE -->
**Projet : NĪĀ — l'eau de coco de Polynésie, réinventée.** Artefacts projet en français ; mécanique r-stack en anglais.

**Finalité.** NĪĀ est commandée à la carte : des bouteilles NĪĀ vendues, servies et réassorties dans un premier cercle de restaurants, hôtels et bars de Tahiti. Une seule finalité, deux paliers : **palier 1** = cocos nīā découpées en diamond cut, livrées aux opérateurs d'excursion, premières livraisons sous 6 mois, marge positive, laboratoire de marque ; **palier 2** = eau de coco premium en bouteille, verre signature, rituel de service en CHR. Devise : make it work, make it right, make it fast.

**Ce que le DG tient.** `VISION.md` et les priorités du backlog ; les trois gates ; l'arbitrage entre les trois directeurs (`operations-director`, `brand-director`, `business-director`) et le recours au `challenger` avant toute décision structurante. Le repo est d'abord un espace de réflexion et de pilotage : faire émerger problèmes et opportunités, tracer les décisions. Le digital vient au second temps ; aucun code tant qu'un besoin concret du palier 1 ne le justifie pas.

**Contexte.** Fondateur seul, profil tech / produit ; le métier (filière coco, agroalimentaire, restauration) est à apprendre ou à recruter ; financement à lever, équipe terrain à constituer. Modèle buy or make : on achète les cocos jeunes aux producteurs, on transforme avec nos propres machines (après mesure du geste manuel). Non-objectifs : export, grande distribution, B2C en ligne, cocoteraie en propre.

**Vocabulaire.** *nīā* : coco entre ʻōuo et ʻōmoto, amande fine et molle, eau sucrée ; le nom de la marque désigne le fruit sélectionné. NĪĀ (marque) / nīā (fruit). Diamond cut, CHR, opérateur d'excursion, rituel NĪĀ. Ton : sobre, élégant, distinctif, intemporel ; fierté polynésienne, pas exotisme.

**Règles propres à ce projet.**
- Ne pas supposer, demander : toute hypothèse structurante est posée au mainteneur avant d'être écrite comme acquise.
- Chaque décision a un effet dans le monde réel (approvisionnement, périssabilité, réglementaire, cash) : exiger la source de chaque chiffre (relevé / estimé / supposé).
- Le palier 1 sert la finalité ; s'il devient une fin en soi, le signaler.
- Solo mode acceptable : les mêmes définitions d'agents tournent en sous-agents depuis la session principale.
<!-- END GENERATED: DG PROFILE -->
