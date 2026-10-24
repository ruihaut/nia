# Charte de projet — NĪĀ, palier 1

> **Statut : v0, soumise à l'approbation du sponsor et du chef de projet.** Rédigée le 2026-10-24 par le Director-General. Découle du business case (`docs/01-business-case.md`) ; le plan détaillé est dans `docs/03-project-management-plan.md`. Cette charte cadre et fait accepter la mission à haut niveau ; elle ne remplace pas le plan.

---

## 1. Elevator pitch

1. **Problème / opportunité.** Chaque jour, des dizaines d'opérateurs d'excursion de Tahiti et Moorea servent à leurs passagers une coco quelconque, cherchée le matin et ouverte au coupe-coupe : 100 000 à 250 000 cocos par an sans marque, sans stade garanti, sans histoire [estimé].
2. **Idée.** NĪĀ livre aux opérateurs des cocos *nīā*, au stade exact où l'eau est la plus agréable, découpées en diamond cut, froides, marquées NĪĀ, avec les mots que le guide dit à ses passagers.
3. **Avantage.** Pour l'opérateur : régularité, qualité du stade, hygiène, temps de guide gagné, un moment distinctif dans son excursion. Pour NĪĀ : un laboratoire de marque rémunéré qui apprend la filière et prépare l'eau de coco premium à la carte des CHR.
4. **Équipe.** Un fondateur chef de projet, profil tech, qui apprend le métier sur le terrain ; une cocoteraie partenaire qui récolte ; un découpeur à la tâche ; une équipe d'agents r-stack qui instruit et documente ; un sponsor à trouver qui connaît la coco ou le tourisme.
5. **Coût / bénéfice.** Apport du fondateur 2–5 M XPF ; besoin de 2,3–2,5 M disponibles pour l'option retenue ; coût de revient ≈ 350 XPF, prix cible 500 XPF, marge ≈ 150 XPF par coco, point mort ≈ 500 cocos par mois ; VAN du palier 1 seul négative au scénario réaliste (−0,84 M), positive au scénario optimiste (+0,47 M). Le bénéfice est l'option sur le palier 2 et les chiffres réels que le pilote produit. Détail : business case § 3.
6. **Planning.** Novembre–décembre 2026 : vérifications (conservation, cocoteraies, opérateurs, CHSP, fret). 4 janvier 2027 : go financement. Février–mars : cocoteraie signée, protocole et DLC validés, opérateur pilote signé, conformité. **Première livraison payante la semaine du 5 avril 2027, au plus tard le 30 avril.** Septembre 2027 : fin du pilote et PV de recette. Octobre 2027 : décision palier 2.

---

## 2. But du projet et résultats recherchés

**But.** Prouver sur le terrain, en douze mois et pour moins de 3 M XPF, que NĪĀ sait approvisionner des cocos nīā au bon stade, les transformer et les livrer froides avec une qualité constante, et qu'un client professionnel paie plus cher pour cela ; apprendre la filière et installer la marque chez ses premiers clients, au service de la finalité de `VISION.md` (NĪĀ à la carte des CHR de Tahiti).

**Résultats recherchés à la fin du pilote (septembre–octobre 2027).**

| Résultat | Critère de succès | Mesure |
|---|---|---|
| Un client payant qui reste | Opérateur pilote livré ≥ 20 semaines ; réassort ≥ 80 % des semaines ; PV de recette signé sans réserve bloquante | Journal de commandes, PV (plan § 4) |
| Une économie unitaire positive | Marge brute par coco livrée > 0 dès le deuxième mois de livraison ; coût par coco relevé ≤ 350 XPF ; prix ≥ 450 XPF accepté | Comptabilité par lot |
| Une filière apprise et transmissible | Fiche de sélection nīā, fiches fournisseurs, protocole de découpe, plan d'hygiène et chaîne du froid écrits, exécutés au moins une fois par quelqu'un d'autre que leur auteur | Definition of Done (plan § 4) |
| Une conformité acquise | Récépissé ou attestation du CHSP, RC professionnelle couvrant denrées et livraison, étiquetage et DLC justifiée | Jalon J4 |
| Une marque qui commence | Le nom NĪĀ dit par un guide et par des passagers sans qu'on le leur souffle ; marquage lisible en fin d'excursion sur ≥ 95 % des cocos | Grille d'observation à bord |
| Un dossier de décision pour le palier 2 | Bilan chiffré en [relevé], note buy or make, enseignements pour l'eau extraite, recommandation continuer / étendre / arrêter | Jalon J8 |
| Des chiffres réels | Les dix chiffres du business case § 6 passés de [estimé] à [relevé] | Tableau de bord |

