# Plan de management de projet — NĪĀ, palier 1

> **Statut : v0, référence de pilotage proposée au chef de projet et au sponsor.** Rédigé le 2026-10-24 par le Director-General à partir des annexes A1 à A7. Découle du business case (`docs/01-business-case.md`) et de la charte (`docs/02-project-charter.md`).
> **Principe de rédaction.** Le périmètre est défini et validé d'abord ; ressources, coûts, calendrier et risques en sont déduits. Le niveau de détail est celui d'un pilote à petit budget porté par une personne : work packages, pas tâches ; markdown, pas outil ; un tableau de bord d'une page. Tout chiffre est [estimé] ou [supposé] tant qu'il n'est pas marqué [relevé].

---

## 0. Comment ce plan est utilisé

- **Source de vérité** : ce fichier et ses annexes dans `docs/`, le backlog dans `scrum/backlog.md`, les sprints et rétrospectives dans `scrum/`. La règle r-stack s'applique : markdown d'abord, toute liste de tâches n'est qu'un miroir.
- **Rythme** : sprints de deux semaines (`/sprint-plan` → travail → `/status` → `/review` → `/retro`) ; revue sponsor mensuelle ; comité de changement à la demande.
- **Rôles** : le fondateur est chef de projet et exécute le terrain ; le Director-General (session r-stack) prépare, documente et garde la finalité ; les directeurs et spécialistes IA instruisent ; le challenger contredit. Le fondateur reste responsable de chaque livrable.
- **Niveau de formalisme choisi** : adapté au risque accepté. On formalise ce qui protège le produit et les gens (hygiène, froid, traçabilité, PV de recette, seuils d'arrêt) ; on reste léger sur le reste.

---

## 1. Périmètre et exigences

### 1.1 Approche de gestion du périmètre

1. Le périmètre est écrit (§ 1.3–1.4), relu par le challenger et signé par le fondateur dans la charte.
2. Il est **validé avec l'opérateur pilote** : au jalon J5, l'opérateur relit et contresigne une fiche d'une page (produit, critères d'acceptation, exclusions, volume indicatif, prix, règle de refus, retours hebdomadaires). Toute demande hors de cette fiche pendant le pilote est notée et traitée à J7, pas en cours de route.
3. Toute modification passe par le comité de changement (§ 7). Les non-objectifs de `VISION.md` ne sont pas modifiables par ce plan.
4. Les exigences sont tracées jusqu'aux work packages (dictionnaire A2 § 3) et vérifiées par leurs critères d'acceptation.

### 1.2 Besoins recueillis

| Source | Besoin exprimé | Traduction dans le plan |
|---|---|---|
| Brief fondateur et `VISION.md` | Une marque dont les Polynésiens sont fiers ; une seule finalité (CHR), deux paliers ; buy or make ; make it work, make it right, make it fast | Palier 1 borné, origine toujours dite, machine seulement sur mesure, critère de sortie vers le palier 2 |
| Notes du fondateur (parcours en 11 étapes) | Récolte → découpe → stockage réfrigéré → commande → livraison → prise en main → service → retours | Mapping étape → work packages (A2 § 1.2) ; stockage réfrigéré conditionné au test de conservation |
| Interview de bootstrap | Première livraison sous 6 mois ; fondateur seul profil tech ; coco incluse dans l'excursion ; Tahiti puis Moorea ; fret agricole à vérifier | Jalon J6 ≤ 30 avril 2027 ; relais terrain ; pas de revente ; Moorea à partir de juin ; WP 4.1 et 5.3 |
| Opérateurs (à relever, A3 § 3.8–3.9 et A5) | Régularité, zéro coco ratée, livraison avant le départ, garder un geste pour le guide, pas de réfrigérateur de plus | Critères d'acceptation du produit, kit de service, glacière de prêt, livraison J-1 ou matin |
| Services du Pays (à confirmer, A2 § 7) | Déclaration d'établissement, préconisations denrées végétales, étiquetage, DLC, biosécurité inter-îles | Branche 4 du WBS, jalon J4 |

### 1.3 Description du produit et critères d'acceptation

Produit : **une coco nīā, découpée en diamond cut, froide, marquée NĪĀ, livrée en caisse, prête à être ouverte et servie par le guide** (spécification complète A2 § 1.1). Critères d'acceptation vérifiés à chaque livraison :

1. 100 % des cocos au stade nīā selon la fiche de sélection ; aucune ʻōuo ni ʻōmoto avancée.
2. Découpe conforme au protocole : facettes régulières, coque interne intacte, aucune fibre, moisissure ni odeur.
3. Température à cœur ≤ 7 °C à la remise, mesurée et consignée sur le bon de livraison.
4. Date de découpe et DLC lisibles sur la caisse ; DLC ≥ J+2 à la remise.
5. Quantité livrée = quantité commandée ; cocos refusées remplacées ou non facturées.
6. Marquage NĪĀ présent et propre sur chaque coco.
7. Aucune réclamation sanitaire d'un passager imputable au produit.

### 1.4 Description du travail du projet et exclusions

