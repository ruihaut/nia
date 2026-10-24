# NĪĀ

**L'eau de coco de Polynésie, réinventée.**

« En France, ils ont le raisin. En Polynésie, nous avons le coco. »

NĪĀ veut faire de l'eau de coco polynésienne un produit d'exception, commandé à la carte des restaurants, hôtels et bars de Polynésie, dont les Polynésiens peuvent être fiers. Le chemin passe par un premier palier : des cocos jeunes (*nīā*) découpées en diamond cut, livrées aux opérateurs d'excursion.

Ce projet n'est pas que digital : il touche l'approvisionnement, la transformation, le conditionnement et la vente dans le monde réel. Ce repo est d'abord l'espace de réflexion et de pilotage du projet.

## Où lire quoi

- `VISION.md` : le problème, la finalité, les deux paliers, le périmètre, les non-objectifs, le vocabulaire et les risques. **Source de vérité.**
- `docs/01-business-case.md`, `docs/02-project-charter.md`, `docs/03-project-management-plan.md`, `docs/04-chiffres-cles.md`, `docs/05-presentation.md` : business case, charte, plan de management, fiche des chiffres clés et source de présentation (slide par slide) du palier 1 ; leurs annexes de travail (modèle financier, WBS, marché, risques, customer journeys, variétés et terroirs, gamme) sont dans `docs/annexes/`.
- `docs/notes/` : notes brutes du fondateur, versées telles quelles.
- `team/roster.md` : l'équipe d'agents activée pour ce projet, et pourquoi.
- `scrum/backlog.md`, `scrum/sprints/`, `scrum/retros/` : le backlog priorisé, les sprints et les rétrospectives.
- `.claude/agents/` : les agents spécialisés pour NĪĀ.
- `catalog/` : les rôles génériques r-stack (bibliothèque, jamais chargée telle quelle).

## Comment travailler ici

Le repo tourne sur [r-stack](https://github.com/ruihaut/r-stack), une équipe d'agents Claude Code : un Director-General (la session principale, aussi Product Owner), des directeurs par domaine et des spécialistes. La mécanique et les principes sont dans `CLAUDE.md`.

Boucle de travail, dans Claude Code :

```
/sprint-plan → travail → /status → /review (gate ③) → /retro
```

`/bootstrap` a déjà été joué ; `/specialize` ré-affûte un agent quand la vision évolue.

Les artefacts projet sont en français. La mécanique r-stack reste en anglais.