**Ce que le projet ne cherche pas** : rentabiliser la mise en douze mois, financer les machines du palier 2 par le cash du palier 1, ni prouver la conservation de l'eau extraite ou l'acceptation du prix d'une bouteille en CHR.

---

## 3. Parties prenantes principales, sponsor, chef de projet

### 3.1 Rôles

| Rôle | Qui | Responsabilité |
|---|---|---|
| **Sponsor** | **À désigner.** Profil recherché : associé terrain ou investisseur local proche de la filière coco ou du tourisme, apportant 5–15 M XPF en deux tranches ou un équivalent en nature (accès cocoteraie, local froid, réseau d'opérateurs). **Jusqu'à sa désignation, le fondateur tient le rôle par intérim** et le dit explicitement dans chaque décision de jalon. | Finance au-delà de l'apport, arbitre les changements hors autorité du chef de projet, valide les jalons J1, J7 et J8, tient les seuils de décision annoncés : tranche 1 sur pilote payant signé et marge par coco positive mesurée ; tranche 2 sur deuxième opérateur qui réassortit et coût par coco en baisse |
| **Chef de projet** | **Le fondateur** (profil tech / produit, temps plein possible) | Porte le périmètre, le calendrier, le budget et la qualité ; exécute le terrain ; décide dans les limites de § 3.2 ; rend compte mensuellement |
| Director-General (équipe IA) | Session principale r-stack, fonction Product Owner | Tient `VISION.md` et le backlog, prépare les décisions, convoque le challenger, garantit la cohérence avec la finalité ; ne décide pas à la place du fondateur |
| Challenger (équipe IA) | Agent `challenger` | Contradicteur de chaque décision structurante et membre du comité de changement (plan § 7) |
| Directeurs IA | `operations-director`, `brand-director`, `business-director` et leurs spécialistes | Instruisent et documentent ; le fondateur reste responsable de chaque livrable |
| Cocoteraie partenaire | À sélectionner (≥ 2 sources, 1 principale) | Sélectionne et récolte au stade nīā selon la fiche, livre au jour fixe, accepte la règle de refus |
| Découpeur | À recruter, à la tâche ou à temps partiel | Contrôle à réception, découpe, mise au froid, selon protocole |
| Opérateur pilote et son guide | À signer parmi les types prioritaires (sortie bateau courte, baleines, lagon journée) | Achète, stocke au froid, sert selon la fiche, rend ses retours chaque semaine, signe le PV de recette |
| Services du Pays | CHSP, DGAE, Direction de la biosécurité, CCISM, CPS | Déclaration, hygiène, étiquetage, fret agricole, création d'entreprise |

Registre complet avec intérêts, influence et stratégie d'engagement : annexe A3 § 5.

### 3.2 Niveau d'autorité du chef de projet

Le chef de projet décide seul, dans le cadre de cette charte, de :

- toute dépense unitaire ≤ 150 000 XPF et tout cumul mensuel ≤ 400 000 XPF, dans la référence budgétaire ;
- l'organisation du travail, le choix des fournisseurs non critiques, le calendrier interne entre deux jalons ;
- le recrutement du découpeur à la tâche ;
- la priorisation du backlog et le contenu des sprints.

Nécessitent le sponsor (ou le fondateur par intérim, **avec avis écrit du challenger**) :

- toute dépense unitaire > 150 000 XPF, et notamment l'atelier, le froid, toute machine ;
- tout dépassement de la référence budgétaire de plus de 10 % ou tout glissement de J6 au-delà du 30 avril 2027 ;
- tout changement de périmètre : second produit, client hors opérateurs d'excursion (hôtels, pensions, croisière), extension à une île autre que Tahiti et Moorea, revente au touriste ;
- le choix entre les options A, B et C et tout passage de l'une à l'autre ;
- tout prix de vente inférieur au plancher de 400 XPF ;
- les décisions de go / no-go des jalons J1, J7 et J8.

Le chef de projet ne peut pas, même avec l'accord du sponsor, s'écarter des non-objectifs de `VISION.md` (export, grande distribution, B2C en ligne, cocoteraie en propre) sans repasser par le gate ① de la vision.

---

## 4. Périmètre initial

### 4.1 Le produit

**Une coco nīā, découpée en diamond cut, froide, marquée NĪĀ, livrée en caisse, prête à être ouverte et servie par le guide.** Stade nīā vérifié (amande fine et molle, eau sucrée), coque interne intacte jusqu'au service, température à cœur ≤ 7 °C à la remise, DLC écrite et fixée par le test de conservation, marquage sobre, caisse consignée de 12 avec étiquette de lot, kit de service (perforateur, pailles, fiche FR/EN) avec les premières livraisons. Spécification et critères d'acceptation : annexe A2 § 1.1.

### 4.2 Le travail du projet

Ce qu'il faut faire pour que ce produit existe, soit légal, soit vendu et soit livré régulièrement, en huit branches : gouvernance et financement ; filière amont ; process de découpe et froid ; réglementaire, hygiène et assurance ; logistique et livraison ; pilote commercial ; marque et présentation ; clôture et leçons. Trente work packages, détaillés dans le plan (§ 1) et l'annexe A2 § 2–3.

### 4.3 Limites

| Dans le périmètre | Hors périmètre |
|---|---|
| Tahiti d'abord, Moorea à partir de juin 2027 si la chaîne du froid et le fret tiennent | Toute autre île ; fret aérien |
| Opérateurs d'excursion (coco incluse dans l'excursion) ; hôtels, pensions et traiteurs seulement en entretiens d'exploration | Vente directe aux touristes, encaissement à bord, revente par l'opérateur |
| Découpe manuelle, atelier déclaré, froid positif, caisses consignées | Machine de découpe ou d'extraction pendant le pilote (une note buy or make est produite pour J8) |
| Cocos achetées à une cocoteraie partenaire qui récolte | Récolte par NĪĀ, cocoteraie en propre |
| Un seul produit : le diamond cut nīā ; origine toujours dite (cocoteraie, île) | Eau extraite, bouteille, pulpe, coco entière non découpée, second produit, gamme Motu / Mouʻa (instruite en A6–A7 pour le palier 2) |
| Marquage, une phrase du guide FR/EN, fiche d'origine | Charte graphique complète, site, réseaux sociaux, code |
| Découpeur à la tâche ou temps partiel, déclaré | Recrutement à temps plein |
| Glacière de prêt chez l'opérateur | Réfrigérateur fourni chez l'opérateur |