Le travail est tout ce qui rend ce produit possible, légal, vendu et livré régulièrement : huit branches, trente work packages (§ 1.5). Exclusions : celles de la charte § 4.3 (pas de vente au touriste, pas d'eau extraite, pas de machine pendant le pilote, pas d'île hors Tahiti et Moorea, pas de froid fourni au-delà d'une glacière, pas de second produit, pas de recrutement à temps plein, pas de code ni d'outil digital).

### 1.5 WBS

```
1  Gouvernance, financement et pilotage
   1.1 Charte de projet et cadrage
   1.2 Financement : apport et sponsor                                  → J1
   1.3 Structure juridique, banque, assurance RC
   1.4 Pilotage : coûts, risques, revues sponsor
2  Filière amont (cocos nīā)
   2.1 Critère de stade nīā écrit et testé
   2.2 Cartographie et sélection des cocoteraies (≥ 2 sources)
   2.3 Contrat cocoteraie partenaire                                     → J2
   2.4 Achat et contrôle à réception (protocole, traçabilité)
3  Process découpe et froid
   3.1 Protocole diamond cut manuel mesuré
   3.2 Test de conservation après découpe (fixe la DLC et le rythme)    → J3
   3.3 Atelier de découpe et équipement froid
   3.4 Recrutement et formation du découpeur
   3.5 Production des lots (à blanc puis payants)
4  Réglementaire, hygiène et assurance
   4.1 Cadrage réglementaire : obligations, rendez-vous avec le Pays, fret agricole
   4.2 Plan de maîtrise sanitaire simplifié
   4.3 Étiquetage, DLC et documents d'accompagnement
   4.4 Dossier de conformité déposé et obtenu                            → J4
5  Logistique et livraison
   5.1 Chaîne du froid de bout en bout
   5.2 Transport routier Tahiti
   5.3 Liaison inter-îles Moorea (deux variantes selon le fret)
   5.4 Processus commande → préparation → livraison → retours
6  Pilote commercial
   6.1 Cartographie et sélection des opérateurs (types prioritaires A5)
   6.2 Coût de revient, prix et offre
   6.3 Contrat opérateur pilote et validation du périmètre              → J5
   6.4 Prise en main par l'opérateur (formation, kit)
   6.5 Exécution du pilote : livraisons, retours, indicateurs           → J6
7  Marque et présentation
   7.1 Présentation « façon NĪĀ » : marquage, geste, phrase du guide FR/EN, origine dite
   7.2 Kit opérateur et marquage testés en conditions réelles
8  Clôture et leçons
   8.1 PV de recette du pilote et revue                                  → J7
   8.2 Bilan, capitalisation, note buy or make, dossier de décision palier 2 → J8
```

