# Annexe A3 — Problème, options, marché, parties prenantes, communication, valeur

> Pièce du business case et du project management plan du **palier 1** de NĪĀ (pilote diamond cut auprès des opérateurs d'excursion, 6 à 12 mois, premières livraisons sous 6 mois à compter de novembre 2026).
> Rédigée par le business-director (travail du market-scout inclus), 2026-10-24. Les chiffres financiers (coût de revient, prix, marge, point mort, VAN, trésorerie) sont dans l'**annexe A1** du financial-modeler : cette annexe ne les refait pas, elle y renvoie.
> **Sourçage.** Aucun fait n'est [relevé] sur le terrain. Trois marquages : **[estimé : source web]** (chiffre public transmis par le DG après recherche web, URL citée, non recoupé sur place), **[estimé : raisonnement]** (ordre de grandeur déduit d'un raisonnement explicite) et **[supposé]** (hypothèse de travail à vérifier). Tout chiffre de marché ou de prix de cette annexe est à confirmer lors des entretiens opérateurs (backlog item 3) et du pré-mortem (item 1).
> **Annexes liées.** A1 (modèle financier) ; **A5** (compatibilité par type d'excursion, customer journeys, critères de choix de l'opérateur pilote) rédigée par le market-scout : A3 ne détaille pas ces trois points, elle y renvoie.

Décisions du fondateur, intégrées et non remises en cause ici : palier 1 seul évalué ; fondateur seul, profil tech, chef de projet ; apport 2–5 M XPF ; sponsor ou investisseur à trouver ; buy strict (la cocoteraie récolte) ; coco incluse dans l'excursion, pas de revente au touriste ; Tahiti puis Moorea ; non-objectifs : export, grande distribution, B2C en ligne.

---

## 0. En une page