---

## 5. Risques majeurs et hypothèses

Les cinq risques qui décident, avec la vérification engagée avant le go financement (registre complet : annexe A4) :

| Risque | Score | Vérification avant le 4 janvier 2027 |
|---|---|---|
| La coco découpée tient moins d'une semaine au froid | 20 | Lot test de 30–50 cocos sur 14 jours, première semaine de novembre |
| Les opérateurs gardent leur guide-coupeur et leur coco du motu | 20 | Dix entretiens, question « qui coupe aujourd'hui et pourquoi ? », cibles prioritaires de A5 |
| Coût complet supérieur au prix accepté | 16 | Coût complet relevé, devis écrit à trois niveaux de prix |
| Cocoteraie hors stade ou irrégulière | 16 | Essai d'achat de 50 cocos triées chez deux cocoteraies, fiche nīā, taux de rejet |
| Fret inter-îles payant ou froid rompu vers Moorea | 16 | Lecture de l'arrêté 1586 CM sur Lexpol, question écrite à la DGAE, fret compté plein en attendant |

Hypothèses structurantes, toutes non relevées à ce jour : conservation ≥ 10 jours ; une cocoteraie de Tahiti livre ≥ 100 nīā par semaine à ≤ 200 XPF ; déclaration CHSP en ≤ 8 semaines sans local hors budget ; un opérateur paie 500–700 XPF ; ≤ 3 min et ≤ 10 % de perte par coco au geste manuel ; conditions du fret agricole. Chacune a un work package et une semaine de vérification (plan § 6).