Le WBS a été construit avec les expertises concernées (operations-director assumant supply-analyst et process-engineer ; business-director et market-scout pour la branche 6 ; brand-director pour la branche 7 ; challenger en relecture). **Dictionnaire du WBS** (description, livrables, critères d'acceptation, ressources, durée, coût, dépendances pour chacun des trente work packages) : annexe A2 § 3. Un work package ajouté par ce plan à la branche 2, hors chemin critique : **2.5 Dégustation comparative variétés × terroirs** (protocole A6 § 5, 40–90 k XPF, 6–8 semaines, février–mars 2027), qui tranche l'hypothèse « cépage » avant toute promesse de gamme (A7).

---

## 2. Calendrier

### 2.1 Approche

Les work packages sont décomposés en activités, ordonnés, estimés en semaines de travail effectif, puis placés dans un planning hebdomadaire sur 53 semaines (A2 § 4.5). Le niveau de détail retenu pour le pilotage est **le work package et le jalon** ; les activités vivent dans les sprints de deux semaines. M0 = novembre 2026 ; semaine 1 = lundi 2 novembre 2026.

### 2.2 Jalons destinés au sponsor (référence calendaire)

| Jalon | Contenu | Cible | Limite |
|---|---|---|---|
| **J1** Go financement | Fonds disponibles, charte signée, six conditions du business case § 7.2 cochées | 4 janvier 2027 (S10) | 18 janvier 2027 |
| **J2** Cocoteraie partenaire signée | Contrat avec fiche nīā annexée et règle de refus ; seconde source identifiée | 1er février 2027 (S14) | 15 février |
| **J3** Protocole et conservation validés | Protocole de découpe mesuré, DLC fixée, rythme découpe → livraison décidé | 15 février 2027 (S16) | 1er mars |
| **J5** Opérateur pilote signé | Accord pilote, périmètre contresigné, première livraison datée | 8 mars 2027 (S19) | 29 mars |
| **J4** Conformité obtenue | Récépissé ou attestation CHSP, RC à jour | 22 mars 2027 (S21) | 26 avril |
| **J6** Première livraison payante | Première livraison facturée | **Semaine du 5 avril 2027 (S23)** | **30 avril 2027** |
| **J7** Fin du pilote | PV de recette signé après ≥ 20 semaines de livraisons, revue | 6 septembre 2027 (S45) | 27 septembre |
| **J8** Décision palier 2 | Bilan en [relevé], dossier de décision, décision tracée | 4 octobre 2027 (S49) | 25 octobre |

### 2.3 Chemin critique et dépendances

```
3.1 protocole v0 (S2–S7) → 3.2 test de conservation lot 1 (S4–S9) → décision lieu et rythme (S10)
→ 3.3 atelier + froid (S10–S18) → 4.4 déclaration sur l'atelier (S15–S21) → 3.5 production à blanc (S18–S21)
→ 6.4 prise en main (S19–S21) → J6 (S23)
```

Le chemin critique passe par la conservation, l'atelier et la conformité, pas par la vente. Marges : une semaine entre J4 cible et la seconde production à blanc, une semaine avant J6, trois semaines entre J6 cible et sa limite. J1 est la porte d'entrée : sans fonds en S10, l'atelier et le froid glissent d'autant.

| Dépendance | Type | Effet |
|---|---|---|
| Test de conservation (3.2) → lieu de l'atelier (3.3) | Interne, décisive | Si DLC < 5 jours : découpe à J-1 près de la cocoteraie, atelier mobile ; la négociation 2.3 inclut l'option de mise à disposition d'un espace |
| Atelier existant (3.3) → déclaration CHSP (4.4) → livraison (6.5) | Interne, chemin critique | Déclaration déposée S15, obtenue S21 |
| Réponse DGAE sur le fret (4.1) → variante Moorea (5.3) | Externe | Décide « livrer depuis Tahiti » ou « cocos brutes + découpe à Moorea » ; n'affecte pas J6 (Tahiti) |
| Fermeture des administrations 20 décembre – 5 janvier | Externe | Rendez-vous CHSP, DGAE, biosécurité pris avant mi-décembre |
| Saison des pluies novembre–avril | Externe | Terrain sous contrainte ; bon pour tester la chaîne du froid |
| Pâques 28–29 mars 2027 | Externe | J6 placé après |
| Haute saison juin–octobre | Externe | Huit semaines de rodage avant ; extension Moorea et second opérateur à partir de juin ; J7 mesure une saison pleine |
| Délai d'import d'un équipement froid (6–12 semaines) | Externe | Acheter sur stock à Tahiti ou d'occasion pour sortir le froid du chemin critique |

Le planning hebdomadaire complet (work packages actifs par semaine, événements, contraintes) est en A2 § 4.5 ; il constitue la **référence calendrier** avec le tableau des jalons ci-dessus.

---

## 3. Coûts et ressources

### 3.1 Estimation à partir du WBS et référence budgétaire

Deux estimations indépendantes ont été produites : le modèle financier (A1, par postes de coût, trésorerie mensuelle) et le dictionnaire du WBS (A2, par work package). Elles ne se recouvrent pas exactement :

| | Modèle financier A1 (option A, réaliste) | WBS A2 (somme des work packages) | Écart expliqué par |
|---|---|---|---|
| Investissement initial | ≈ 1,04 M (0,7–1,5 M) | inclus ci-dessous | — |
| Besoin de trésorerie maximal | ≈ 1,78 M en juillet 2027 ; 2,3–2,5 M à prévoir | Scénario sobre ≈ 2,5–3,5 M ; plan ≈ 4–5 M ; haut ≈ 6–6,5 M | A2 compte un loyer d'atelier de 60–150 k par mois sur 9 mois (A1 : 40 k dans les fixes), un froid à 300–800 k (A1 : 250 k d'occasion), 100–300 k d'analyses et 0,3–0,8 M de fonds de roulement |

**Référence budgétaire retenue : 3,0 M XPF pour douze mois**, soit le haut du scénario sobre de A2 et le besoin recommandé de A1 augmenté d'une réserve :