- **Problème.** Les opérateurs d'excursion de Tahiti et Moorea servent déjà des cocos à boire à leurs passagers, mais de façon artisanale : approvisionnement au coup par coup, stade de maturité aléatoire, ouverture au coupe-coupe par le guide, aucune présentation, aucune histoire. Le touriste retient « une coco », pas un produit.
- **Opportunité.** 281 227 touristes et 70 062 excursionnistes de croisière en 2025, record historique [estimé : source web ISPF, § 1.2]. Un marché estimé à **100 000–250 000 cocos par an** servies en excursion à Tahiti et Moorea [estimé : raisonnement, § 1.2], avec un prix de référence actuel de **150–300 XPF la coco brute** et un coût complet pour l'opérateur de **250–450 XPF** une fois le temps de guide compté [estimé : raisonnement, § 3.4]. Aucun fournisseur n'y propose une coco jeune sélectionnée, découpée, froide, présentée [supposé, à vérifier en priorité : « pourquoi ça n'existe pas déjà ? »]. Intuition du fondateur : les sorties bateau sont compatibles a priori, les randonnées non (transport pendant la marche) ; matrice complète en annexe A5.
- **Stratégie.** NĪĀ à la carte des CHR de Tahiti (palier 2). **Exécution évaluée ici** : le palier 1, un pilote payant diamond cut avec un opérateur, puis 3–5 opérateurs, qui apprend la filière, teste le prix et finance les premières machines.
- **Option recommandée : A (manuel porté par NĪĀ), avec bascule conditionnelle vers B** (première machine) sur seuil de volume mesuré, et C (découpe à la cocoteraie) gardée comme variante à tester pour Moorea. D (aller directement au palier 2) et 0 (ne rien faire) écartées. Détail § 2.
- **Trois KPI qui décident.** Taux de réassort de l'opérateur pilote (cible ≥ 80 % des semaines de la période), marge brute par coco livrée (cible > 0 dès le mois 2, chiffre en A1), livraisons à l'heure (cible ≥ 95 %). Détail § 4.
- **Sponsor recherché.** Un associé terrain ou un investisseur local qui connaît la filière coco ou le tourisme, apporte 5–15 M XPF ou son équivalent en nature (accès cocoteraie, local froid, réseau d'opérateurs), et tient trois seuils : un pilote payant signé, une marge par coco positive mesurée, un deuxième opérateur qui réassortit. Détail § 9.

---

## 1. Problème et opportunité

### 1.1 État actuel : comment le coco est servi en excursion aujourd'hui

Ce que l'on sait ou déduit du fonctionnement des excursions à Tahiti et Moorea (à confirmer entretien par entretien) :

| Dimension | État actuel probable | Marquage |
|---|---|---|
| Qui sert une coco | Les tours lagon avec pique-nique sur motu (Moorea surtout), une partie des tours 4x4 intérieur (arrêt « fruits » à Papenoo, Opunohu), une minorité des tours d'île en van. | [estimé : la coco est le geste d'accueil polynésien standard dès qu'il y a un arrêt dégustation ; les tours sans arrêt n'en servent pas] |
| D'où vient la coco | Jardin familial, cocoteraie d'un proche, achat au producteur ou au bord de route, parfois au marché de Papeete. Pas de fournisseur dédié ; approvisionnement la veille ou le matin même. | [estimé : structures familiales, réseau de proximité ; aucun grossiste en coco jeune connu] |
| Qui la prépare | Le guide ou le capitaine, au coupe-coupe, devant les passagers, souvent intégré à un « show » (ouverture, parfois préparation du lait de coco pour le poisson cru). | [estimé : pratique observable dans la plupart des tours motu] |
| Stade de maturité | Variable : la coco ouverte est celle qu'on a trouvée. Eau parfois fade, parfois trop mûre. Le stade nīā n'est pas un critère explicite de sélection. | [supposé] |
| Coût argent | 0–150 XPF si ramassage / famille ; 150–300 XPF si achat au producteur ou bord de route. | [estimé : prix de détail d'une coco à boire au bord de route 300–500 XPF pour un touriste, donc 150–300 en gros / local] |
| Coût temps | Approvisionnement : 15–45 min par sortie (aller chercher, charger, stocker). Ouverture : 1–2 min par coco, soit 15–40 min de temps de guide par sortie de 15–20 passagers. | [estimé : geste au coupe-coupe par une personne expérimentée] |
| Froid | Rarement. Les cocos voyagent dans la glacière si place, souvent à température ambiante. | [supposé] |
| Hygiène | Pas de process formalisé ; ouverture à la machette sur une coco non lavée, paille ou pas. | [supposé] |
| Ce que le touriste retient | Un bon moment, une photo, « on a bu une coco fraîche ». Rien de nommé, rien d'achetable ensuite, rien qui distingue cet opérateur d'un autre. | [estimé : absence totale de marque sur ce geste] |

**Le point clé pour NĪĀ** : la coco n'est pas un coût majeur ni un problème ressenti par l'opérateur. C'est une habitude bon marché et une partie du spectacle. Le palier 1 ne vend donc pas « moins cher » ni « moins de travail » en premier : il vend **une régularité, une qualité de stade garantie, une présentation qui valorise l'excursion** et une histoire. Le risque n° 3 de la vision (acceptation du prix) est entier.

### 1.2 Faits qui justifient d'agir

**Fréquentation 2025** [estimé : source web — ISPF, bilan tourisme décembre 2025, https://www.ispf.pf/content//uploads/1517_PC_Tourisme_2025_12_9e5f74a421.pdf ; repris par https://outremers360.com/bassin-pacifique-appli/281-227-touristes-en-polynesie-en-2025-lispf-decortique-ce-record-absolu-de-frequentation ; chiffres transmis par le DG, non recoupés sur place].
- **281 227 touristes** en 2025 (+6,6 % vs 2024, record absolu), dont 227 286 en hébergement terrestre (+7,4 %) et 53 941 en tourisme flottant (croisières intra-polynésiennes, charters nautiques).
- **70 062 excursionnistes de croisière** à bord de 32 navires en escale : segment spécifique, escales à Papeete et Moorea, excursions vendues à bord, gros volumes concentrés sur une journée.
- **351 289 visiteurs** au total. Amérique du Nord 42 % des effectifs, métropole deuxième : clientèles habituées aux produits présentés et nommés.
- Chiffre d'affaires des entreprises du tourisme : **217 Mds XPF** (+5,3 %). Le poste « coco » du palier 1, même à 100 M XPF/an de marché théorique, en représente moins de 0,05 % : il est invisible pour l'économie touristique, mais pas pour un opérateur individuel.
- Durée moyenne de séjour : **14–16 nuits**, multi-îles. [estimé : raisonnement, ordre de grandeur habituel des bilans ISPF]
- Part des touristes qui passent par Tahiti : quasi 100 % y transitent, 30–40 % y dorment ; à Moorea : **60–70 %** des touristes y passent. [estimé : raisonnement]

**Taille du geste « coco en excursion ».**
- Nombre d'excursions payantes par touriste terrestre pendant le séjour : **2–4** toutes îles. [supposé]
- Participations annuelles aux excursions sur Tahiti + Moorea (touristes terrestres et flottants) : 281 000 × 3 × 40–50 % de part Tahiti/Moorea ≈ **340 000–420 000**. [estimé : raisonnement]
- Croisiéristes en escale : 70 000 × 0,5–1 excursion par escale à Papeete ou Moorea → **35 000–70 000** participations supplémentaires, concentrées sur des journées d'escale (pics de 500–2 000 passagers à terre le même jour). [estimé : raisonnement]
- Part des excursions où une coco est servie : **30–50 %**. [supposé]
- **Cocos servies en excursion à Tahiti + Moorea : 100 000–250 000 par an** (arrondi du produit des hypothèses ci-dessus). [estimé : raisonnement]
- Recoupement par l'offre : 70–130 prestataires d'excursion actifs sur les deux îles [estimé : raisonnement, § 3.1 ; aucune source publique trouvée par le DG sur ce nombre], dont 40–75 servent une coco, à 10–30 cocos par jour d'activité et 200–250 jours par an → 80 000–280 000 cocos/an. Les deux approches donnent le même ordre de grandeur.
- Le segment croisière est à part : volumes forts et prévisibles (calendrier des escales publié), mais vendus via des agences réceptives, avec des cahiers des charges d'hygiène plus stricts et un cycle de décision plus long. À qualifier après le pilote, pas pour le pilote.

**Saisonnalité.** Haute saison juillet–août et octobre–novembre ; saison des pluies décembre–mars plus creuse (sauf fêtes de fin d'année) ; avril–juin et septembre intermédiaires. Ratio mois creux / mois haut sur les volumes d'excursion : **0,5–0,7**. [estimé : raisonnement] Toute hypothèse de volume du palier 1 doit être exprimée en « cocos par semaine en haute saison » et « en basse saison », pas en moyenne annuelle.

**Pourquoi maintenant.**
- La reprise touristique post-2022 est installée ; les opérateurs ont du volume et des marges pour accepter une petite dépense de différenciation. [estimé]
- Aucune marque de coco jeune n'existe en Polynésie ; le premier qui l'installe chez les opérateurs devient la référence du geste. Fenêtre ouverte, mais pas protégée : la barrière à l'entrée est faible.
- La question du pré-mortem (« pourquoi ça n'existe pas déjà ? ») a trois réponses probables à vérifier : (1) la coco est perçue comme gratuite et banale, donc personne n'a cherché à la vendre « mieux » ; (2) la main-d'œuvre de découpe ne remplit pas un temps plein ; (3) la périssabilité après découpe et la logistique inter-îles découragent. Si l'une de ces réponses est « parce que les opérateurs n'en veulent pas », le palier 1 s'arrête là.

### 1.3 Stratégie et exécution : deux niveaux distincts

| | Formulation de la stratégie | Exécution de première étape (objet de ce business case) |
|---|---|---|
| Énoncé | NĪĀ, l'eau de coco de Polynésie réinventée, commandée à la carte dans un premier cercle de CHR de Tahiti (palier 2). | Palier 1 : des cocos nīā en diamond cut, présentées façon NĪĀ, livrées régulièrement à des opérateurs d'excursion, à marge positive, premières livraisons sous 6 mois. |
| Horizon | 18–36 mois. | 6–12 mois (novembre 2026 → avril/octobre 2027). |
| Succès | Bouteilles vendues, servies et réassorties en CHR. | Un opérateur pilote payant qui réassortit, puis 3–5 opérateurs ; marge par coco positive ; filière apprise ; prix testé. |
| Ce que le palier 1 doit prouver pour la stratégie | — | (a) qu'on sait approvisionner des nīā au bon stade régulièrement ; (b) qu'un client paie plus cher pour une coco « meilleure » ; (c) qu'on tient la chaîne du froid et la conservation ; (d) qu'une présentation NĪĀ crée une réaction chez le consommateur final. |
| Ce que le palier 1 ne prouve pas | — | La durée de vie de l'eau extraite, l'acceptation du prix d'une bouteille en CHR, le rituel de service en salle. Ces sujets restent au palier 2. |
| Signal de dérive | — | Si les décisions du palier 1 (machines, recrutement, volumes) ne servent plus que le diamond cut, le signaler au DG (risque « dérive du palier 1 » de la vision). |

---

## 2. Options

Cinq options, comparées sur ce qu'elles apprennent de la finalité, leur coût en cash et en temps du fondateur, leur risque, leur cohérence de marque et leur réversibilité. Chiffres financiers : renvoi à l'annexe A1.

### Option 0 — Ne rien faire (ou attendre d'avoir levé)

- **Description.** Pas de palier 1 ; le fondateur poursuit la réflexion, cherche un financement sur dossier, lance directement quand il a les moyens.
- **Ce que ça apprend.** Rien sur la filière, rien sur le client, rien sur le prix.
- **Avantages.** Aucun cash engagé ; pas de risque réglementaire ni sanitaire ; temps du fondateur libre.
- **Inconvénients.** Le dossier de levée reste une projection sans client ; aucun financeur local ne s'engage sur une idée de boisson premium sans un début de preuve. L'apprentissage terrain (stades de maturité, producteurs, logistique inter-îles) est reporté, donc le palier 2 aussi.
- **Coût d'opportunité.** Fenêtre : la barrière à l'entrée est faible ; un opérateur bien organisé, une cocoteraie ou un grossiste alimentaire peut installer « la coco découpée livrée » avant NĪĀ et devenir la référence du geste. Apprentissage perdu : 6–12 mois de filière. Réseau : les premiers contacts opérateurs et producteurs ne se font pas.
- **Pré-conditions.** Aucune.

### Option A — Palier 1 manuel, porté par NĪĀ

- **Description.** NĪĀ achète les nīā à une cocoteraie partenaire qui récolte selon le critère de stade écrit ; NĪĀ contrôle à réception, découpe à la main (découpeur à la tâche ou à temps partiel, fondateur formé au geste), stocke au froid, livre l'opérateur pilote, collecte les retours. Tahiti d'abord, un opérateur de Moorea en second si la logistique ferry tient.
- **Ce que ça apprend.** Tout ce que la finalité exige du palier 1 (§ 1.3 a–d) : stade, régularité, geste et temps de découpe réels, perte, conservation, chaîne du froid, réaction des touristes, prix accepté. C'est la mesure du geste manuel qui conditionne l'arbitrage buy or make des machines (vision).
- **Avantages.** Cash minimal (outils, glacières/réfrigérateur, caisses, consommables, assurance ; chiffres en A1) ; démarrable en 2–4 mois ; réversible en une semaine ; chaque coco livrée est une donnée.
- **Inconvénients.** Temps du fondateur très sollicité (approvisionnement, découpe, livraison, vente) ; qualité du diamond cut dépendante d'une personne ; volume plafonné (un découpeur : 20–40 cocos/heure en rythme de croisière [estimé], largement suffisant pour 1–5 opérateurs) ; précarité de l'emploi de découpe.
- **Coût d'opportunité si écartée.** Perte de la seule option qui donne des chiffres réels avant d'investir.
- **Pré-conditions.** Une cocoteraie partenaire d'accord sur le stade et un rythme ; protocole de découpe et conservation testé sur un lot (item 4) ; cadre réglementaire minimal (item 5) ; un opérateur d'accord pour un pilote payant (item 8).

### Option B — Palier 1 avec première machine de découpe

- **Description.** Même modèle que A, mais NĪĀ importe dès le départ une machine de découpe de coco jeune (type « trimmer / diamond cutter » de table) pour garantir la régularité du cut et réduire la main-d'œuvre.
- **Ce que ça apprend.** La même chose que A sur la filière et le client, plus la maîtrise d'une machine (import, maintenance, débit réel). Mais elle fige un choix de machine **avant** d'avoir mesuré le geste manuel, à l'inverse de ce que la vision demande.
- **Avantages.** Régularité visuelle du diamond cut ; argument marque ; moins de dépendance à un découpeur.
- **Inconvénients.** Cash immobilisé (machine, fret, douane, pièces ; A1) sur un volume non prouvé ; délai d'import 2–4 mois [estimé] qui met en risque les 6 mois ; une machine mal choisie pour les nīā locales (taille, fibre) est un coût perdu ; irréversibilité partielle.
- **Coût d'opportunité si écartée.** Faible à court terme : la machine reste accessible plus tard, mieux choisie. Le vrai coût est si le volume décolle et que la découpe manuelle sature ; d'où la bascule conditionnelle (recommandation).
- **Pré-conditions.** Mesures du geste manuel (temps, perte, qualité) ; volume engagé par au moins deux opérateurs ; financement de la machine disponible (cash palier 1 ou sponsor).

### Option C — Découpe sous-traitée à la cocoteraie partenaire ; NĪĀ = marque + logistique + vente

- **Description.** La cocoteraie récolte **et** découpe selon le protocole et la check-list NĪĀ ; NĪĀ contrôle, assure le froid, livre, vend et porte la marque.
- **Ce que ça apprend.** Le client et le prix, la logistique et la marque ; moins la découpe et la conservation, qui passent chez un tiers. Teste un modèle d'organisation (filière intégrée en amont) qui pourrait servir au palier 2 pour l'extraction.
- **Avantages.** Pas de main-d'œuvre de découpe à employer ni à précariser ; cash minimal ; fondateur concentré sur vente et marque ; le découpeur travaille là où sont les cocos (pas de transport de cocos entières).
- **Inconvénients.** Dépendance forte à un partenaire sur la qualité du geste qui fait la marque ; contrôle qualité à distance ; la cocoteraie peut apprendre le métier et vendre directement aux opérateurs (désintermédiation) ; la découpe a lieu dans un lieu non maîtrisé sanitairement.
- **Coût d'opportunité si écartée.** Une organisation plus légère pour Moorea (découpe sur l'île ; les cocos entières relèvent du fret agricole non transformé, pris en charge à 100 % par le Pays selon l'arrêté n° 1586 CM, alors qu'une coco parée n'est éligible qu'au cas par cas [estimé : source web, § 3.6]) ; une relation partenaire plus engagée.
- **Pré-conditions.** Une cocoteraie disposée et équipée (eau, froid, main-d'œuvre) ; protocole écrit et formation ; contrat d'exclusivité ou de non-concurrence sur la découpe de marque ; audit hygiène du lieu.

### Option D — Aller directement au palier 2 (eau de coco premium en bouteille, CHR)

- **Description.** Sauter le diamond cut ; développer la bouteille, l'extraction, la conservation et le rituel ; prospecter les CHR.
- **Ce que ça apprend.** Directement la finalité, mais sans aucune des briques amont (stade, approvisionnement, froid) et avec le risque technique maximal (durée de vie de l'eau extraite, agréments).
- **Avantages.** Pas de « détour » ; cohérence marque totale ; pas de risque de dérive du palier 1.
- **Inconvénients.** Investissement lourd (extraction, conditionnement, labo, agrément ; A1) avant tout client ; 12–24 mois sans chiffre d'affaires [estimé] ; un fondateur seul sans compétence agroalimentaire ; aucun financeur local ne suit sans preuve ; le CHR n'achète pas une promesse de régularité.
- **Coût d'opportunité si écartée.** 6–12 mois de délai sur la finalité, et le risque que le palier 1 absorbe l'énergie. Acceptable si le palier 1 reste borné dans le temps.
- **Pré-conditions.** Financement de 20–50 M XPF [supposé, A1], recrutement production/qualité, faisabilité conservation (item 12).

### Tableau comparatif (1 = défavorable, 5 = favorable)

| Critère | 0 Rien | A Manuel NĪĀ | B Machine | C Cocoteraie découpe | D Palier 2 direct |
|---|---|---|---|---|---|
| Apprentissage filière | 1 — rien n'est appris | 5 — chaque étape mesurée par NĪĀ | 4 — même apprentissage, mais machine choisie à l'aveugle | 3 — découpe et conservation apprises par le partenaire, pas par NĪĀ | 2 — saute l'amont, apprend la finalité au prix fort |
| Cash | 5 — rien engagé | 4 — outils, froid, consommables, assurance (A1) | 2 — machine et import immobilisés avant volume | 4 — pas de main-d'œuvre, mais marge partagée | 1 — investissement lourd sans revenu |
| Risque (exécution, sanitaire, dépendance) | 3 — pas de risque opérationnel, mais fenêtre perdue | 3 — dépend d'une personne et d'un partenaire ; sanitaire maîtrisable | 3 — risque technique machine en plus | 2 — qualité et désintermédiation chez le partenaire | 1 — technique, réglementaire, financier cumulés |
| Délai jusqu'à première livraison | 1 — jamais | 5 — 2–4 mois réalistes | 2 — import 2–4 mois + apprentissage | 4 — dépend de l'équipement du partenaire | 1 — 12–24 mois |
| Cohérence marque | 2 — la marque n'existe pas | 4 — geste maîtrisé, présentation NĪĀ, risque d'irrégularité visuelle | 5 — cut régulier et « signé » | 3 — le geste qui fait la marque est délégué | 5 — la marque est au produit final |
| Réversibilité | 5 — rien à défaire | 5 — arrêt en une semaine | 2 — machine à revendre ou à amortir | 3 — contrat partenaire à dénouer | 1 — investissements spécifiques |
| **Total / 30** | **17** | **26** | **18** | **19** | **11** |

### Recommandation (le DG tranche)

**Option A pour le pilote, avec deux clauses :**

1. **Bascule vers B sur seuil mesuré.** Dès que (a) deux opérateurs réassortissent et (b) le volume hebdomadaire mesuré dépasse ce qu'un découpeur à la tâche produit à qualité stable (seuil à fixer après l'item 4, ordre de grandeur 150–300 cocos/semaine [supposé]) et (c) la marge cumulée ou le sponsor couvre la machine (A1), NĪĀ commande la première machine. C'est exactement « mesurer le geste manuel avant les machines » de la vision.
2. **C testée comme variante, pas comme modèle.** Si la cocoteraie partenaire a l'eau, le froid et une personne disponible, confier un lot de découpe sous protocole NĪĀ et comparer qualité et coût avec la découpe interne. Pertinent surtout pour Moorea : si la coco parée n'obtient pas la prise en charge du fret (§ 3.6), découper sur l'île à partir de cocos entières transportées gratuitement est la voie la moins chère ; si elle l'obtient, A depuis Tahiti suffit. Condition dans les deux cas : le contrôle qualité et la marque restent chez NĪĀ.

**Pourquoi pas les autres.** 0 laisse la fenêtre ouverte à un autre et ne produit aucune preuve pour le financement ; B dépense avant de savoir ; C seule délègue le geste qui fait la marque et crée un futur concurrent ; D demande un financement et des compétences que le projet n'a pas et qu'aucune preuve ne justifie encore.

**Ce que la recommandation ne règle pas et qu'il faut dire au DG.** A repose sur le temps du fondateur. Si le fondateur ne peut pas consacrer 2–3 jours par semaine au terrain pendant 6 mois, A devient C par défaut, et il faut le choisir explicitement plutôt que de le subir.

---

## 3. Marché du palier 1

### 3.1 Segmentation des opérateurs d'excursion

Tous les chiffres de ce tableau sont [estimé : raisonnement] ; le DG n'a trouvé aucune source publique sur le nombre d'opérateurs. La colonne « compatibilité » reprend l'intuition du fondateur (sortie bateau compatible a priori : la coco reste en glacière à bord ; randonnée incompatible : il faudrait porter les cocos pendant la marche). **La matrice de compatibilité détaillée par type d'excursion, les customer journeys et les critères de choix de l'opérateur pilote sont dans l'annexe A5.**

| Segment | Île | Opérateurs actifs | Passagers / sortie | Sorties / jour | Usage actuel du coco | Compatibilité a priori (détail A5) |
|---|---|---|---|---|---|---|
| Lagon / motu avec pique-nique | Moorea | 25–45 | 8–20 | 1–2 | Fort : coco sur le motu, démonstration d'ouverture, lait de coco pour le poisson cru | Oui (bateau, glacière, arrêt long) |
| Lagon / motu | Tahiti (côte ouest, presqu'île, Tetiaroa à la journée) | 10–20 | 8–16 | 1 | Moyen | Oui (bateau) |
| 4x4 intérieur | Tahiti (Papenoo, vallées) | 8–15 | 8–12 | 1–2 | Moyen : arrêt dégustation | Probable (véhicule, glacière) |
| 4x4 / quad intérieur | Moorea (Opunohu, Belvédère, plantations) | 10–20 | 6–12 | 2–3 | Moyen à fort | Probable (4x4) ; à vérifier pour le quad |
| Tour d'île (van, bus) | Tahiti, Moorea | 15–30 | 8–25 | 1–2 | Faible : arrêts courts | Possible, faible valeur |
| Randonnée, canyoning | Tahiti, Moorea | 5–10 | 6–12 | 1 | Faible | Non (portage pendant la marche) |
| Excursions croisière (vendues à bord, exécutées par les opérateurs ci-dessus via agences réceptives) | Papeete, Moorea | — | 20–50 par car / bateau | Jours d'escale | Variable | Oui en lagon / 4x4, mais cycle long ; après le pilote |
| Agences réceptives, desks d'hôtels (prescripteurs) | Tahiti, Moorea | 5–10 | — | — | Revendent ; peuvent imposer un standard | — |
| **Total opérateurs** | | **70–130** | | | **dont 40–75 servent une coco** | |

Lecture : **le cœur du marché est le tour lagon / motu de Moorea**, suivi des 4x4 de Moorea et des tours lagon de Tahiti. Tahiti reste le point de départ (producteurs, découpe, fondateur). Pour Moorea, deux voies : le fret maritime (§ 3.6, prise en charge par le Pays à vérifier) ou la découpe sur l'île (option C).

### 3.2 Taille estimée

- **Marché total Tahiti + Moorea** : 100 000–250 000 cocos/an servies en excursion [estimé, § 1.2]. À un prix NĪĀ de 400–700 XPF/coco [supposé, A1], soit **40–175 M XPF/an** de chiffre d'affaires théorique si tout le marché basculait, ce qui n'arrivera pas.
- **Marché accessible au palier 1** (opérateurs qui servent déjà une coco, ont du volume, un décideur joignable et une logistique compatible) : 15–30 opérateurs, **40 000–100 000 cocos/an**. [estimé]
- **Objectif du palier 1** : 1 opérateur pilote (10–30 cocos/jour, 5–6 jours/semaine → **60–180 cocos/semaine** en haute saison, moitié en basse), puis 3–5 opérateurs à 12 mois (**200–600 cocos/semaine**). Soit 2–5 % du marché accessible. Ce volume est celui qui dimensionne la découpe, le froid et la trésorerie (A1).

### 3.3 Décideur et cycle de décision

- **Décideur** : dans 80 % des cas le propriétaire-exploitant, souvent lui-même capitaine ou guide ; structures familiales de 1–5 personnes. [estimé] Dans les structures plus grosses ou adossées à un hôtel : le gérant ou le responsable des activités.
- **Prescripteurs** : les agences réceptives et desks d'hôtels qui revendent les excursions et peuvent valoriser « coco NĪĀ incluse » dans leur descriptif ; les guides, qui décident de ce qui se passe à bord.
- **Cycle** : court. Première rencontre sur le quai ou au retour d'une sortie, dégustation d'un échantillon, proposition de pilote, décision en 2–6 semaines et 2–3 contacts. [estimé] Pas d'appel d'offres ni de référencement formel. Le meilleur moment pour prospecter : saison intermédiaire (avril–juin 2027 pour un démarrage, ou dès décembre 2026 pour préparer la haute saison de juillet).
- **Paiement** : à la livraison ou hebdomadaire, en espèces ou virement ; attendre des délais de paiement courts mais une discipline variable. [supposé] Le pilote doit fixer la règle de paiement dès le départ (KPI délai de paiement).

### 3.4 Prix de référence actuel et coût complet

| Poste | Fourchette XPF / coco | Marquage |
|---|---|---|
| Coco brute, famille / ramassage | 0–150 | [estimé] |
| Coco brute, achat au producteur ou bord de route (gros) | 150–300 | [estimé : détail touriste 300–500] |
| Temps de guide pour approvisionner (15–45 min / sortie, 15 cocos, valorisé 1 500–2 500 XPF/h) | 25–125 | [estimé] |
| Temps de guide pour ouvrir (1–2 min / coco) | 25–85 | [estimé] |
| Perte (cocos trop mûres, vides, abîmées : 10–20 %) | 15–60 | [supposé] |
| **Coût complet actuel pour l'opérateur** | **250–450** | [estimé : somme des lignes] |
| Prix de l'excursion par passager | 5 000–15 000 | [estimé : 4x4 5 000–8 000 ; lagon demi-journée 7 000–9 000 ; lagon journée pique-nique 9 000–15 000] |
| Poids de la coco dans le prix de l'excursion | 2–6 % | calcul |

**Conséquence pour le prix NĪĀ.** Un prix de 400–700 XPF livrée froide et découpée [supposé, à tester ; chiffre d'A1] représente un **surcoût de 0–300 XPF par passager**, soit 0–3 % du prix de l'excursion, contre un gain de temps de guide, une qualité garantie et un argument commercial. L'hypothèse à tester n'est pas « l'opérateur peut-il payer » (il peut) mais « voit-il une valeur pour laquelle payer » (il ne la voit pas encore). Le prix est une hypothèse, pas une variable d'ajustement : on teste un prix, on note la réaction mot pour mot, on ne le casse pas pour signer.

### 3.5 Saisonnalité et conséquence sur l'offre

- Volumes d'excursion : haut juillet–août et octobre–novembre ; creux décembre–mars ; ratio 0,5–0,7. [estimé]
- Côté offre, la production de cocos est relativement continue mais la récolte au stade nīā exige des passages réguliers ; météo et houle (saison des pluies) perturbent récolte, ferry et sorties lagon. [supposé]
- Conséquence : une offre « à la commande, livrée J-1 ou J, sans engagement de volume mensuel » pour le pilote ; un engagement de volume minimum seulement une fois la saisonnalité mesurée sur un cycle.

### 3.6 Contrainte logistique

- **Horaires** : les sorties partent entre 8 h et 9 h 30 ; livraison la veille en fin de journée (dans un réfrigérateur chez l'opérateur) ou le matin avant 7 h 30 sur le quai / au local. [estimé]
- **Froid à bord** : glacières ; peu de réfrigération. La coco NĪĀ doit tenir 4–8 h en glacière après sortie du froid [supposé, à tester item 4].
- **Conditionnement** : caisses de 10–20, empilables, lavables, avec couvercle ; chaque coco protégée en pointe (le diamond cut est fragile et la surface ouverte doit rester propre, filmée ou capuchonnée). [supposé]
- **Moorea** : ferry Papeete–Vaiare, 30–45 min, plusieurs rotations par jour, fret possible ; rupture de chaîne du froid à mesurer ; alternative : découpe sur Moorea (option C) ou un point froid relais à Vaiare. [estimé : raisonnement]
- **Coût du fret inter-îles.** Information du fondateur : le fret inter-îles des produits agricoles serait gratuit ou pris en charge par le Pays [supposé, à vérifier sur Lexpol]. Précision apportée par le DG : arrêté n° 1586 CM du 13/09/2023 (modifié mai 2026), le Pays prend en charge **100 % du fret maritime des produits agricoles non transformés**, des îles vers Tahiti et entre îles ; les **produits transformés sont traités au cas par cas** ; bénéficiaires : titulaires de la carte CAPL ou sociétés inscrites au RCS [estimé : source web, https://www.service-public.pf/dgae/aides/prise-en-charge-du-fret-maritime-par-le-pays/ ; texte non lu dans Lexpol]. Conséquences : (a) une **coco entière** voyage probablement gratuitement, ce qui favorise l'option C (découpe à Moorea à partir de cocos de Tahiti, ou d'une cocoteraie de Moorea) ; (b) une **coco parée diamond cut est probablement un produit transformé**, donc éligible seulement au cas par cas : à demander à la DGAE avant de dimensionner Moorea ; (c) si l'éligibilité est obtenue, Moorea puis d'autres îles touristiques (Bora Bora, Raiatea, Huahine) deviennent accessibles au même coût de transport que Tahiti, et le ratio Moorea / Tahiti de la segmentation bascule en faveur de Moorea dès le deuxième opérateur. Le froid pendant le transport reste à notre charge dans tous les cas.
- **Retours** : récupération des caisses et des invendus ; la coco non servie dans la DLC est perdue ou retournée.

### 3.7 Risque d'internalisation

Un opérateur peut copier le geste : acheter des cocos jeunes, les découper, les mettre au froid. Ce qui l'en empêche aujourd'hui, et que NĪĀ doit rendre durable :
- il n'a ni le temps ni la régularité d'approvisionnement au bon stade (c'est le vrai savoir-faire : la sélection nīā chez le producteur) ;
- la découpe diamond cut propre et régulière demande un geste et un outillage qu'il n'a pas ;
- la marque et le texte dit au passager ne se copient pas ; la coco NĪĀ est une coco **nommée** ;
- le service (livraison, reprise des caisses, régularité, hygiène documentée) est une charge mentale qu'il ne veut pas.
Signal d'alerte : un opérateur qui demande « où achetez-vous vos cocos ? » et « quel outil utilisez-vous ? » à la deuxième rencontre. Réponse : rester transparent sur la qualité, discret sur les sources et le geste, et faire porter la valeur sur la régularité et la marque.

### 3.8 Proposition de valeur pour l'opérateur

**En une phrase** : « Vous servez déjà une coco ; servez une NĪĀ : une coco jeune au bon stade, découpée, froide, livrée quand vous partez, avec une histoire à raconter à vos passagers ; sans aller la chercher ni l'ouvrir. »

| Bénéfice | Ce que ça change pour lui | Preuve à apporter |
|---|---|---|
| Régularité | Le bon nombre de cocos, chaque sortie, sans courir le matin | Taux de livraison à l'heure du pilote |
| Qualité du stade nīā | Une eau sucrée, pas une coco fade ou mûre ; zéro coco vide devant les passagers | Taux de rejet qualité, verbatims passagers |
| Hygiène et froid | Une coco lavée, découpée proprement, froide ; un argument face à des clientèles exigeantes | Protocole écrit, DLC, étiquette |
| Présentation | Le diamond cut façon NĪĀ, photographié, partagé | Observation des passagers (photos, questions) |
| Temps gagné | 30–60 min de temps de guide par sortie récupérés | Mesure avant / après avec le guide |
| Histoire | Le guide raconte le nīā, le stade, la fierté polynésienne ; l'excursion gagne un « moment » | Texte FR/EN fourni (item 7) |
| Différenciation commerciale | « Coco NĪĀ incluse » dans son descriptif, face à des concurrents identiques | Mention sur ses supports, retours des agences |

### 3.9 Objections attendues et réponses

| Objection (telle qu'on l'entendra) | Réponse | Ce qu'elle nous apprend si elle revient souvent |
|---|---|---|
| « On a déjà des cocos, ça nous coûte rien. » | « Elles vous coûtent le temps du guide et les cocos ratées. Testons 2 semaines sur une sortie, vous comparez. » | Le prix sera dur à tenir ; la valeur doit être démontrée sur l'expérience passager, pas sur le coût. |
| « C'est trop cher pour une coco. » | « C'est 2–3 % de votre excursion pour le moment que vos passagers photographient. On ne baisse pas le prix, on vous laisse mesurer. » | Si > 50 % des opérateurs la disent après dégustation, le prix d'A1 est à revoir **ou** la cible est la mauvaise. Remonter au DG. |
| « Ouvrir la coco devant les touristes, c'est le show. » | « Gardez le show : la NĪĀ arrive découpée, le guide fait le geste final d'ouverture et raconte le nīā. On fournit le texte. » | La présentation doit laisser un geste au guide : contrainte pour le brand-director. |
| « Et si vous ne livrez pas un matin ? » | « Livraison la veille au froid, un stock tampon de X cocos, et votre ancien circuit reste en secours pendant le pilote. » | La régularité est le premier critère de rétention : KPI livraisons à l'heure. |
| « Combien de temps ça se garde ? » | « Donnée mesurée sur lot, DLC écrite sur l'étiquette ; on reprend ce qui n'est pas servi dans la DLC. » | La DLC est une condition de vente, pas un détail (item 4, item 5). |
| « On peut le faire nous-mêmes. » | « Oui. La question est si vous voulez chercher des cocos au bon stade tous les jours. Nous, c'est notre métier. » | Internalisation : surveiller qui pose la question (§ 3.7). |
| « Mes passagers ne verront pas la différence. » | « Testons : on observe deux sorties avec et deux sans, on compte photos et questions. » | Si vrai, le laboratoire de marque échoue : information majeure pour le palier 2. |
| « Je ne veux pas d'un réfrigérateur de plus. » | « Livraison le matin en caisse isotherme, ou prêt d'une glacière dédiée NĪĀ. » | Dimensionne la logistique et le coût par coco livrée. |

### 3.10 Choix de l'opérateur pilote

Les critères de choix, la grille de notation et les customer journeys par type d'excursion sont dans l'**annexe A5** (market-scout). Deux principes non négociables du point de vue business, quels que soient les critères retenus : l'opérateur **sert déjà une coco à chaque sortie** (on ne crée pas l'usage, on le remplace), et le pilote est **payant** au prix d'A1 ; un opérateur gratuit « pour tester » n'est pas un pilote, c'est la seule mesure du prix qui serait perdue.

---

## 4. Critères de valeur mesurables (KPI du pilote)

| KPI | Définition | Cible pilote | Méthode | Fréquence | Qui mesure |
|---|---|---|---|---|---|
| Taux de réassort | Semaines où l'opérateur recommande / semaines du pilote | ≥ 80 % sur 8–12 semaines ; 100 % les 4 dernières | Journal de commandes | Hebdo | Fondateur |
| Volume livré | Cocos livrées / semaine, haute et basse saison distinguées | Conforme au volume annoncé ± 20 % | Bons de livraison | Hebdo | Fondateur |
| Marge brute par coco livrée | Prix − coût complet par coco (achat, découpe, froid, transport, perte, emballage) ; chiffre A1 | > 0 dès le mois 2 ; cible A1 | Comptabilité simple par lot | Mensuel | Fondateur + financial-modeler |
| Coût par coco livrée | Toutes charges variables / cocos livrées | Trajectoire baissière mois après mois ; cible A1 | Idem | Mensuel | Fondateur |
| Livraisons à l'heure | Livraisons à l'heure convenue / livraisons | ≥ 95 % ; 0 sortie sans coco | Bon signé avec heure | Chaque livraison | Opérateur (signature) |
| Taux de rejet qualité à réception des nīā | Cocos refusées à la check-list / cocos reçues de la cocoteraie | < 10 % au mois 3 | Check-list réception | Chaque lot | Fondateur / découpeur |
| Cocos perdues | Cocos non servies dans la DLC + abîmées en transport / cocos découpées | < 5 % | Comptage retours | Hebdo | Fondateur |
| Rejet par l'opérateur ou le passager | Cocos refusées au service (fade, mûre, sale, cut raté) / cocos servies | < 2 % | Fiche de sortie remplie par le guide | Chaque sortie | Guide |
| Satisfaction opérateur | Note sur 5 + 3 verbatims cités | ≥ 4/5 ; verbatims consignés mot pour mot | Entretien court | Toutes les 2 semaines, puis fin de pilote | Fondateur |
| Réaction des touristes observée | Photos prises, questions posées, mention du nom NĪĀ | Observation sur ≥ 4 sorties ; tendance « avec / sans » | Grille d'observation à bord, 10 lignes | 2 sorties/mois | Fondateur ou guide |
| Délai de paiement | Jours entre livraison et encaissement | ≤ 7 jours | Relevé | Mensuel | Fondateur |
| Temps de guide gagné | Minutes par sortie avant / après | ≥ 20 min | Déclaratif guide, 2 mesures | Début et fin de pilote | Guide |

**Pourquoi pas de CSAT / NPS grand public.** Le touriste n'est pas le client de NĪĀ au palier 1 (la coco est incluse, il ne l'achète pas) ; un questionnaire en excursion gêne l'opérateur, biaise un échantillon minuscule et mesure l'excursion plus que la coco. On remplace par **deux mesures légères** : (1) la grille d'observation à bord (photos, questions, « c'est quoi NĪĀ ? », cocos finies ou laissées) ; (2) une question unique posée par le guide à la fin de la sortie quand c'est naturel : « la coco, vous l'avez aimée ? » avec comptage oui / bof / non sur la fiche de sortie. Ces mesures servent le laboratoire de marque, pas la décision de poursuivre : celle-ci repose sur le réassort et la marge.

**Règle de décision à la fin du pilote (12 semaines).** Poursuivre vers 3–5 opérateurs si : réassort ≥ 80 %, marge brute par coco > 0, livraisons à l'heure ≥ 95 %, satisfaction ≥ 4/5. Revoir le prix ou la cible si l'opérateur réassortit mais la marge est négative. Arrêter ou pivoter (option C, ou retour au DG) si l'opérateur ne réassortit pas malgré une livraison fiable.

---

## 5. Registre des parties prenantes

| Partie prenante | Intérêt | Influence | Attentes | Attitude probable | Stratégie d'engagement |
|---|---|---|---|---|---|
| Fondateur | Prouver la finalité ; apprendre la filière ; ne pas s'épuiser | Décisive | Un pilote payant sous 6 mois ; des chiffres réels | Engagé, à risque de dispersion (digital) | Cadrage par le DG et le challenger ; 2–3 jours terrain / semaine protégés |
| Sponsor / investisseur à trouver | Rendement ou intérêt stratégique ; limiter sa perte | Forte (financement palier 1 → 2) | Preuves : commande, marge, réassort ; reporting court et honnête | Prudent, curieux si proche de la filière ou du tourisme | Point mensuel, tableau de bord à 6 KPI, seuils de décision annoncés (§ 9) |
| Cocoteraie partenaire | Débouché régulier et payé pour des cocos jeunes (moins de valeur en coprah) ; nouvelle recette | Forte (risque n° 1) | Volume prévisible, prix juste, paiement rapide, critère de stade clair | Intéressée mais sceptique sur la régularité de la demande | Critère nīā écrit ensemble ; engagement de volume progressif ; paiement à réception ; visite hebdo |
| Découpeur (à la tâche / temps partiel) | Revenu complémentaire stable ; reconnaissance du geste | Moyenne (qualité du cut) | Volume lisible, rémunération à la pièce ou à l'heure, outillage, horaires compatibles | Disponible si le rythme est clair | Contrat simple, grille de rémunération, formation, photo de référence du cut |
| Opérateur pilote | Différenciation, temps gagné, fiabilité ; ne pas se compliquer la vie | Forte (le client) | Zéro raté, prix tenable, souplesse de commande | Ouvert à l'essai, réticent au prix | Pilote payant borné (8–12 semaines), stock tampon, retour toutes les 2 semaines |
| Opérateurs suivants | Idem ; ne pas être le premier | Moyenne | Preuve par le pilote, référence d'un pair | Attentistes | Témoignage du pilote, dégustation sur le quai, offre en saison intermédiaire |
| Guides / équipages | Moins de corvée, un moment valorisant à bord, fierté | Forte sur l'usage réel | Garder un geste, texte simple, pas de contrainte froide lourde | Alliés si consultés, résistants si imposé | Les associer dès la première rencontre ; fiche de sortie courte ; les nommer dans les retours |
| Touristes | Un bon moment, authentique, photogénique | Indirecte (via l'opérateur) | Fraîcheur, goût, propreté, une histoire | Positifs si le produit est bon | Observation, pas d'enquête ; texte du guide FR/EN |
| Services du Pays : hygiène (CHSP), agriculture (DAG), création d'entreprise (CCISM, DGAE) | Conformité sanitaire, filière agricole locale, création d'emploi | Forte (autorisation) | Déclaration d'activité, règles d'hygiène, étiquetage/DLC, patente | Neutre à favorable (produit local, emploi) | Rendez-vous d'information avant la première livraison (item 5) ; dossier simple ; demander plutôt que supposer |
| Transporteurs (route, ferry Papeete–Moorea) et DGAE (prise en charge du fret) | Fret payé (par NĪĀ ou par le Pays selon l'éligibilité, § 3.6) | Moyenne (Moorea et autres îles) | Caisses conformes, horaires ; pour la DGAE : statut agricole / transformé de la coco parée, carte CAPL ou RCS | Indifférents ; DGAE neutre | Tester un envoi fret avec sonde de température avant d'engager un opérateur de Moorea ; demander par écrit l'éligibilité de la coco parée |
| Banque / financeur (prêt d'honneur, microcrédit, banque locale) | Remboursement ; dossier solide | Moyenne à forte | Apport, pilote, chiffres | Prudents | Dossier après pilote, pas avant ; A1 comme pièce |
| Futurs CHR (palier 2) | Une boisson locale premium à la carte ; mais pas maintenant | Faible au palier 1 | Rien à ce stade ; ne pas être sollicités trop tôt | Curieux | Observer, noter, ne pas vendre (anti-pattern) ; 2–3 conversations informelles pour écouter |
| Communauté polynésienne (familles, producteurs, voisinage) | Fierté d'une ressource valorisée ; crainte d'une « marque » sur un bien commun | Diffuse mais réelle (réputation) | Respect, prix juste au producteur, pas de folklore | Bienveillante si le ton est juste, critique si exotisme ou appropriation | Ton de marque (fierté, pas exotisme) ; nommer le stade nīā en tahitien ; payer les producteurs correctement et le dire |

---

## 6. Plan de communication

| Partie prenante | Quoi | Quand | Canal | Qui |
|---|---|---|---|---|
| Sponsor | Tableau de bord 6 KPI (réassort, volume, marge/coco, livraisons à l'heure, pertes, trésorerie), décisions à prendre, risques | **Mensuel**, 45 min ; point flash si seuil franchi | Réunion + une page écrite | Fondateur |
| DG / équipe projet (repo) | Journal de pilote, décisions, hypothèses vérifiées ou invalidées | Hebdo (`/status`), revue de sprint | Markdown `scrum/`, `docs/notes/` | Fondateur / business-director |
| Cocoteraie | Commande de la semaine, retour qualité du lot (check-list), paiement | Hebdo, le même jour | Visite ou appel + message écrit | Fondateur |
| Découpeur | Planning, volume, retour qualité du cut, paie | Hebdo ; feedback à chaque lot | Oral + photo de référence | Fondateur |
| Opérateur pilote | Confirmation de commande J-1, bon de livraison, point de satisfaction | Chaque livraison ; entretien toutes les 2 semaines ; bilan fin de pilote | Message J-1, bon signé, entretien 20 min au retour d'une sortie | Fondateur |
| Guides | Texte NĪĀ FR/EN, fiche de sortie, remerciement nominatif | Démarrage, puis à chaque évolution | En main propre, à bord | Fondateur + brand-director (texte) |
| Opérateurs suivants | Dégustation, chiffres du pilote (avec accord du pilote), offre | Saison intermédiaire suivant le pilote | Quai, local, bouche-à-oreille | Fondateur |
| Services du Pays | Déclaration, questions, mise en conformité | Avant première livraison ; puis à chaque changement (Moorea, machine) | Rendez-vous, courrier | Fondateur / operations-director |
| Transporteurs | Test fret, horaires | Avant Moorea | Guichet | Fondateur |
| Banque / financeur | Dossier avec résultats du pilote | Après 12 semaines de pilote | Rendez-vous | Fondateur + financial-modeler |
| Futurs CHR | Écoute, pas de vente | Opportuniste | Conversation | Fondateur |
| Communauté | Nom, stade nīā, provenance, prix payé au producteur | Dès la première présentation publique du produit | Bouche-à-oreille, étiquette, texte du guide ; pas de réseaux sociaux avant le second temps | Brand-director |

**Cadence des points sponsor.** Mensuelle, calée sur la clôture du tableau de bord. Un point intermédiaire de 15 minutes si un seuil est franchi.

**Déclencheurs d'escalade (au sponsor et au DG, sous 48 h).**
- Deux livraisons manquées ou en retard dans le même mois.
- Rupture d'approvisionnement cocoteraie > 1 semaine, ou taux de rejet à réception > 25 % sur deux lots.
- Incident sanitaire ou plainte passager liée à une coco.
- Marge brute par coco négative deux mois consécutifs après le mois 2.
- L'opérateur pilote ne réassortit pas deux semaines de suite sans raison saisonnière.
- Un tiers (opérateur, cocoteraie, grossiste) commence à livrer des cocos découpées.
- Trésorerie sous un mois de charges (seuil chiffré en A1).

---

## 7. Conduite du changement chez l'opérateur pilote

L'opérateur change une habitude ancrée et quasi gratuite : il ne va plus chercher ses cocos et ne les ouvre plus lui-même, ou il quitte un fournisseur familial. Cinq leviers, courts et concrets :

1. **Sentiment d'urgence (sans dramatiser).** Montrer, pas dire : une dégustation côte à côte, sa coco du jour contre une NĪĀ froide au bon stade. Puis une question : « combien de cocos ratées la semaine dernière ? combien de minutes à les chercher ? ». L'urgence vient de la saison haute qui approche et de la clientèle qui compare les excursions en ligne.
2. **Coalition : le patron et le guide.** Ne jamais signer avec le patron sans le guide. Le guide garde un geste (l'ouverture finale, le texte) et devient le témoin du gain de temps ; le patron tient le prix. Un seul des deux, et l'habitude revient à la première livraison compliquée.
3. **Vision.** « Votre excursion a un moment que les autres n'ont pas, et il a un nom. » Le texte FR/EN de 30 secondes fourni par NĪĀ (item 7) est la vision incarnée.
4. **Quick wins.** Semaine 1 : zéro coco à chercher le matin. Semaine 2 : premières photos de passagers avec la coco, montrées au patron. Semaine 4 : fiche de sortie avec « 0 coco ratée ». Rendre chaque gain visible avec un chiffre.
5. **Ancrage.** Au bout de 8 semaines : la coco NĪĀ figure dans son descriptif d'excursion ; une routine de commande fixe (même jour, même heure, même message) ; le guide dit le texte sans y penser ; l'ancien circuit n'est plus activé. Témoignage cité, avec son accord, pour les opérateurs suivants.

Ce qui fera échouer la conduite du changement : une livraison manquée dans les 3 premières semaines, un cut irrégulier devant les passagers, ou un prix négocié à la baisse qui dévalorise le produit avant même qu'il soit servi.

---

## 8. Elevator pitch de la charte (6 lignes)

1. **Problème / opportunité.** Chaque jour, des dizaines d'opérateurs d'excursion de Tahiti et Moorea servent à leurs passagers une coco quelconque, cherchée le matin et ouverte au coupe-coupe : 100 000 à 250 000 cocos par an sans marque, sans stade garanti, sans histoire [estimé].
2. **Idée.** NĪĀ livre aux opérateurs des cocos nīā, au stade exact où l'eau est la plus sucrée, découpées en diamond cut, froides, présentées façon NĪĀ, avec le texte que le guide raconte.
3. **Avantage.** Pour l'opérateur : régularité, qualité, temps de guide gagné, un moment distinctif dans son excursion ; pour NĪĀ : un laboratoire de marque rémunéré qui prépare l'eau de coco premium à la carte des CHR.
4. **Équipe.** Un fondateur chef de projet, profil tech, qui apprend la filière sur le terrain ; une cocoteraie partenaire qui récolte ; un découpeur à la tâche ; un sponsor à trouver qui connaît la coco ou le tourisme.
5. **Coût / bénéfice.** Apport fondateur 2–5 M XPF ; besoin complémentaire, coût de revient, prix, marge, point mort et VAN du palier 1 : voir **annexe A1**. Critère de succès : un opérateur qui paie et réassortit, marge par coco positive.
6. **Planning.** Novembre 2026 : partenaires et protocole ; janvier–février 2027 : lot test, cadre réglementaire, opérateur signé ; **premières livraisons avant mai 2027** ; pilote 12 semaines ; décision 3–5 opérateurs et première machine à l'été 2027 ; palier 2 instruit en parallèle.

---

## 9. Modes de financement et profil du sponsor

### 9.1 Besoins et sources, par ordre de préférence

| Source | Pour quoi | Ordre de grandeur | Conditions | Marquage |
|---|---|---|---|---|
| Apport du fondateur | Palier 1 complet en option A (outillage, froid, consommables, assurance, stock tampon, déplacements) | 2–5 M XPF, chiffre A1 | Décision prise | [décision fondateur] |
| Cash du palier 1 | Réassort, puis première machine | Marge cumulée du pilote, A1 | Marge par coco positive | [A1] |
| Apport en nature d'un associé terrain | Accès cocoteraie, local avec eau et froid, véhicule, réseau d'opérateurs | Équivalent 1–3 M XPF | Pacte simple, part du capital ou rémunération variable | [supposé] |
| Prêt d'honneur / microcrédit (réseaux locaux d'aide à la création type Initiative, ADIE, dispositifs du Pays) | Première machine, fonds de roulement | 1–5 M XPF | Dossier après pilote, patente, apport | [supposé : dispositifs existants en Polynésie française, montants à vérifier] |
| Investisseur local (business angel, entrepreneur du tourisme ou de l'agroalimentaire) | Passage à 3–5 opérateurs, première machine, préparation palier 2 | 5–15 M XPF | Preuves du pilote ; participation minoritaire | [supposé] |
| Banque locale | Palier 2 (extraction, conditionnement) | 20–50 M XPF | Deux cycles de pilote, bilan, garanties | [supposé, A1] |
| Aides du Pays à l'agro-transformation et à la création d'entreprise | Co-financement machine, formation | Variable | Éligibilité à vérifier (item 5 / item 10) | [supposé] |
| Prise en charge du fret maritime inter-îles par le Pays (arrêté n° 1586 CM) | Transport Tahiti → Moorea et autres îles | 100 % du fret pour produits agricoles non transformés ; cas par cas pour les transformés | Carte CAPL ou RCS ; statut de la coco parée à faire qualifier par la DGAE | [estimé : source web, § 3.6] |

Règle : **ne pas chercher d'argent externe avant d'avoir un pilote payant signé**. Le dossier change de nature à ce moment-là : il passe d'une idée à une activité.

### 9.2 Qui a intérêt à sponsoriser, et quel deal

| Profil | Pourquoi il a intérêt | Ce qu'on lui demande | Ce qu'on lui offre | Seuils de décision qu'il tiendra |
|---|---|---|---|---|
| **Associé terrain** (connaît la coco, la pêche ou le tourisme ; a un local, un véhicule, un réseau) | Valoriser ce qu'il a déjà ; participer à une marque dont il peut être fier | 2–3 jours/semaine, apport en nature, réseau | Part du capital, rémunération variable sur la marge, co-fondateur opérationnel | Un opérateur signé ; marge par coco positive ; sa place écrite |
| **Cocoteraie partenaire** | Débouché à meilleure valeur que le coprah pour des cocos jeunes ; volume régulier | Récolte au stade nīā, éventuellement découpe (option C), prix stable, exclusivité de la découpe de marque | Volume engagé progressif, paiement rapide, part du prix ou prime à la qualité, visibilité (« nīā de [vallée] ») | Volume hebdo stable 3 mois ; paiement à l'heure |
| **Investisseur local** (entrepreneur, famille d'affaires du tourisme ou de l'agroalimentaire) | Rendement, diversification, image « produit local premium » | 5–15 M XPF en 2 tranches, conseil, réseau CHR pour le palier 2 | Participation minoritaire, tableau de bord mensuel, option sur le palier 2 | Tranche 1 : pilote payant + marge positive mesurée ; tranche 2 : deuxième opérateur qui réassortit et coût par coco en baisse |
| **Opérateur d'excursion** (un gros acteur ou un groupement) | Exclusivité temporaire sur son île ou son segment ; différenciation | Engagement de volume, préfinancement d'un stock ou d'une glacière, témoignage | Exclusivité limitée dans le temps et le segment, prix stable, co-marquage discret | Zéro raté sur 4 semaines ; réaction des passagers observée |

**Profil recherché en priorité** : l'associé terrain ou l'investisseur local **proche de la filière ou du tourisme**, parce qu'il apporte ce qui manque au fondateur (le métier et le réseau) et parce qu'il comprend des seuils de décision formulés en commandes et marges. Un financeur purement financier arrivera après le pilote, sur dossier A1 mis à jour avec des chiffres relevés.

**Ce qu'on ne fait pas.** Pas de sponsor qui impose une revente au touriste, une grande surface, un export, ou une baisse de prix pour « faire du volume » : ce sont les non-objectifs de la vision.

---

## Les 5 choses à vérifier sur le terrain avant de signer un opérateur

1. **Il sert vraiment une coco à chaque sortie, et combien.** Compter sur deux sorties, pas croire le déclaratif. Noter d'où viennent ses cocos et ce qu'elles lui coûtent réellement (argent et minutes de guide).
2. **Pourquoi personne ne le lui propose déjà.** Poser la question au patron, au guide et au producteur ; si la réponse est « on nous l'a proposé et on a refusé », comprendre pourquoi avant toute offre.
3. **Le froid, l'horaire et le fret tiennent.** Où la coco passera la nuit, à quelle heure elle doit être sur le quai, combien d'heures elle restera en glacière ; une livraison test à blanc avec une sonde de température. Pour un opérateur hors Tahiti : **vérifier sur Lexpol et auprès de la DGAE** (arrêté n° 1586 CM) si une coco parée diamond cut est éligible à la prise en charge du fret maritime par le Pays, ou seulement la coco entière ; la réponse décide entre livrer depuis Tahiti et découper sur l'île.
4. **Le prix est dit à haute voix et accepté.** Annoncer le prix d'A1 après dégustation, noter la réponse mot pour mot, ne pas le baisser ; un pilote gratuit ne vaut rien.
5. **Le guide est d'accord.** Il garde un geste et un texte ; s'il n'y est pas, l'habitude reviendra à la première difficulté, quel que soit l'accord du patron.