---

## 6. Planification macro

| Phase | Période | Contenu | Jalon sponsor |
|---|---|---|---|
| **0. Vérification** | 2 novembre 2026 → 3 janvier 2027 | Charte signée ; lot test de conservation ; fiche nīā ; cartographie cocoteraies et opérateurs ; rendez-vous CHSP, DGAE, biosécurité ; création de l'entité et RC ; modèle économique v0 ; dossier sponsor | **J1 Go financement — 4 janvier 2027** (limite 18 janvier) |
| **1. Mise en place** | Janvier → mars 2027 | Contrat cocoteraie ; second lot de conservation en conditions réelles ; atelier et froid ; plan d'hygiène ; étiquetage et DLC ; découpeur recruté et formé ; chaîne du froid testée ; présentation façon NĪĀ ; offre et accord pilote ; dossier CHSP déposé | **J2 Cocoteraie signée — 1er février** ; **J3 Protocole et DLC validés — 15 février** ; **J5 Opérateur pilote signé — 8 mars** ; **J4 Conformité obtenue — 22 mars** |
| **2. Pilote** | Avril → août 2027 | Productions à blanc puis lots payants ; livraisons hebdomadaires ; indicateurs ; revues sponsor mensuelles ; extension à Moorea et à un second opérateur à partir de juin si Tahiti tient | **J6 Première livraison payante — semaine du 5 avril 2027 (limite 30 avril)** |
| **3. Clôture et décision** | Septembre → octobre 2027 | PV de recette après ≥ 20 semaines ; bilan en chiffres relevés ; note buy or make ; enseignements pour l'eau extraite ; décision | **J7 Fin du pilote — 6 septembre** ; **J8 Décision palier 2 — 4 octobre 2027** |

Chemin critique : conservation → atelier et froid → déclaration CHSP → production à blanc → première livraison. Il passe par la conformité, pas par la vente. Le financement du 4 janvier en est la porte d'entrée. Contraintes externes : saison des pluies de novembre à avril, fermeture des administrations fin décembre, Pâques fin mars, haute saison touristique de juin à octobre.

---

## 7. Budget et financement

| | Montant | Source |
|---|---|---|
| Référence budgétaire du palier 1 (option A, douze mois) | **3,0 M XPF**, dont ≈ 1,0 M d'investissement, ≈ 1,5 M de pertes d'exploitation et de fonds de roulement jusqu'au point bas, ≈ 0,5 M de réserve | Plan § 3 ; annexes A1 § 3–4 et A2 § 3 bis |
| Phase de vérification (avant J1) | ≤ 150 k XPF | Business case § 7.2 |
| Financement | Apport du fondateur (2–5 M) ; complément possible par préfinancement d'un opérateur ou microcrédit ; sponsor pour l'accélération, la machine et le palier 2 | A1 § 7 |

Aucune dépense d'atelier, de froid ou de machine avant le go financement du 4 janvier 2027.

---

## 8. Approbation

Par leur signature, le sponsor et le chef de projet acceptent la mission telle que décrite : but, résultats recherchés, périmètre et limites, autorité du chef de projet, jalons et référence budgétaire. Toute modification passe par le comité de changement défini au plan § 7.

| Rôle | Nom | Date | Signature |
|---|---|---|---|
| Chef de projet | Le fondateur | | |
| Sponsor | À désigner ; le fondateur par intérim | | |

Relu par le Director-General et le challenger le 2026-10-24.