| Poste | Montant de référence | Règle |
|---|---|---|
| Investissement (froid d'occasion, outils, glacières, inox, hygiène, marquage, caution, création, RC, analyses, formation) | 1,0 M | Aucune dépense d'atelier ou de froid avant J1 |
| Pertes d'exploitation et fonds de roulement jusqu'au point bas (loyer, découpeur, cocos, glace, transport, créances à 30 jours) | 1,5 M | Plan de trésorerie mensuel ; seuil d'arrêt |
| Réserve de management | 0,5 M (≈ 17 %) | Engagée seulement par décision du comité de changement |
| **Total** | **3,0 M** | Phase de vérification ≤ 150 k incluse |

Deux postes font l'écart entre sobre et plan : **l'atelier** (local prêté ou chez la cocoteraie contre local loué) et **le fonds de roulement** (délai de paiement des opérateurs). Les relevés de la phase de vérification (loyer réel, délai de paiement, prix d'achat) permettront de re-baser le budget à J1 (WP 6.2 v1).

### 3.2 Suivi des coûts

- **Tableau de bord mensuel d'une page** (WP 1.4), présenté au sponsor : les six KPI de pilotage (réassort, volume, marge par coco, livraisons à l'heure, pertes, trésorerie) ; coûts réels contre estimés **par branche du WBS** ; coût complet par coco livrée et sa trajectoire ; écart au budget de référence et consommation de la réserve ; nombre de chiffres passés de [estimé] à [relevé].
- **Comptabilité par lot** : chaque lot de cocos porte un numéro (date, cocoteraie), ses coûts (achat, main-d'œuvre, glace, transport, pertes) et ses recettes ; c'est la base de la marge par coco.
- **Seuils d'alerte** : dépenses cumulées > 40 % de l'apport sans bon de commande signé ; écart > 10 % sur la référence ; réserve entamée à plus de 50 % ; point bas prévisionnel sous un mois de charges.
- Outils : tableur et carnet autocopiant ; pas d'outil développé (exclusion du périmètre).

### 3.3 Ressources

Les ressources sont traitées avec le périmètre et le calendrier : le fondateur est la ressource critique, la cocoteraie et le découpeur conditionnent le produit, l'opérateur pilote conditionne le pilote.

| Ressource | Engagement | Coût | Risque et réponse |
|---|---|---|---|
| Fondateur, chef de projet | Temps plein possible ; **≥ 50 % du temps sur le terrain** (journal hebdomadaire en quatre colonnes : terrain, commercial, marque, outillage) | Non rémunéré pendant le pilote (coût d'opportunité 2–4 M [estimé], hors VAN) | Épuisement ou dispersion : relais à la tâche identifié avant janvier ; « pas de code avant la première facture » |
| Découpeur | À la tâche (≈ 100 XPF par coco conforme) ou temps partiel déclaré CPS, 2–3 jours par semaine ; deux personnes formées | 30–80 k par mois au volume pilote | Instabilité : statut clarifié avant le premier paiement ; rémunération lisible ; le fondateur sait découper |
| Cocoteraie partenaire (+ seconde source) | Contrat de volume indicatif, jour fixe de récolte, fiche nīā, règle de refus | 100–250 XPF par coco | Hors stade ou irrégulière : check-list à réception, prime de sélection, seconde source |
| Opérateur pilote et son guide | Accord pilote 3–6 mois, ≥ 50 cocos par semaine, retours hebdomadaires | Client | Non-adoption : patron et guide signent ensemble ; quick wins visibles les quatre premières semaines |
| Sponsor | Revue mensuelle de 45 min ; décisions de jalon | 5–15 M en deux tranches ou nature, pour l'accélération et le palier 2 | Non trouvé : le palier 1 doit tenir sur l'apport seul |
| Équipe IA r-stack | Director-General, trois directeurs, six spécialistes | Temps de session | Dispersion documentaire : chaque sprint produit au moins une mesure terrain |
| Services du Pays, laboratoire, assureur, transporteurs | Rendez-vous, analyses, contrats | Analyses 15–40 k l'unité ; RC 60–200 k par an | Délais : rendez-vous avant mi-décembre, créneaux d'analyse réservés avant la mise au froid |

### 3.4 Matrice de responsabilités (RACI)

R = réalise, A = responsable du résultat, C = consulté, I = informé. Le Director-General et les directeurs IA préparent et documentent ; ils ne portent jamais le A.

| Livrable / décision | Fondateur (CdP) | Sponsor | Cocoteraie | Découpeur | Opérateur pilote | DG (IA) | Directeur IA concerné | Challenger (IA) |
|---|---|---|---|---|---|---|---|---|
| Charte et plan de management | A/R | A (approbation) | — | — | — | R (rédaction) | C | C |
| Go financement J1, décisions J7 et J8 | R (dossier) | **A** (fondateur par intérim) | — | — | I | R (préparation) | C | **C (avis écrit)** |
| Fiche de sélection nīā et contrat cocoteraie | A/R | I | **R** (coécrit, signe) | I | — | I | R (supply-analyst) | C |
| Protocole diamond cut, test de conservation, DLC | A/R | I | C | R (exécute) | I | I | R (process-engineer) | C |
| Atelier, froid, achats > 150 k | R (choix) | **A** | C (option sur place) | — | — | I | C (operations-director) | C |
| Plan d'hygiène, déclaration CHSP, étiquetage | A/R | I | I | R (applique) | I | I | R (operations-director) | — |
| Chaîne du froid et logistique, variante Moorea | A/R | I | — | R | C | I | R (operations-director) | — |
| Cartographie opérateurs, offre, prix, accord pilote | A/R | C (prix sous le plancher) | — | — | **C puis signe** | I | R (business-director, market-scout) | C |
| Validation du périmètre avec l'opérateur | A/R | I | — | — | **R** (contresigne) | I | C | — |
| Présentation façon NĪĀ, phrase du guide, origine dite | A/R | I | C (nom du lieu) | — | C (le guide) | C | R (brand-director, copywriter) | C |
| Dégustation comparative variétés × terroirs (2.5) | A/R | I | R (fournit les lots) | — | C (passagers) | I | R (supply-analyst, brand-director) | C |
| Exécution du pilote, indicateurs hebdomadaires | A/R | I (mensuel) | R (livre) | R (découpe) | R (sert, rend les retours) | I | C | I |
| PV de recette | A/R | I | — | — | **R** (signe) | C | C | C |
| Tableau de bord mensuel et registre des risques | A/R | I | — | — | — | R (préparation) | C | C |
| Bilan, note buy or make, dossier palier 2 | A/R | **A** (décision) | C | C | C | R (rédaction) | R (financial-modeler, process-engineer) | **C** |
| Changements de périmètre, budget, calendrier | R (demande) | **A** | I | I | I | R (instruction) | C | **C (avis)** |

---

## 4. Qualité et validation

### 4.1 Niveau de qualité visé

Pas un niveau de laboratoire : un niveau **constant et sûr**, qu'un guide vérifie d'un coup d'œil et qu'un passager remarque.

| Cible | Valeur | Mesure |
|---|---|---|
| Stade | 100 % nīā dans les caisses livrées | Tri à réception, contrôle avant livraison |
| Sécurité | 0 incident sanitaire ; 0 rupture de froid > 7 °C non tracée | Enregistreurs, bons de livraison, registre des réclamations |
| Conformité à la livraison | ≥ 95 % des cocos acceptées par l'opérateur | Bons de livraison, refus consignés |
| Régularité | ≥ 90 % des livraisons à l'heure convenue (cible pilote 95 %) | Journal du pilote |

### 4.2 Contrôles et check-lists

Un contrôle à chaque étape du parcours (récolte, réception, découpe, stockage, préparation de commande, transport, remise, service à bord), avec responsable, enregistrement et action en cas d'écart (A2 § 6.2). Deux check-lists sont le cœur du dispositif :

- **Check-list A, qualité à réception des cocos** (12 points : stade, calibre, intégrité, pédoncule frais, son, propreté ; ouverture d'une coco sur vingt pour l'amande et l'eau ; comptage, numéro de lot, taux de refus consigné) : A2 § 6.3.
- **Check-list B, avant livraison** (12 points : même lot et DLC ≥ J+2, découpe conforme, aucune odeur, marquage, température à cœur ≤ 4 °C au départ, comptage et étiquette de caisse, glacière pré-refroidie et enregistreur, kit, bon de livraison, horaire, caisses à reprendre, ferry confirmé pour Moorea) : A2 § 6.3.

### 4.3 Definition of Done des livrables du projet

Un livrable (protocole, fiche, contrat, rapport) est « done » quand : il est écrit dans le repo, en français, daté, versionné ; chaque chiffre est marqué [relevé], [estimé] ou [supposé] avec une date de vérification pour les [supposé] ; s'il s'agit d'un protocole ou d'une check-list, **il a été exécuté au moins une fois en conditions réelles par quelqu'un d'autre que son auteur** ; ses critères d'acceptation sont cochés avec preuve (photo, registre, signature, résultat de laboratoire) ; il a été relu par le directeur IA concerné et, pour les livrables de jalon, par le Director-General et le challenger ; ses coûts réels sont inscrits dans le tableau de bord. Cette Definition of Done est tenue avec le Product Owner (fonction DG) et revue à chaque rétrospective.

### 4.4 Validation du périmètre et recette

- **Validation du périmètre** : fiche d'une page contresignée par l'opérateur à J5 (§ 1.1).
- **Revues de sprint** (gate ③ r-stack) : toutes les deux semaines, l'incrément est accepté contre l'objectif du sprint et la vision ; chaque sprint doit produire au moins une mesure terrain.
- **PV de recette du pilote** (jalon J7) : signé par l'opérateur après vingt semaines, dix lignes (livraisons prévues et réalisées, cocos acceptées et refusées, stade, découpe et marquage, froid, sécurité, service, réaction des passagers, réserves, décision de poursuite avec volume et prix acceptés). Modèle : A2 § 6.6.
- **Recette interne** : revue avec le Director-General et le challenger à J7 : le palier 1 sert-il la finalité ou devient-il une fin en soi ?

---

## 5. Parties prenantes, communication et changement

### 5.1 Parties prenantes

Registre complet (intérêt, influence, attentes, attitude probable, stratégie d'engagement) : annexe A3 § 5. Les trois relations qui décident : la **cocoteraie** (fiche nīā coécrite, paiement rapide, visite hebdomadaire), le **couple patron–guide** de l'opérateur pilote (jamais signer avec l'un sans l'autre), le **sponsor** (seuils de décision annoncés à l'avance, reporting court et honnête). La **communauté polynésienne** est une partie prenante diffuse mais réelle : ton de fierté sans exotisme, stade nīā nommé en tahitien, producteurs payés correctement et on le dit ; les mots *motu* et *mouʻa* sont réservés et ne servent pas de décoration au palier 1 (A7).

### 5.2 Plan de communication

| Partie prenante | Quoi | Quand | Canal | Qui |
|---|---|---|---|---|
| Sponsor | Tableau de bord d'une page (6 KPI, coûts, risques, décisions à prendre) | Mensuel, 45 min ; point flash de 15 min si un seuil est franchi | Réunion et une page écrite | Fondateur |
| Équipe projet (repo) | Journal de pilote, décisions, hypothèses vérifiées ou invalidées | `/status` hebdomadaire, revue de sprint bimensuelle | Markdown dans `scrum/` et `docs/` | Fondateur, DG |
| Cocoteraie | Commande de la semaine, retour qualité du lot, paiement | Hebdomadaire, même jour | Visite ou appel, message écrit | Fondateur |
| Découpeur | Planning, volume, retour qualité du cut, paie | Hebdomadaire ; retour à chaque lot | Oral, photo de référence | Fondateur |
| Opérateur pilote | Confirmation J-1, bon de livraison signé, point de satisfaction | Chaque livraison ; entretien toutes les deux semaines ; bilan à J7 | Message, bon signé, entretien de 20 min au retour d'une sortie | Fondateur |
| Guides | Phrase NĪĀ FR/EN, fiche de service, remerciement nominatif | Démarrage, puis à chaque évolution | En main propre, à bord | Fondateur, brand-director (texte) |
| Services du Pays | Déclaration, questions, mise en conformité | Avant la première découpe d'essai, puis à chaque changement (Moorea, machine) | Rendez-vous, courrier | Fondateur, operations-director |
| Opérateurs suivants, futurs CHR | Dégustation, chiffres du pilote avec accord ; écoute sans vendre | Saison intermédiaire ; opportuniste | Quai, bouche-à-oreille, conversation | Fondateur |
| Banque, financeur | Dossier avec résultats du pilote | Après douze semaines de pilote | Rendez-vous | Fondateur, financial-modeler |

**Déclencheurs d'escalade** (sponsor et DG sous 48 h) : deux livraisons manquées ou en retard dans le mois ; rupture d'approvisionnement > 1 semaine ou rejet > 25 % sur deux lots ; incident sanitaire ou plainte de passager ; marge brute par coco négative deux mois consécutifs après le deuxième mois ; l'opérateur ne réassortit pas deux semaines de suite sans raison saisonnière ; un tiers commence à livrer des cocos découpées ; trésorerie sous un mois de charges.

### 5.3 Conduite du changement chez l'opérateur pilote

L'opérateur change une habitude quasi gratuite. Cinq leviers (A3 § 7) : **urgence** montrée, pas dite (dégustation côte à côte, « combien de cocos ratées la semaine dernière ? ») ; **coalition** patron et guide, le guide garde un geste ; **vision** en une phrase (« votre excursion a un moment que les autres n'ont pas, et il a un nom ») ; **quick wins** chiffrés (semaine 1 : zéro coco à chercher ; semaine 2 : premières photos ; semaine 4 : zéro coco ratée) ; **ancrage** à huit semaines (la coco NĪĀ dans son descriptif, routine de commande fixe, ancien circuit éteint, témoignage pour les suivants). Ce qui fait échouer : une livraison manquée dans les trois premières semaines, un cut irrégulier devant les passagers, un prix négocié à la baisse avant même le premier service.

---

## 6. Risques et achats

### 6.1 Gestion des risques négatifs et des opportunités

- **Registre** : annexe A4 (19 risques négatifs, 5 risques de l'option « ne rien faire », 8 opportunités, 15 hypothèses critiques), tenu par le fondateur, préparé par le challenger, revu à chaque revue sponsor et à chaque rétrospective.
- **Évaluation** : probabilité × impact de 1 à 5 ; coût chiffré du risque et de sa réponse quand c'est possible ; zone rouge ≥ 15.
- **Stratégies de réponse** : escalade (au sponsor), évitement (changer le plan), transfert (contrat, assurance), mitigation, acceptation. Les opportunités ont leurs réponses symétriques : exploiter, partager, améliorer, accepter.
- **Ce qui n'est pas couvert à 100 %**, par choix : concurrence réactive, météo (5–10 % de pertes budgétées), accident et incident sanitaire au-delà de l'assurance et du protocole, Moorea avant la réponse sur le fret et le test de froid (A4 § 3.4).

| Id | Risque rouge | P × I | Réponse | Propriétaire | Déclencheur |
|---|---|---|---|---|---|
| R01 | Conservation réelle < 1 semaine | 20 | Lot test 14 jours dès S1 ; si < 7 jours : découpe à J-1, film, stock ≤ 3 jours | process-engineer / operations-director | Résultat du lot ; brunissement visible sur un lot livré |
| R02 | Non-adoption, internalisation (le guide-coupeur est le spectacle) | 20 | Cibler les opérateurs sans numéro coco (A5) ; vendre stade, froid, régularité ; laisser la finition au guide | market-scout / business-director | > 50 % des dix premiers entretiens disent « on le fait nous-mêmes » |
| R03 | Coût complet > prix accepté | 16 | Coût complet avant tout prix ; devis à trois niveaux ; marge ≥ 150 XPF ou on ne lance pas | financial-modeler / business-director | A1 v1 : marge < 150 ou point mort > 2 500 par mois |
| R04 | Cocoteraie hors stade ou irrégulière | 16 | Deux sources ; check-list et droit de refus ; prime de sélection ; essai de 50 cocos triées | supply-analyst / operations-director | Rejet > 20 % sur deux livraisons ; un seul fournisseur en janvier |
| R09 | Fret Moorea payant ou froid rompu | 16 | Fret compté plein ; demande DGAE ; sonde sur trajet réel ; sinon découpe à Moorea avec cocos de Moorea | operations-director | Silence ou refus DGAE en janvier ; > 8 °C à l'arrivée |
| R05 | Délai ou refus réglementaire | 15 | Rendez-vous CHSP avant la première découpe ; travaux chiffrés ; DLC prudente ; escalade si > 2 mois | operations-director ; fondateur | Pas de réponse écrite en janvier |
| R06 | Fondateur seul : épuisement ou dispersion | 15 | Journal de temps ; relais à la tâche avant janvier ; pas de code avant la première facture | Fondateur ; challenger surveille | Terrain < 50 % deux semaines de suite |
| R07 | Trésorerie épuisée avant la première facture | 15 | Plan de trésorerie avec seuil d'arrêt ; froid d'occasion ou loué ; pas de chambre froide sans lettre d'intention | Fondateur ; financial-modeler | Dépenses > 40 % de l'apport sans bon de commande |

Opportunités à instruire sans coût dans les entretiens déjà prévus : hôtels de plage, pensions et traiteurs comme clients (O1) ; cocos brutes d'une île productrice à fret gratuit (O2) ; la cocoteraie qui découpe elle-même (O4) ; mesures transférables au palier 2, Brix et rendement en eau (O6).

### 6.2 Achats et fournisseurs

Tableau complet (fournisseur, type de contrat, délai, coût, risque, clause clé) : annexe A2 § 5. Les contrats sont simples et courts (6 mois pour la cocoteraie, 3–6 mois pour le pilote, bail court ou convention pour l'atelier), payables à la livraison ou à la semaine.

| Achat | Type de contrat | Délai | Coût [estimé] | Clause clé |
|---|---|---|---|---|
| **Cocos nīā, source principale** | Contrat de volume indicatif 6 mois, paiement à la livraison | Commande à J-7, récolte à jour fixe | 100–250 XPF par coco | Fiche nīā annexée ; droit de refus sans paiement ; préavis de 2 semaines sur les prix ; option d'espace de découpe sur place |
| Cocos nīā, source de secours | Achat au comptant | 48–72 h | 150–300 XPF par coco | Lettre d'intention ; commande test trimestrielle |
| **Froid de stockage** | Achat, SAV local | Stock Tahiti 1–2 semaines ; import 6–12 semaines | 300–800 k | Pièces et SAV à Tahiti ; alarme de température ; stock local préféré même plus cher |
| **Atelier** | Bail court ou convention de mise à disposition | 2–6 semaines | 60–150 k par mois + dépôt | Eau potable et évacuation ; clause de sortie à 1 mois si conformité refusée |
| Glacières, enregistreurs, caisses, outils, consommables | Achat au comptant | 1–6 semaines (pailles importées) | 260–730 k pour le pilote | Deux jeux d'outils ; stock de 8 semaines de consommables |
| Ferry Tahiti–Moorea, variante fret payant | Billets, fret à l'unité | Immédiat | 1 500–3 000 passager A/R ; 1 000–2 000 par colis | Livraison Moorea décalable de 24 h sans pénalité |
| Fret inter-îles, variante prise en charge par le Pays | Dossier DGAE (arrêté 1586 CM modifié) | Formalités à relever | 0 de fret si éligible | Si la coco parée est inéligible : cocos brutes à fret gratuit et découpe près du client |
| Assurance RC professionnelle | Contrat annuel | 2–4 semaines | 60–200 k par an | Garantie explicite « préparation et livraison de denrées », intoxication couverte |
| Découpeur | Contrat à la tâche ou temps partiel déclaré CPS ; ou prestation de la cocoteraie | 3–5 semaines | 60–120 XPF par coco | Deuxième personne formée ; rémunération à la coco conforme |
| Laboratoire d'analyses | Prestation à l'analyse | 5–10 jours par résultat | 15–40 k par analyse | Créneaux réservés avant la mise au froid du lot test |

**Achats critiques** : les cocos au bon stade (le contrat porte le critère de qualité), le froid (seul achat dont le délai peut décaler J6), l'atelier (support de la déclaration sanitaire, donc de J4).

---

## 7. Pilotage et gestion des changements

### 7.1 Références (baselines)

| Référence | Contenu | Document |
|---|---|---|
| **Périmètre** | Produit et critères d'acceptation (§ 1.3), exclusions (charte § 4.3), WBS à 30 + 1 work packages (§ 1.5) et son dictionnaire | A2 § 1–3, ce plan |
| **Calendrier** | Les huit jalons avec cibles et limites (§ 2.2), le planning hebdomadaire (A2 § 4.5) | Ce plan § 2 |
| **Coûts** | 3,0 M XPF dont 0,5 M de réserve ; ventilation par branche du dictionnaire ; plan de trésorerie mensuel A1 § 4 | Ce plan § 3.1 |
| Qualité | Niveau visé, critères d'acceptation, Definition of Done | § 4 |

Les références sont figées à la signature de la charte et **re-basées une fois, à J1**, avec les relevés de la phase de vérification (loyer, prix d'achat, délai de paiement, DLC). Tout autre changement passe par le comité.

### 7.2 Mesure des écarts

À chaque revue mensuelle : écart de calendrier par jalon (semaines d'avance ou de retard sur la cible, marge restante avant la limite) ; écart de coûts par branche et consommation de la réserve ; écart de périmètre (demandes hors fiche notées dans le journal) ; écart de qualité (KPI § 4.1 et business case § 5). Analyse de cause en une ligne par écart, action, propriétaire, date. Seuils qui déclenchent le comité : glissement d'un jalon au-delà de sa limite ; écart de coûts > 10 % de la référence ; toute demande de changement de périmètre ; tout KPI rouge deux mois de suite.

### 7.3 Comité de changement (Change Control Board)

| | |
|---|---|
| Composition | **Le sponsor** (décide ; le fondateur par intérim tant qu'il n'est pas désigné), **le chef de projet** (présente), **le challenger** (contradicteur, avis écrit obligatoire), le Director-General (instruit le dossier, vérifie la cohérence avec `VISION.md`) |
| Saisine | Toute modification d'une référence (§ 7.1) ; tout seuil de § 7.2 ; toute décision réservée au sponsor par la charte § 3.2 |
| Dossier | Une page : changement demandé, cause, effet sur périmètre, calendrier, coûts, risques et finalité ; options (accepter, refuser, différer, variante) ; avis du challenger |
| Délai | Décision sous une semaine ; sous 48 h pour un déclencheur d'escalade |
| Trace | Décision écrite dans `scrum/` (journal des décisions), référence mise à jour, backlog ajusté |
| Ce qui n'est pas un changement | La priorisation du backlog entre deux jalons, le choix d'un fournisseur non critique, l'ajustement d'une activité à l'intérieur d'un work package |
| Ce qui n'est jamais accepté par le comité | Un écart aux non-objectifs de `VISION.md` : cela relève du gate ① de la vision, avec le mainteneur |

### 7.4 Leçons apprises

- **Rétrospective** à chaque fin de sprint (`/retro`) : ce qui a marché, ce qui a raté, ce qu'on change ; deux backlogs alimentés, le produit et l'équipe (agents et skills ré-affûtés via `/specialize`).
- **Journal du pilote** hebdomadaire : hypothèses vérifiées ou invalidées, verbatims cités, mesures ; chaque passage d'un chiffre de [estimé] à [relevé] y est daté.
- **Revue de pré-mortem** à J1 et à J7 : les dix causes d'échec de A4 § 1 sont relues ; celles qui se sont manifestées, celles qui ont été évitées, celles qu'on n'avait pas vues.

### 7.5 Clôture

À J7 : PV de recette signé, revue interne, réserves listées avec propriétaire et date. À J8 : bilan économique en chiffres relevés (marge réelle, coût de revient, volume, pertes, temps du fondateur), classeur des protocoles et fiches fournisseurs en version transmissible à une équipe, note buy or make (seuil de volume pour une machine de découpe, options, coûts), enseignements pour l'eau extraite (conservation, froid, réglementaire, variétés et terroirs si la dégustation 2.5 a eu lieu), dossier de décision pour le sponsor : continuer, étendre, basculer vers une machine, pivoter vers la découpe à la cocoteraie, ou arrêter ; et, dans tous les cas, lancement de la faisabilité du palier 2 au plus tard au neuvième mois. Clôture administrative : contrats soldés, caisses récupérées, registres archivés dans le repo, plan de régime ou plan du palier 2 ouvert.

---

## 8. Articulation avec le backlog et les sprints r-stack

Les work packages se retrouvent dans `scrum/backlog.md` (items 1 à 16) ; chaque sprint de deux semaines prend les work packages de la fenêtre courante (A2 § 4.4) et doit produire au moins une mesure terrain. Premier sprint proposé (2–15 novembre 2026) : lot test de conservation mis au froid, contact CHSP pris, fiche nīā v0 avec un producteur, trois premiers entretiens d'opérateurs, lecture de l'arrêté fret sur Lexpol, charte signée.

---

## Annexes

- **A1** Modèle financier : `docs/annexes/A1-modele-financier-palier-1.md`
- **A2** Périmètre, WBS, dictionnaire, calendrier, achats, qualité, réglementaire : `docs/annexes/A2-perimetre-wbs-calendrier-qualite.md`
- **A3** Options, marché, parties prenantes, communication, valeur : `docs/annexes/A3-options-marche-parties-prenantes.md`
- **A4** Risques, opportunités, pré-mortem, hypothèses : `docs/annexes/A4-risques-opportunites-premortem.md`
- **A5** Compatibilité par type d'excursion, customer journeys, plan de prospection : `docs/annexes/A5-compatibilite-excursions-customer-journeys.md`
- **A6** Variétés et terroirs du coco, critère nīā par variété, protocole de dégustation : `docs/annexes/A6-varietes-terroirs-coco.md`
- **A7** Architecture de gamme (Motu / Mouʻa), lexique, test de marque : `docs/annexes/A7-architecture-de-gamme.md`
