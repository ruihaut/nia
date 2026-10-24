# Annexe A5 — Compatibilité des types d'excursion et customer journeys (palier 1)

> Statut : document de travail, version 0 (2026-10-24). Rédigé par `market-scout` sans accès au web : **chaque fait ou chiffre porte `[estimé : raisonnement]` ou `[supposé]`** et doit être remplacé par un relevé terrain avant d'être tenu pour acquis. Le seul chiffre sourcé est celui des excursionnistes de croisière (ISPF, voir §1).
> Articulation : l'annexe A3 (`business-director`) fait la segmentation courte et renvoie ici pour le détail ; l'annexe A1 (`financial-modeler`) fixe le prix de vente par coco — ici on raisonne en fourchette 400–800 XPF `[supposé]`, **voir A1 pour le prix retenu**. Les items 3 et 8 du backlog (`scrum/backlog.md`) sont les suites opérationnelles de ce document.
> Modèle de vente rappelé (`VISION.md`) : le coco nīā diamond cut, réfrigérée, est **incluse dans l'excursion** ; l'opérateur l'achète à NĪĀ et la sert à ses passagers ; pas de revente au touriste.

---

## 0. En une page

**Question posée.** Quels types d'excursion de Tahiti et Moorea sont compatibles avec un coco nīā diamond cut, livrée froide, servie à bord ou sur place ? Et à quoi ressemble, étape par étape, la vie de ce coco chez l'opérateur et dans les mains du passager ?

**Intuitions de départ du fondateur, testées.**
- *Randonnée = incompatible a priori* : **confirmé** pour le service pendant la marche (1,2–1,5 kg par passager à porter, pas de froid, coque à redescendre). Une variante « coco à l'arrivée », servie au véhicule du guide au retour, existe mais reste une cible tertiaire (petits groupes, peu de sorties).
- *Sortie bateau = pleinement compatible a priori* : **confirmé et affiné**. Ce n'est pas « le bateau » qui rend compatible, c'est quatre conditions que le bateau réunit presque toujours.

**Règle générale qui en sort (à retenir).** Un type d'excursion est compatible si, et seulement si :
1. **un véhicule porte la glacière jusqu'au point de service** (le passager ne porte jamais le coco plus de quelques mètres) ;
2. il existe **un temps mort d'au moins 15 minutes, passagers assis ou à l'arrêt, mains libres** (retour, mouillage, belvédère, attente des baleines) ;
3. **la coque repart dans un bac** avec le véhicule (rien ne reste sur le motu, sur le site ou sur le sentier) ;
4. le guide **n'a pas déjà un rituel coco à la machette** qui fait partie de son spectacle — ou accepte que NĪĀ le complète plutôt que le remplace.

Bateau : 1–2–3 oui, 4 variable. Safari 4x4 : 1–2–3 oui, 4 souvent non. Tour d'île en bus : 1 oui, 2 et 3 difficiles (sites publics, pas d'endroit pour servir ni pour jeter). Randonnée : rien. Kayak, quad : 1 non.

**Classement (matrice pondérée, §2).** Cibles prioritaires : observation des baleines (saison), sortie bateau courte snorkeling, sortie lagon journée avec motu, sunset cruise d'hôtel (pont vers le palier 2). Cibles secondaires : pêche sportive, safari 4x4, plongée, jet-ski guidé, canal croisière, tour d'île en van/bus, randonnée « à l'arrivée ». Incompatibles : quad/VTT, kayak/paddle/pirogue en location, randonnée pendant la marche.

**Trois journeys détaillés (§3).** J1 sortie lagon journée avec motu ; J2 sortie bateau courte sans débarquement (snorkeling, baleines en saison) ; J3 safari 4x4 (meilleure cible terrestre, écrite pour tester la généralisation de la règle hors du bateau).

**Point de friction principal de chaque journey.** J1 : le guide ouvre déjà des cocos à la machette sur le motu, c'est son numéro — NĪĀ doit s'y insérer, pas le remplacer. J2 : le service tient en 15–20 minutes sur le trajet retour, bateau en mouvement — il faut un geste d'ouverture sans outil dangereux et une coque qui va directement au seau. J3 : chaleur, poussière, glacière ouverte dix fois — le froid est le maillon faible, et le prix pèse plus lourd dans un billet à 5 000–7 000 XPF.

**Potentiel (§5, fourchettes).** 1 opérateur prioritaire : 300–650 cocos/mois en haute saison, soit 0,13–0,52 M XPF/mois ; 3 opérateurs : 0,5–1,7 M XPF/mois ; 10 opérateurs : 1,7–5,8 M XPF/mois `[estimé, prix 400–800 XPF, voir A1]`. En basse saison, diviser par 1,5 à 2.

---

## 1. Typologie des excursions à Tahiti et Moorea

Conventions : « pax » = passagers par sortie ; prix par adulte en XPF ; « HS/BS » = haute/basse saison. Haute saison touristique : juillet–août et octobre–novembre, pic secondaire à Noël ; basse : février–mars (pluies) et, dans une moindre mesure, mai–juin `[estimé : saisonnalité générale du tourisme polynésien, à caler sur les séries ISPF]`. La saison des baleines à bosse court de juillet à novembre `[estimé : connaissance générale ; recouvre la haute saison]`.

Le seul chiffre sourcé de cette annexe : **70 062 excursionnistes de croisière en 2025** (ISPF, *Points conjoncture Tourisme 2025-12*, https://www.ispf.pf/content//uploads/1517_PC_Tourisme_2025_12_9e5f74a421.pdf). Au sens ISPF, l'excursionniste de croisière est le passager d'un paquebot en escale qui ne dort pas à terre ; il se distingue du croisiériste embarquant en Polynésie (type *Paul Gauguin*, *Aranui*, *Windstar*) qui est compté comme touriste `[estimé : définition ISPF de mémoire, à vérifier dans la note]`.

| # | Type | Durée | Pax / sortie | Sorties / jour · / semaine (HS) | Prix billet `[estimé]` | Profil passagers | Moment naturel d'un rafraîchissement | Ce qui est servi aujourd'hui `[estimé/supposé]` |
|---|---|---|---|---|---|---|---|---|
| 1 | **Sortie lagon journée avec arrêt motu et pique-nique** (Moorea surtout ; Tahiti Iti, Tetiaroa en version premium) | 6–7 h (≈ 9h–15h30) | 12–30 (bateau à fond plat, poti marara, catamaran) | 1 · 5–6 | 9 000–13 000 repas inclus `[estimé : positionnement « journée tout compris »]` | Couples en voyage de noces, familles, passagers de paquebots les jours d'escale ; 60–80 % non francophones `[supposé]` | Arrivée sur le motu après le snorkeling raies/requins (bouche salée, 11h) ; ou avant le repas | Eau, jus, parfois ponch ou bière au repas ; poisson cru au lait de coco préparé devant les passagers ; **démonstration d'ouverture de coco à la machette par le guide**, fruits locaux `[estimé : format répandu des tours motu]` |
| 2 | **Sortie bateau courte snorkeling** (raies, requins pointe noire, jardin de corail, dauphins hors saison baleines) | 2,5–3,5 h | 8–20 | 2 (matin/après-midi) · 10–12 | 6 000–9 000 | Même profil que 1, plus de clients d'hôtel « demi-journée » | Trajet retour après le dernier arrêt (15–25 min, tout le monde assis, soif) | Bouteilles d'eau, parfois fruits coupés ; pas de repas `[estimé]` |
| 3 | **Observation des baleines** (juillet–novembre, mise à l'eau encadrée) | 3–4 h | 8–12 (quotas et pratiques encadrées) `[estimé : réglementation de l'approche des cétacés, petits groupes]` | 2–3 · 12–15 en saison | 11 000–16 000 | Clientèle motivée, pouvoir d'achat plus élevé, beaucoup de répétiteurs `[supposé]` | Longues phases d'attente et de recherche moteur réduit ; après la mise à l'eau (froid, fatigue) | Eau, biscuits, fruits ; thermos de thé/café chez certains `[supposé]` |
| 4 | **Jet-ski guidé** (tour de l'île ou demi-tour, arrêt banc de sable / motu) | 1,5–3 h | 2–8 jets, 2–14 pax | 2–3 · 12–15 | 18 000–30 000 par jet (1–2 pax) | Jeunes couples, groupes d'amis, clientèle à budget | Arrêt baignade sur banc de sable ou motu (20–30 min) | Rien, ou eau dans le coffre du guide ; certains guides font une démonstration de coco et de fruits à l'arrêt `[supposé]` |
| 5 | **Plongée bouteille** (2 plongées, bateau semi-rigide ou coque dure) | 3–4 h | 6–12 plongeurs + encadrants | 2–3 · 12–18 | 8 000–11 000 la plongée, forfaits dégressifs | Plongeurs certifiés et baptêmes ; clientèle sensible au prix du forfait | Intervalle de surface entre les deux plongées (45–60 min) ; retour | Eau, biscuits sucrés, parfois fruits ; thé chaud `[estimé]` |
| 6 | **Kayak / paddle / pirogue** (location libre ; quelques sorties guidées au lever du soleil ou vers un motu) | 1–3 h | 1–8 | Location continue · faible encadrement | 2 000–5 000 la location ; 6 000–9 000 guidé | Clients d'hôtel ou de pension, autonomie | Retour à la plage de départ | Rien (location) ; parfois fruits au motu (guidé) |
| 7 | **Pêche sportive** (charter hauturier) | 4–8 h | 2–6 | 1 · 2–5 | 60 000–150 000 le bateau | Clientèle masculine, pouvoir d'achat élevé, souvent répétiteurs | Dès la sortie de passe puis toute la journée (chaleur, bière) | Glacière pleine : bières, sodas, sandwichs ; très bien équipé en glace (poisson) |
| 8 | **Safari 4x4 intérieur de l'île** (Papenoo, Opunohu, Belvédère, champs d'ananas, cascades) | 3,5–4,5 h ; journée 7 h | 8 par camion (bancs latéraux, ouvert), 1–4 camions | 2 · 10–12 par camion | 5 000–7 500 demi-journée ; 9 000–12 000 journée repas inclus | Mixte familles, croisière, seniors ; francophones plus nombreux qu'en lagon `[supposé]` | Arrêt belvédère ou cascade (15–25 min) ; à Moorea arrêt dégustation d'ananas et confitures | Eau ; **dégustation de fruits, parfois coco ouvert à la machette** par le guide à un arrêt ; passage à un stand de bord de route `[estimé : pratique fréquente des safaris]` |
| 9 | **Tour d'île en van / bus** (Pointe Vénus, trou du souffleur, cascades, jardins, grotte) | 4–8 h | 8 (van) à 45 (bus) | 1 · 3–6 ; pics les jours de paquebot | 5 000–9 000 ; vendu 10 000–14 000 équivalent à bord des paquebots avec commission `[supposé]` | Croisière majoritaire, seniors, groupes | Arrêts sur sites publics (10–15 min chacun), pause déjeuner | Eau en bouteille ; déjeuner au restaurant ou snack ; rien sur les sites |
| 10 | **Randonnée guidée** (vallées, cascades, crêtes, Fautaua, Aorai, Trois Cocotiers) | 3–8 h de marche | 4–12 | 1 · 3–6 | 6 000–12 000 | Marcheurs, 25–50 ans, autonomes, souvent résidents aussi | Pause au sommet / à la cascade ; retour au véhicule | Chacun porte son eau ; le guide porte fruits secs, parfois fruits ; rien de froid |
| 11 | **Quad / VTT** (pistes intérieures, plantations, belvédère) | 2–3 h | 2–8 machines, 2–12 pax | 2–3 · 12–15 | 15 000–25 000 le quad (1–2 pax) ; VTT 5 000–8 000 | Jeunes couples, groupes ; sensations | Arrêt belvédère (15 min) | Eau ; parfois dégustation de fruits au point de vue `[supposé]` |
| 12 | **Excursions croisière** (escales à Papeete, Moorea, Bora Bora, Raiatea, Huahine ; vendues à bord ou en direct au quai) — **c'est un canal qui irrigue les types 1, 2, 8, 9, plus qu'un type en soi** | Calée sur l'escale (4–8 h) | Par vagues de 20 à 300 pax sur un jour | 0 la plupart des jours, 5–20 sorties un jour d'escale | Vendu 8 000–20 000 à bord ; l'opérateur touche 50–70 % `[supposé]` | Seniors internationaux, anglophones, peu de temps, forte envie de « l'expérience locale » | Au premier arrêt, après la marche depuis le quai | Ce que sert l'opérateur sous-traitant (voir types 1, 8, 9) |
| 13 | **Activités d'hôtel / pension** : sunset cruise en catamaran, cocktail et animation plage (démonstration coco, tressage), pique-nique motu privé | 1,5–2,5 h (sunset) ; 1–2 h (animation) | 15–40 (catamaran) ; 20–60 (animation) | 1 le soir · 3–6 ; animation quotidienne | 7 000–12 000 (sunset) ; animation offerte | Clients de l'hôtel, voyage de noces, pouvoir d'achat élevé | Apéritif au coucher du soleil ; fin d'animation | Champagne/cocktails et amuse-bouches (sunset) ; **l'hôtel ouvre déjà des cocos lors de son animation** avec son propre personnel `[estimé : animation classique des resorts]` |

Ce que le tableau dit déjà : le coco **existe déjà** dans l'offre des types 1, 4, 8 et 13 — mais **chaude, ouverte à la machette, à un stade non sélectionné**. C'est à la fois la preuve que le moment existe et le principal concurrent de NĪĀ (voir critère « internalisation », §2).

---

## 2. Matrice de compatibilité

### 2.1 Critères, échelle et pondération

Note 1 (très défavorable) à 5 (très favorable). La pondération reflète ce qui conditionne une **livraison régulière** sous 6 mois (volume, moment) plus que l'image, qui compte mais ne fait pas vivre le palier 1.

| Critère | Ce qu'on note | Poids |
|---|---|---|
| **T — Transport jusqu'au point de service** | Un coco diamond cut pèse ≈ 0,9–1,3 kg une fois une partie de la bourre retirée `[estimé : coco jeune entière 1,2–1,5 kg, le diamond cut en enlève 20–30 %]` ; 20 cocos + glace = 30–35 kg, soit une glacière de 80–100 L. Qui porte, jusqu'où, sur quoi ? | 10 % |
| **F — Maintien au froid pendant l'excursion** | Cible de service 4–8 °C ; durée hors chambre froide ; glacière ouverte souvent ou non ; soleil, chaleur moteur, poussière | 10 % |
| **M — Moment et durée disponibles pour servir** | Existe-t-il un temps mort ≥ 15 min, passagers assis ou arrêtés, qui coïncide avec la soif ? | 15 % |
| **G — Geste d'ouverture et de service** | Qui ouvre (guide, matelot, passager), avec quoi (pointe de couteau, ouvre-coco, pas de machette), stabilité du support, sécurité | 10 % |
| **C — Gestion de la coque** | 0,8–1,2 kg de déchet humide par passager ; existe-t-il un bac qui repart avec le véhicule ? | 10 % |
| **V — Volume par sortie et régularité des commandes** | Cocos par sortie × sorties par semaine × régularité sur l'année | 15 % |
| **P — Prix du billet et place d'un plus de 400–800 XPF** `[supposé]` | Part du coût NĪĀ dans le billet ; capacité de l'opérateur à l'absorber ou à le répercuter | 10 % |
| **I — Valeur d'image** | Photo naturelle (coco en main, lagon ou montagne derrière), moment partagé, place pour l'histoire du nīā | 10 % |
| **R — Risque d'internalisation (noté à l'envers : 5 = faible risque)** | L'opérateur le fait-il déjà lui-même à la machette ? A-t-il le personnel, le temps et l'envie de le faire ? | 10 % |

### 2.2 Scores

| Type | T | F | M | G | C | V | P | I | R | **Score pondéré** | Classe |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 3 Observation des baleines (saison) | 5 | 5 | 5 | 4 | 4 | 3 | 5 | 5 | 4 | **4,40** | Prioritaire (saisonnière) |
| 2 Sortie bateau courte snorkeling | 5 | 5 | 4 | 4 | 4 | 5 | 4 | 4 | 4 | **4,35** | Prioritaire |
| 1 Sortie lagon journée avec motu | 5 | 4 | 5 | 4 | 3 | 5 | 5 | 5 | 2 | **4,30** | Prioritaire |
| 13a Sunset cruise d'hôtel / catamaran | 5 | 5 | 5 | 4 | 4 | 3 | 4 | 5 | 3 | **4,20** | Prioritaire conditionnelle (pont palier 2) |
| 7 Pêche sportive | 5 | 5 | 4 | 4 | 4 | 1 | 5 | 3 | 4 | **3,75** | Secondaire |
| 8 Safari 4x4 | 4 | 3 | 4 | 4 | 4 | 4 | 3 | 4 | 2 | **3,60** | Secondaire haute (meilleure cible terrestre) |
| 5 Plongée bouteille | 5 | 4 | 3 | 3 | 4 | 3 | 3 | 2 | 5 | **3,50** | Secondaire |
| 4 Jet-ski guidé | 3 | 3 | 4 | 3 | 3 | 2 | 5 | 5 | 3 | **3,40** | Secondaire |
| 12 Canal croisière (via types 1, 2, 8, 9) | 4 | 3 | 3 | 3 | 3 | 3 | 3 | 4 | 4 | **3,30** | Secondaire (phase 2 du palier 1) |
| 9 Tour d'île van / bus | 4 | 3 | 3 | 3 | 3 | 4 | 2 | 3 | 4 | **3,25** | Secondaire basse |
| 10b Randonnée, variante « coco à l'arrivée » | 3 | 3 | 4 | 3 | 3 | 2 | 3 | 3 | 5 | **3,20** | Secondaire basse / tertiaire |
| 13b Animation plage d'hôtel | 5 | 5 | 4 | 3 | 4 | 3 | 2 | 4 | 1 | **3,45** | Hors palier 1 (porte d'entrée palier 2) |
| 11 Quad / VTT | 2 | 2 | 3 | 3 | 2 | 2 | 4 | 4 | 4 | **2,85** | Incompatible |
| 6 Kayak / paddle / pirogue | 2 | 2 | 2 | 2 | 2 | 2 | 2 | 4 | 4 | **2,40** | Incompatible |
| 10a Randonnée, service pendant la marche | 1 | 1 | 2 | 2 | 1 | 2 | 3 | 3 | 5 | **2,20** | Incompatible |

Seuils : prioritaire ≥ 4,0 ; secondaire 3,0–3,99 ; incompatible < 3,0. Les scores sont des jugements `[estimé]` ; une visite terrain par type suffit à en bouger un de ±0,3. Ce qui ne bougera pas : l'écart entre le bateau (≥ 4,2) et la randonnée pendant (2,2).

### 2.3 Justifications des cases notables (une ligne par case)

- **1·R = 2** : sur le motu, l'ouverture de coco à la machette est souvent le numéro du guide ; NĪĀ arrive chez quelqu'un qui « fait déjà des cocos » — c'est l'objection principale et le test clé du pilote.
- **1·C = 3** : le motu n'a pas de poubelle ; les coques doivent revenir au bateau dans un bac, ce que les opérateurs sérieux font déjà pour leurs déchets de repas `[supposé]`.
- **2·V = 5** : deux sorties par jour, six jours sur sept, toute l'année : c'est le flux le plus régulier de la typologie, donc le meilleur pour apprendre à livrer.
- **2·M = 4** et non 5 : le service se fait sur le trajet retour, bateau en route ; il faut qu'il tienne en 15–20 min avec un seul matelot.
- **3·V = 3** : 8–12 pax par sortie et cinq mois par an ; mais les mêmes bateaux font du snorkeling hors saison, d'où un couplage naturel 2+3 chez le même opérateur.
- **3·P = 5** : 500 XPF dans un billet à 12 000–16 000, c'est 3–4 % ; invisible pour l'opérateur comme pour le passager.
- **13a·R = 3 et 13b·R = 1** : l'hôtel a du personnel de cuisine et d'animation ; il peut tout internaliser. La sunset cruise reste jouable parce qu'elle est souvent sous-traitée à un catamaran extérieur `[supposé]` ; l'animation plage ne l'est pas.
- **7·V = 1** : 4–6 pax, 2–5 sorties par semaine, dépendantes de la météo : trop peu pour structurer une tournée ; à servir en appoint quand le camion passe.
- **8·F = 3** : 4 h de piste, glacière à l'arrière d'un camion ouvert, ouverte à chaque arrêt pour l'eau ; sans glacière dédiée et pains de glace, le coco arrive tiède au belvédère.
- **8·P = 3** : 500 XPF dans un billet à 5 000–7 500, c'est 7–10 % ; l'opérateur demandera à répercuter, donc à justifier auprès des agences qui lui achètent ses places.
- **8·R = 2** : la dégustation de fruits et le coco ouvert au couteau à un arrêt font déjà partie de beaucoup de safaris `[estimé]`.
- **5·I = 2** : le plongeur photographie sous l'eau, pas sa coco ; l'intervalle de surface est un moment de récupération plus que de partage.
- **9·M = 3 et 9·C = 3** : sur un parking de site public, pas d'endroit pour servir 40 cocos ni pour jeter 40 coques ; le bus n'a pas de bac ; seul l'arrêt déjeuner convient.
- **9·P = 2** : les billets croisière passent par le navire et l'agence réceptive ; la marge de l'opérateur est déjà comprimée.
- **12** : 70 062 excursionnistes de croisière en 2025 (ISPF) donnent environ 190 par jour en moyenne lissée, mais la réalité est 0 la plupart des jours et 500–2 000 passagers débarqués un jour d'escale `[estimé : taille des paquebots en escale]`. Pour NĪĀ en année 1, ce sont des pics de 100–300 cocos sur un jour, impossibles à absorber tant que la découpe est manuelle — à traiter en phase 2 du palier 1, quand la capacité et la conservation sont prouvées.
- **4·T = 3** : le coffre d'un jet-ski prend une glacière souple de 6–8 cocos au mieux ; au-delà, il faut un bateau suiveur.
- **11·T = 2** : pas de place pour une glacière rigide sur un quad ; poussière et secousses.
- **6** : la location libre n'a pas de guide, donc pas de moment de service ni de personne pour ouvrir.

### 2.4 Pourquoi la randonnée est incompatible, et quelle variante existe

**Pendant la marche (10a).** Les quatre conditions de la règle générale tombent : (1) pas de véhicule — un groupe de 8 représenterait 8–10 kg de cocos plus de la glace dans le sac du guide, qui porte déjà la trousse de secours, la corde et l'eau de réserve ; (2) la pause au sommet existe, mais (3) il faudrait redescendre 8 kg de coques humides, et (4) le coco n'a aucune place dans le récit d'un guide de montagne. Le froid est perdu après 2 h de marche au soleil. **Incompatible sans discussion.**

**Au départ.** Personne n'a soif à 7h au parking, et le passager garderait la coque ou la laisserait sur place. Sans intérêt.

**À l'arrivée (10b).** Le guide laisse une glacière dans son véhicule au point de départ/arrivée ; au retour, après 4–6 h d'effort, le coco froid est un vrai moment (soif, récompense, photo du groupe au pied de la vallée). Conditions : glacière rigide avec pains de glace dans un véhicule à l'ombre pendant 5–8 h `[estimé : une glacière de qualité pré-refroidie tient < 10 °C sur cette durée]`, coques laissées dans le véhicule. Volume faible (4–12 par sortie, 3–6 sorties par semaine) : **cible tertiaire**, à servir en appoint d'une tournée existante, jamais en premier client.

**Ce que la randonnée enseigne pour généraliser.** Le critère n'est pas « terre ou mer » mais « la glacière voyage-t-elle avec le groupe jusqu'au moment de soif, et la coque repart-elle avec elle ? ». C'est ce qui sépare le safari 4x4 (oui, camion) du tour d'île en bus (le bus est là, mais le lieu de service n'existe pas) et de la randonnée (non).

---

## 3. Customer journeys des cibles prioritaires

Trois journeys : **J1** sortie lagon journée avec motu (type 1) ; **J2** sortie bateau courte sans débarquement (type 2, et type 3 en saison : mêmes bateaux, mêmes équipages) ; **J3** safari 4x4 (type 8, secondaire haute, inclus pour tester la règle hors du bateau). La sunset cruise d'hôtel (13a) suit J2 à la lettre avec un apéritif en plus ; elle n'a pas de journey séparé.

Chaque journey a deux fils : **(a) l'opérateur et son équipage**, **(b) le passager**. Colonnes : ce qui se passe / ce que fait NĪĀ / ce qui peut rater / ce qu'on mesure. Les unités de mesure sont celles qu'un fondateur seul peut relever en montant à bord une fois par semaine pendant le pilote.

### Présentation « façon NĪĀ » minimale, commune aux trois journeys

À détailler par `brand-director` et `copywriter` (item 7 du backlog). Hypothèse de travail ici, volontairement sobre : coco diamond cut froide, facettes nettes, **sans paille plastique** ; un marquage discret sur la facette (estampille NĪĀ ou bracelet papier) ; un geste d'ouverture propre (pointe de couteau ou ouvre-coco, jamais la machette) ; **trois phrases dites par le guide** (FR/EN) : ce qu'est le stade nīā, pourquoi elle est froide, d'où elle vient. Pas de mise en scène supplémentaire : le lagon ou la montagne fait le décor.

### 3.1 J1 — Sortie lagon journée avec arrêt motu et pique-nique

Contexte type `[estimé]` : départ 9h d'une plage ou d'un quai (Moorea : Haapiti, Papetoai, Vaiare, Temae ; Tahiti : Teahupoo, Punaauia), 15–25 pax, un capitaine et un ou deux guides, snorkeling raies/requins 10h–11h, arrivée motu 11h30, repas 12h30, retour 15h30. Glacières à bord : 2–3 de 60–100 L pour boissons et poisson.

**(a) Fil opérateur et équipage**

| Étape | Ce qui se passe | Ce que fait NĪĀ | Ce qui peut rater | Ce qu'on mesure |
|---|---|---|---|---|
| A1 Commande | Le jeudi, l'opérateur connaît ses réservations de la semaine suivante à ±20 % ; il commande par message (WhatsApp/SMS) un nombre de cocos par jour de sortie | Reçoit, confirme sous 2 h, propose quantité = pax réservés + 10 % ; fixe le créneau de livraison | Commande oubliée ; réservations de dernière minute (croisière) ; NĪĀ ne peut pas suivre | Délai commande→confirmation ; écart commandé / servi |
| A2 Réception | Livraison en caisse consignée NĪĀ, cocos pré-refroidies, lundi 6h30–7h30 à la base (fare, maison du capitaine, quai) ; à Moorea via le ferry du matin `[supposé : Papeete–Vaiare 30–45 min, premier départ vers 6h]` | Livre, prend la température à cœur devant l'opérateur, fait signer un bon simple (quantité, température, heure), reprend les caisses et les coques de la semaine précédente | Pas de personne pour réceptionner ; rupture du froid sur le ferry ; retard | Température à réception ; heure de livraison ; casse/fuite |
| A3 Stockage à terre | Si frigo à la base : cocos au frigo, sorties le matin même. Sinon : glacière dédiée avec pains de glace, renouvelés chaque soir | Fournit, en prêt pendant le pilote, une glacière marquée NĪĀ et des pains de glace ; indique la DLC du lot (voir item 4 du backlog) | Pas de frigo → autonomie 2 jours max → livraison bi-hebdo ; mélange avec les poissons et bières ; porte de frigo ouverte | Jours de stock avant service ; température matin ; pertes (écoulement, odeur) |
| A4 Embarquement | 7h30–8h30 : chargement des glacières ; les cocos du jour dans leur glacière dédiée, avec glace | Rien : c'est le geste de l'opérateur ; NĪĀ a conçu la caisse pour qu'elle rentre dans une glacière de 80 L | Glacière oubliée ; cocos mises dans la glacière à boissons ouverte toutes les 10 min | Nombre de cocos embarquées vs pax du jour |
| A5 Pendant — moment de service | **Option A (recommandée)** : à l'arrivée sur le motu, avant le repas, le guide sort les cocos ; **Option B** : au mouillage après le snorkeling, à bord | Fiche plastifiée du geste et des trois phrases ; un ouvre-coco ou couteau court dans la glacière ; marquage visible | Le guide préfère son numéro à la machette avec des cocos chaudes achetées le matin ; passe les cocos sans un mot ; les ouvre toutes à l'avance et elles tiédissent | Heure et lieu réels du service ; qui ouvre ; durée totale du service pour 20 pax (objectif < 10 min) ; les trois phrases dites ou non |
| A6 Pendant — récit | Le guide dit ce qu'est le nīā (le stade entre ʻōuo et ʻōmoto, l'eau sucrée, l'amande fine) et d'où vient le coco | Texte FR/EN, deux versions (30 s et 2 min) ; forme le guide à la première sortie | Récit déformé (« coco bio », « coco de Tahiti » générique) ; guide anglophone peu à l'aise | Phrases entendues notées mot pour mot ; questions des passagers |
| A7 Après — coques | Coques dans un bac ou sac solide, retour au bateau, puis à la base | Reprend les coques à la livraison suivante si l'opérateur le souhaite (compost, cocoteraie partenaire : à instruire avec `supply-analyst`) | Coques laissées sur le motu ; bac percé ; odeur | Poids/nombre de coques rapportées vs servies |
| A8 Après — retours | Le capitaine note ce que les clients ont dit ; l'équipage dit ce qui l'a gêné | Passe ou appelle le vendredi : 5 minutes, 3 questions ; consigne les verbatims | On n'a que « c'était bien » ; l'équipage ne dit pas que ça l'ennuie | Verbatims cités ; incidents ; demandes |
| A9 Réassort | Commande suivante, ajustée aux réservations et aux restes | Propose la quantité, signale la DLC des restes | Restes périmés ; sur-commande par prudence puis sous-commande par réaction | Taux de recommande ; cocos jetés / livrées |

**(b) Fil passager**

| Étape | Ce qui se passe | Ce que fait NĪĀ | Ce qui peut rater | Ce qu'on mesure |
|---|---|---|---|---|
| P1 Découverte (avant) | Le passager a réservé via l'hôtel, une agence ou le site de l'opérateur ; « rafraîchissements inclus » | Rien d'obligatoire ; option : une ligne « coco nīā NĪĀ incluse » dans le descriptif, si l'opérateur le souhaite | Promesse sur-vendue (« fresh coconut » puis coco absente un jour de rupture) | Mention présente ou non dans la description |
| P2 Mise en scène | Le guide sort une glacière et annonce « maintenant, un coco » | Marquage visible, facettes propres, buée de froid | Coco sale, bourre humide qui coule, marquage délavé | Réaction immédiate observée (sourire, téléphone sorti) |
| P3 Geste de réception | Le passager prend le coco à deux mains ; elle est froide, lourde (≈ 1 kg) | Facettes qui tiennent bien en main ; ouverture faite devant lui en un geste | Coco trop lourde pour un enfant ; ouverture ratée qui éclabousse | Nombre de refus (ne veut pas de coco) ; nombre de cocos pour deux |
| P4 Goût | Eau froide, sucrée, goût du nīā ; souvent la première coco froid de sa vie | Stade nīā constant ; température de service 4–8 °C | Coco tiède ; eau acide (stade trop mûr ou DLC dépassée) ; quantité inégale | Verbatims sur le goût ; cocos non finies |
| P5 Photo | Coco en main, lagon derrière, groupe ; selfie | Facette marquée tournée vers l'objectif par le geste du guide | Rien à photographier de distinctif | Part des passagers qui photographient ; ce qu'ils cadrent (le coco ? le marquage ? le guide ?) |
| P6 Amande | Après l'eau, le guide ouvre le coco en deux et fait goûter l'amande fine et molle du nīā | Geste de finition conçu pour ne pas dépendre d'une machette (à valider avec `process-engineer`) | Impossible sans machette → le numéro du guide revient, et c'est acceptable sur le motu | Fait ou non ; réaction |
| P7 Souvenir et récit | Le soir, le passager raconte « le coco froid du motu » ; poste la photo ; demande où en trouver | Un mot de marque mémorisable ; pas de QR code ni de site tant que le second temps n'est pas ouvert | Le passager retient « coco » et pas « NĪĀ » ; il cherche la marque et ne trouve rien | Nom cité spontanément ou non ; questions « où en acheter ? » (signal pour le palier 2) |

**Friction principale J1** : l'étape A5. Le motu est le territoire du guide et de sa machette. L'angle à tester : NĪĀ apporte le froid, le stade et la régularité ; le guide garde le geste final et l'amande (P6). Si le guide refuse ce partage, l'opérateur n'est pas un bon pilote.

### 3.2 J2 — Sortie bateau courte sans débarquement (snorkeling ; baleines en saison)

Contexte type `[estimé]` : départ 8h30 et 13h30 d'une marina ou d'une plage, 8–20 pax, un capitaine et un guide, 2–3 arrêts dans l'eau, retour 11h30 / 16h30. En saison des baleines : mêmes bateaux ou semi-rigides plus petits, 8–12 pax, 3–4 h, longues phases de recherche. Une seule glacière à bord en général.

**(a) Fil opérateur et équipage**

| Étape | Ce qui se passe | Ce que fait NĪĀ | Ce qui peut rater | Ce qu'on mesure |
|---|---|---|---|---|
| A1 Commande | Deux sorties par jour : l'opérateur commande à la semaine sur la base des réservations, par jour | Confirme ; quantité = pax réservés + 10 % ; arrondit à la caisse (par 10 ou 12 `[supposé]`) | Variabilité forte des demi-journées (météo, annulations hôtel) | Écart commandé / servi ; annulations |
| A2 Réception | Comme J1 ; souvent base à la marina ou à la maison du patron | Idem J1 ; vise une livraison avant 7h pour la sortie du matin | Marina sans frigo ; livraison entre deux sorties impossible (équipage en mer) | Température ; heure ; signature |
| A3 Stockage | Idem J1 ; les cocos de l'après-midi restent à terre au frais pendant la sortie du matin | Glacière NĪĀ dédiée ; pains de glace en double jeu | Les cocos des deux sorties embarquées le matin et exposées 8 h | Température des cocos de l'après-midi au service |
| A4 Embarquement | 8h : les cocos du matin dans la glacière du bord | Caisse dimensionnée pour une glacière de 60 L (10–12 cocos) | Pas de place : glacière unique déjà pleine d'eau et de masques | Nombre embarqué |
| A5 Service | **Après le dernier arrêt, moteur relancé** : le guide ouvre et distribue pendant les 15–25 min de retour, passagers assis | Ouverture en un geste sur support stable (planche sur la glacière) ; pas de machette à bord en route ; cocos ouvertes au fur et à mesure | Mer agitée : ouverture dangereuse, cocos renversées ; guide seul, doit aussi ranger le matériel | Durée du service pour N pax ; incidents ; cocos renversées |
| A5' Service en saison baleines | **Pendant l'attente** entre deux observations, moteur réduit, ou après la mise à l'eau | Idem ; le coco froid après 20 min dans l'eau à 26 °C est un moment fort | Observation qui arrive au moment du service → cocos abandonnées sur le pont | Moment choisi ; cocos finies |
| A6 Récit | Trois phrases du guide pendant la distribution | Texte FR/EN court (30 s) : au retour, personne n'écoute 2 minutes | Bruit moteur ; guide muet | Phrases dites ; questions |
| A7 Coques | Seau ou bac à bord ; vidé à la base | Reprise des coques à la livraison suivante si souhaité | Coques jetées par-dessus bord (image et réglementation) | Coques rapportées / servies |
| A8 Retours | Capitaine et guide après la sortie | 5 minutes, 3 questions, une fois par semaine | Idem J1 | Verbatims |
| A9 Réassort | Hebdo, ajusté | Idem | Idem | Taux de recommande |

**(b) Fil passager**

| Étape | Ce qui se passe | Ce que fait NĪĀ | Ce qui peut rater | Ce qu'on mesure |
|---|---|---|---|---|
| P1 Découverte | Réservation demi-journée, souvent la veille à l'hôtel ; attentes centrées sur les raies et requins | Rien d'imposé ; le coco est une surprise à l'arrivée | — | Mention dans le descriptif |
| P2 Moment | Sortie de l'eau, bouche salée, soleil, le bateau repart ; le guide tend un coco froid | Le contraste froid/sel/sucre est l'argument produit | Coco tiède = effet nul | Réaction ; verbatims |
| P3 Geste | Le passager boit assis, coco calée entre les genoux ; mains mouillées | Facettes antidérapantes de fait ; ouverture propre, pas d'éclaboussure | Coco qui glisse, se renverse sur le pont | Cocos renversées |
| P4 Goût | 300–500 ml d'eau froide `[estimé : contenu d'un coco jeune]` en 5 minutes | Stade nīā constant | Acide, tiède, trop ou pas assez | Cocos non finies |
| P5 Photo | Moins de photos qu'au motu (mains mouillées, bateau qui bouge) ; photo de groupe au retour avec cocos | Marquage visible ; le guide propose la photo de groupe | Aucune photo → faible effet d'image | Part de passagers photographiant |
| P6 Amande | Pas le temps ni l'outil en route ; option à la marina à l'arrivée | Pas prévu en J2 (différence assumée avec J1) | Frustration de ceux qui connaissent | Demandes « et la chair ? » |
| P7 Souvenir | « On a bu un coco glacé en revenant des requins » ; recommande le tour | Nom et marquage mémorisables | Marque non retenue | Nom cité ; questions « où en trouver ? » |

**Friction principale J2** : A5. Tout doit tenir en 15–20 minutes, en mouvement, avec un seul guide : l'ouverture doit être un geste d'une seconde sur un support stable, sans outil long, et la coque doit aller droit au seau. Si `process-engineer` ne livre pas un diamond cut « à ouvrir d'une pression » et un ouvre-coco sûr, J2 se dégrade.

### 3.3 J3 — Safari 4x4 intérieur de l'île (secondaire haute, test de généralisation)

Contexte type `[estimé]` : départ 8h30 et 13h30 d'un parking ou d'un hôtel, 8 pax par camion ouvert, 1–4 camions, 3,5–4,5 h, 3–5 arrêts (belvédère, cascade, plantation, site archéologique), glacière de 40–60 L à l'arrière pour l'eau.

**(a) Fil opérateur et équipage**

| Étape | Ce qui se passe | Ce que fait NĪĀ | Ce qui peut rater | Ce qu'on mesure |
|---|---|---|---|---|
| A1 Commande | Hebdo, par camion et par sortie ; multiples de 8 | Confirme ; caisse de 8 = un camion, une sortie | Agences qui remplissent les camions la veille | Écart commandé / servi |
| A2 Réception | Base = garage ou maison du patron, souvent avec frigo ou congélateur `[supposé]` | Livre tôt ; température ; bon | Chauffeurs qui partent de chez eux sans passer par la base | Heure ; température |
| A3 Stockage | Frigo de la base ; glacière dédiée par camion avec pains de glace | Glacière NĪĀ par camion pendant le pilote | Pains de glace non recongelés ; glacière partagée avec l'eau | Température au service |
| A4 Chargement | 8h : glacière à l'arrière, sanglée | Caisse qui rentre dans une glacière de 40 L | Glacière en plein soleil sur le plateau | Position de la glacière observée |
| A5 Service | **Au belvédère ou à la cascade**, 15–25 min, passagers à terre ; le chauffeur-guide ouvre sur le hayon | Ouverture sur le hayon = support stable ; fiche du geste et des trois phrases | Le guide a déjà sa dégustation de fruits et sa coco à la machette ; il sert à l'arrêt ananas où un stand vend déjà des jus | Moment choisi ; durée ; qui ouvre |
| A6 Récit | Le guide raconte beaucoup en 4x4 (histoire, plantes) ; le nīā s'insère naturellement dans son discours sur le cocotier | Texte 2 min, version botanique (ʻōuo, nīā, ʻōmoto, haʻari) | Dilué dans un discours déjà long | Phrases dites ; questions |
| A7 Coques | Bac à l'arrière, retour à la base | Reprise possible | Coques laissées au belvédère (site public, image désastreuse) | Coques rapportées / servies |
| A8 Retours | Chauffeurs-guides, souvent plusieurs par opérateur : retours hétérogènes | Un passage par semaine à l'heure du retour | Le patron ne monte plus en camion, ne voit rien | Verbatims par chauffeur |
| A9 Réassort | Hebdo | Idem | Idem | Taux de recommande |

**(b) Fil passager**

| Étape | Ce qui se passe | Ce que fait NĪĀ | Ce qui peut rater | Ce qu'on mesure |
|---|---|---|---|---|
| P1 Découverte | Réservation à l'hôtel ou sur le quai ; attentes : paysages, fraîcheur de la montagne | Rien d'imposé | — | Mention |
| P2 Moment | Arrêt au point de vue, poussière, chaleur ; le guide ouvre la glacière | Coco froide au moment où l'on redescend du camion | Coco tiède après 2 h de piste | Réaction |
| P3 Geste | Debout, coco en main, vue derrière | Ouverture sur le hayon | File d'attente de 8 devant un seul guide | Durée de service |
| P4 Goût | Idem J1 | Idem | Idem | Cocos non finies |
| P5 Photo | **Très forte** : coco en main devant la baie de Cook ou la vallée de la Papenoo | Marquage ; le guide propose la photo | Rien de distinctif dans le cadre | Part qui photographie |
| P6 Amande | Possible à l'arrêt (temps, support) ; compatible avec le couteau du guide | Geste de finition | — | Fait ou non |
| P7 Souvenir | « Un coco froid au belvédère » | Nom | Marque non retenue | Nom cité |

**Friction principale J3** : le froid (A3–A5) et le prix (P du §2). Le camion ouvert, la poussière et la glacière ouverte à chaque arrêt dégradent la température ; et 500 XPF pèsent 7–10 % d'un billet demi-journée. J3 n'a de sens qu'avec une glacière dédiée par camion et un opérateur dont le patron croit à la montée en gamme.

---

## 4. Choix de l'opérateur pilote, objections, modèle de commande, conservation

### 4.1 Critères de choix du pilote (grille commune, pondérée par cible)

| Critère | Seuil souhaité | Pourquoi | J1 motu | J2 bateau court | J3 4x4 |
|---|---|---|---|---|---|
| Taille | 1–3 bateaux ou 2–4 camions ; 60–250 pax/semaine | Assez pour apprendre, pas assez pour saturer une découpe manuelle | 1–2 bateaux | 1–2 bateaux, 2 sorties/jour | 2–3 camions |
| Régularité | ≥ 4 sorties/semaine toute l'année | Une tournée de livraison hebdomadaire ne se justifie pas en dessous | Journée quotidienne | Idéale | Correcte |
| Port d'attache | **Tahiti d'abord** (Punaauia, Papeete, Teahupoo) ; Moorea si l'opérateur a un frigo et réceptionne au ferry | La logistique inter-îles est un risque de `VISION.md`, pas un détail | Tahiti Iti ou Moorea | Punaauia/Papeete | Papenoo (Tahiti) ou Opunohu (Moorea) |
| Équipement froid | Frigo à la base **ou** accepte une glacière dédiée et des pains de glace | Décide du rythme de livraison (§4.4) | Souvent oui (poisson) | Variable | Souvent oui (base garage) |
| Décideur | Patron-capitaine joignable, qui monte encore à bord | Les retours doivent remonter sans filtre | Oui | Oui | Risque : patron à terre |
| Ouverture au changement | A déjà changé quelque chose dans son offre depuis 2 ans ; accepte un prix supérieur au coco de bord de route | Risque n° 3 (prix) ; objection « on a déjà des cocos » | À tester fort | Plus facile | À tester |
| Visibilité | Bien noté sur les plateformes d'avis, référencé par 1–2 hôtels ou agences | Les premiers ambassadeurs doivent être vus | Forte | Forte | Moyenne |
| Rituel coco existant | Pas de machette comme numéro central ; ou guide d'accord pour garder la finition | Sinon, NĪĀ est perçue comme une perte de spectacle | Critère éliminatoire | Rare | À vérifier |
| Acceptation du pilote | Accepte un pilote **payant**, 6–8 semaines, un passage de NĪĀ à bord par semaine, et des retours cités | Un pilote gratuit ne teste pas le prix | Oui | Oui | Oui |

### 4.2 Objections attendues et réponses (par cible)

Verbatims : **à relever mot pour mot** sur le terrain, colonne de droite laissée vide à dessein. Les formulations ci-dessous sont des hypothèses d'objection, pas des citations.

| Objection (hypothèse) | Où elle pèse | Réponse à tester | Verbatim relevé (date, opérateur) |
|---|---|---|---|
| « On a déjà des cocos, je les ouvre moi-même devant les clients. » | J1 (fort), J3 | « Gardez le geste. Nous apportons ce que la machette ne peut pas : le coco froid, le bon stade à chaque fois, la régularité, et 20 minutes de préparation en moins le matin. » | ___ |
| « 500 francs le coco, j'en achète à 150 au bord de la route. » `[estimé : prix d'un coco jeune non préparée, à relever]` | Toutes, J3 surtout | Décomposer : stade sélectionné, découpe, froid, livraison, régularité ; comparer au coût d'un jus en bouteille servi à bord ; proposer de **mesurer la réaction des clients sur 6 semaines** avant de juger le prix | ___ |
| « Mes clients ne verront pas la différence. » | J2 | Faire goûter à l'équipage un coco NĪĀ froide et un coco du matin côte à côte ; demander qui a vu la différence | ___ |
| « Et si vous ne livrez pas un lundi ? » | Toutes | Stock tampon de 2 jours chez l'opérateur ; engagement de prévenir 48 h avant ; **ne pas promettre une régularité qu'`operations-director` n'a pas validée** | ___ |
| « C'est propre, votre truc ? Combien de temps ça se garde ? » | Toutes | DLC écrite sur la caisse ; température à la réception signée ; renvoi à l'item 5 (réglementaire) — ne rien affirmer avant | ___ |
| « Je n'ai pas de place dans la glacière. » | J2, J4 jet-ski | Glacière dédiée prêtée pendant le pilote ; caisse dimensionnée | ___ |
| « Qu'est-ce que je fais des coques ? » | J1, J3 | Bac fourni ; reprise à la livraison suivante | ___ |
| « Les agences ne me paieront pas plus cher. » | J3, J9 | Le coco est un argument de vente pour l'agence (photo, « fresh young coconut included ») ; tester avec une agence | ___ |
| « Je peux apprendre la découpe à mon matelot. » | Toutes (internalisation) | Oui ; mais le stade nīā, le froid de bout en bout et la régularité ne s'apprennent pas en une matinée ; la marque n'est pas copiable | ___ |
| « Pourquoi personne ne le fait déjà ? » | Toutes | Question du pré-mortem (item 1) : répondre honnêtement qu'on cherche à le savoir avec eux | ___ |

### 4.3 Modèle de commande proposé

| | J1 motu | J2 bateau court / baleines | J3 4x4 |
|---|---|---|---|
| Unité | Caisse consignée de 10–12 `[supposé]` | Caisse de 10–12 | Caisse de 8 (un camion, une sortie) |
| Fréquence | Hebdo (lundi) si frigo ; lundi + jeudi sinon | Hebdo si frigo ; lundi + jeudi sinon (2 sorties/jour épuisent vite) | Hebdo si frigo à la base |
| Quantité | Pax réservés de la semaine + 10 % | Idem, par demi-journée | Multiples de 8 par camion-sortie |
| Délai de commande | Jeudi 18h pour le lundi ; ajustement possible jusqu'à la veille 18h | Idem | Idem |
| Livraison où et quand | Base ou quai, 6h30–7h30 ; Moorea : réception au ferry du matin par l'opérateur ou tournée NĪĀ sur l'île (coût à chiffrer en A1) | Marina ou plage de départ, avant 7h | Base/garage, avant 8h |
| Reprise | Caisses vides, coques (optionnel), invendus périmés comptés | Idem | Idem |
| Facturation | Hebdo, sur bon signé, à le coco livré ; les invendus périmés sont au compte de l'opérateur au-delà du +10 % `[supposé : règle à négocier]` | Idem | Idem |
| Prix | Fourchette 400–800 XPF `[supposé]` — **voir A1 pour le prix retenu** | Idem | Idem (pression à la baisse attendue) |

### 4.4 Conséquences sur la conservation et le rythme

L'intuition « deux semaines en stock réfrigéré » n'est **pas vérifiée** (`VISION.md`, item 4). Le rythme de livraison dépend de deux inconnues : la DLC réelle après découpe (D, en jours) et l'autonomie de froid chez l'opérateur (A, en jours).

| Cas | A (opérateur) | D (DLC) | Rythme | Conséquence pour NĪĀ |
|---|---|---|---|---|
| Opérateur avec frigo, DLC ≥ 7 j | 7+ | 7+ | Hebdo | Une tournée par semaine suffit ; Moorea jouable |
| Opérateur avec frigo, DLC 4–5 j | 7+ | 4–5 | Bi-hebdo (lundi, jeudi) | Deux tournées ; Moorea coûteuse |
| Opérateur sans frigo (glacière + glace) | 2 | ≥ 4 | **Bi- ou tri-hebdo** | Prêter un petit réfrigérateur (question posée dans les notes du fondateur) devient rentable dès que le volume dépasse ~100 cocos/semaine `[estimé : un frigo d'occasion contre deux tournées supplémentaires par semaine]` |
| Opérateur sans frigo, DLC courte | 2 | 2–3 | Quotidien | Incompatible avec un fondateur seul ; refuser ce pilote |

Règle pratique pour le pilote : **choisir un opérateur avec frigo à Tahiti**, livrer hebdo, et mesurer D sur le terrain en même temps que `process-engineer` le mesure en laboratoire. Un pilote à Moorea n'a de sens qu'avec A ≥ 7 et D ≥ 7.

---

## 5. Potentiel par cible prioritaire

Toutes les lignes sont `[estimé]` ; raisonnement : nombre de prestataires actifs par type d'après la densité d'offre visible depuis les hôtels et les quais (à remplacer par le recensement du plan §6, et par les listes de Tahiti Tourisme et des comités du tourisme de Moorea et Tahiti Iti). Taux de prise = part des passagers qui acceptent le coco incluse : 85–95 %, arrondi à 1 coco par passager pour la commande.

### 5.1 Nombre d'opérateurs et cocos par semaine et par opérateur

| Cible | Opérateurs Tahiti | Opérateurs Moorea | Pax / semaine par opérateur (HS) | Cocos / semaine (HS) | Cocos / semaine (BS) |
|---|---|---|---|---|---|
| J1 lagon journée motu | 8–15 (Punaauia, Teahupoo, Tetiaroa) | 15–25 | 1–2 bateaux × 15–25 pax × 5–6 sorties = 75–250 | 75–250 | 40–120 |
| J2 bateau court snorkeling | 6–12 | 10–20 (recouvrement fort avec J1 : mêmes bateaux) | 2 sorties × 10–20 pax × 6 j = 120–240 | 120–240 | 50–120 |
| Baleines (saison, 5 mois) | 5–10 | 10–15 | 2–3 sorties × 8–12 × 6 j = 100–200 | 100–200 | 0 hors saison |
| J3 safari 4x4 | 5–8 | 5–8 | 2 sorties × 8 pax × 2–3 camions × 6 j = 190–290 | 190–290 | 80–150 |
| Sunset cruise hôtel / catamaran | 3–5 | 4–6 | 3–6 sorties × 15–40 = 60–200 | 60–200 | 30–100 |

Ensemble adressable palier 1 (prioritaires + 4x4) : **40–80 opérateurs distincts** sur les deux îles, après déduplication J1/J2/baleines `[estimé]`. Dix clients représentent donc 12–25 % de l'adressable : un objectif de deuxième année, pas de première.

### 5.2 Chiffre d'affaires mensuel pour NĪĀ

Hypothèses : 4,3 semaines/mois ; un opérateur « type » prioritaire = 75–150 cocos/semaine en haute saison (bas de fourchette J1 ou J2 avec un seul bateau), moitié en basse saison ; prix 400–800 XPF `[supposé]`, **voir A1 pour le prix retenu**.

| Scénario | Cocos / mois HS | CA / mois HS à 400 | CA / mois HS à 800 | Cocos / mois BS | CA / mois BS (400–800) |
|---|---|---|---|---|---|
| 1 opérateur | 320–650 | 0,13 M XPF | 0,52 M XPF | 170–340 | 0,07–0,27 M XPF |
| 3 opérateurs (mix J1/J2 + 1 autre) | 1 300–2 150 | 0,52 M XPF | 1,72 M XPF | 650–1 100 | 0,26–0,88 M XPF |
| 10 opérateurs | 4 300–7 300 | 1,72 M XPF | 5,84 M XPF | 2 100–3 700 | 0,84–2,96 M XPF |

Lecture : à 1 opérateur, le palier 1 ne paie personne ; il **apprend**. À 3, il paie un découpeur à temps partiel et une tournée hebdomadaire (à confirmer en A1 avec le coût de revient). À 10, il commence à financer une machine — mais 10 opérateurs, c'est 1 000–1 700 cocos par semaine en haute saison, hors de portée d'une découpe manuelle par une personne `[estimé : à 3–5 min par coco, 1 000 cocos = 50–80 h de découpe]`. Le volume et la capacité de découpe doivent croître ensemble ; c'est exactement l'arbitrage buy or make (item 9).

Le canal croisière, lissé, ajoute en théorie 70 062 passagers/an, soit ~1 350 par semaine ; en pratique des pics de 100–300 cocos un jour d'escale. À viser quand la capacité de découpe le permet, par l'intermédiaire des opérateurs J1/J2/J3 qui travaillent déjà les escales, jamais en direct.

---

## 6. Plan de prospection des 8 premières semaines

Principe : **écouter avant de proposer** (karpathy). Chaque visite commence par 10 minutes de questions et un coco à faire goûter à l'équipage, pas par un pitch. Les fiches produites doivent être reprenables par un commercial recruté : un fichier par opérateur, la grille §6.3 remplie, les verbatims datés.

### 6.1 Ce qu'on a en main

- Une **glacière de 10–12 cocos nīā diamond cut, froides**, préparées la veille selon le protocole en cours de l'item 4 (même imparfait : c'est un prototype, on le dit) ; un ouvre-coco ou couteau court ; un bac pour les coques ; un thermomètre.
- Une **fiche d'une page** : ce qu'est le nīā, ce que NĪĀ livre (coco froid, stade sélectionné, livrée à la base, caisse consignée), ce qu'on propose (pilote payant 6–8 semaines), fourchette de prix (voir A1), ce qu'on demande en retour (retours cités, un passage à bord par semaine).
- La **grille d'entretien** (§6.3) et un carnet pour les verbatims.
- Pas de contrat, pas de plaquette marque : le laboratoire de marque commence au pilote, pas en prospection.

### 6.2 Qui aller voir, dans quel ordre

| Semaine | Où | Qui (catégorie ; noms à confirmer sur place) | Objectif | Livrable |
|---|---|---|---|---|
| S1 | Tahiti, côte ouest (marina Taina, Punaauia, Papeete) | Sources de liste : comptoirs d'activités des hôtels de Punaauia, Tahiti Tourisme (liste des prestataires), 1–2 agences réceptives (DMC) ; 2–3 opérateurs J2 snorkeling/dauphins | Recenser 10–15 opérateurs bateau de Tahiti avec décideur et téléphone ; 3 premiers entretiens | 10–15 fiches amorcées ; 3 grilles remplies |
| S2 | Tahiti Iti (Teahupoo, Vairao) | Taxi-boats et sorties lagon/vague J1-J2 ; 3–4 entretiens | Tester l'objection « on a déjà des cocos » dans le contexte motu | 3–4 grilles ; premiers verbatims |
| S3 | Moorea (2 jours sur place : Vaiare, Temae, Papetoai/Opunohu, Haapiti) | Opérateurs J1 lagon-motu (4–6), J2/baleines (2–3) ; comité du tourisme de Moorea comme source de liste | Comparer Tahiti/Moorea sur le froid, la réception au ferry, le prix | 6–9 grilles ; carte Moorea |
| S4 | Tahiti (Papenoo) et Moorea (Opunohu) | Opérateurs J3 safari 4x4 (3–4) ; 1 opérateur de quad pour fermer la question | Tester la règle de généralisation à terre ; relever la pratique coco/fruits | 4–5 grilles |
| S5 | Tahiti et Moorea | Appoints : 1–2 centres de plongée, 1 charter de pêche, 1 jet-ski guidé ; **1 hôtel pour sa sunset cruise** (responsable F&B ou activités : noter le contact pour le palier 2, ne pas vendre le palier 2) | Compléter la matrice avec du relevé ; confirmer les classes « secondaire » | 4–5 grilles ; matrice révisée |
| S6 | Retour chez les 4–6 meilleurs | Deuxième visite avec cocos : goûter avec tout l'équipage ; **monter à bord d'une sortie** chez 2 d'entre eux en observateur | Observer le moment de service réel, le rituel machette, les glacières | 2 comptes rendus d'observation à bord |
| S7 | Synthèse | Avec `business-director` et `operations-director` : choisir 1 pilote (et 1 remplaçant) ; vérifier que le rythme de livraison est tenable (§4.4) et validé par `operations-director` | Décision pilote | Fiche pilote : opérateur, rythme, durée, critères de réussite |
| S8 | Chez le pilote | Proposition écrite d'une page, prix (A1), calendrier de première livraison, grille de mesure (§3) | Accord oral puis écrit sur un pilote payant | Pilote signé ; date de première livraison |

Repères : 25–35 entretiens en 8 semaines ; 2 observations à bord ; 1 pilote signé, 1 remplaçant identifié. Si à S5 aucun opérateur n'a dit « combien et quand ? », c'est un signal fort pour le pré-mortem (item 1) : remonter au DG avant S7.

### 6.3 Grille d'entretien — 10 questions (dans cet ordre, les trois premières avant de sortir la glacière)

1. Combien de sorties faites-vous par semaine en ce moment, et combien de passagers par sortie ? Et en février ? *(volume, saisonnalité)*
2. Qu'est-ce que vous servez à boire et à manger à bord ou à l'arrêt, et à quel moment ? *(moment, pratiques)*
3. Est-ce que vous servez des cocos aujourd'hui ? Lesquelles, combien, achetées où, à quel prix, qui les ouvre, avec quoi ? *(usage actuel, internalisation, prix de référence)*
4. Où stockez-vous vos boissons avant la sortie : frigo à la base, glacière, glace achetée où ? *(froid, autonomie A)*
5. Comment gérez-vous vos déchets de sortie ? *(coque)*
6. Qui décide de ce qui est inclus dans l'excursion et du prix du billet ; vos places sont-elles vendues par des hôtels ou des agences, et à quel pourcentage ? *(décideur, place du prix)*
7. *(faire goûter)* Qu'est-ce que vous en pensez, vous et l'équipage ? Vos clients verraient-ils la différence avec un coco du matin ? *(verbatim, goût)*
8. À quel moment de votre sortie la serviriez-vous ? Qui l'ouvrirait ? *(moment, geste — c'est l'opérateur qui dessine le journey)*
9. À combien le coco, livrée froide à votre base chaque semaine, cela resterait-il intéressant pour vous ? *(prix — laisser répondre, ne pas annoncer le prix en premier)*
10. Si on faisait un essai de 6 semaines, payant, avec un passage de notre part à bord une fois par semaine : qu'est-ce qui vous ferait dire oui, et qu'est-ce qui vous ferait arrêter ? *(critères de réussite, objections)*

À relever en plus, sans question : nom et rôle de l'interlocuteur, île et point de départ, nombre et taille des bateaux/camions, glacières vues (nombre, litres), présence d'une machette à bord, réaction au mot « nīā ».

### 6.4 Ce qui déclenche la proposition de pilote

Proposer le pilote **dès la première visite** si, et seulement si, les cinq conditions sont réunies ; sinon, revenir en S6 :

1. Le décideur est devant nous et a répondu « combien et quand ? » ou l'équivalent, sans qu'on le lui souffle.
2. Volume ≥ 60 pax/semaine, ≥ 4 sorties/semaine, toute l'année ou au moins sur les 3 mois du pilote.
3. Froid : frigo à la base, ou accord pour une glacière dédiée et un stock de 2 jours (et dans ce cas, livraison bi-hebdo tenable depuis Tahiti).
4. Prix : la réponse à la question 9 tombe dans la fourchette A1, ou au-dessus de son bas.
5. Rituel : pas de machette comme numéro central, ou accord explicite pour que NĪĀ amène le coco froid et que le guide garde la finition.

Si la condition 1 est remplie mais pas la 3 ou la 5 : ne pas forcer ; c'est un bon deuxième client, pas un bon premier.

---

## Les 3 types d'excursion où aller en premier et pourquoi, en 5 lignes

1. **Sortie bateau courte snorkeling (Tahiti côte ouest, puis Moorea)** : deux sorties par jour toute l'année, pas de motu donc pas de machette installée, une glacière suffit, le service tient sur le trajet retour ; c'est le flux le plus régulier pour apprendre à livrer.
2. **Sortie lagon journée avec motu (Tahiti Iti et Moorea)** : le plus gros volume par sortie et la meilleure image, mais le guide y a déjà sa coco à la machette ; on y va pour tester frontalement l'objection « on a déjà des cocos » et pour y insérer NĪĀ sans voler le numéro.
3. **Observation des baleines (juillet–novembre)** : mêmes opérateurs que 1 et 2, billets à 12 000–16 000 XPF où 500 XPF sont invisibles, longues attentes idéales pour servir ; c'est l'extension naturelle du pilote dès l'été 2027 si les premières livraisons ont lieu au printemps.
Le safari 4x4 vient juste derrière, comme meilleure cible terrestre et seul test sérieux de la règle « le coco suit la glacière, la glacière suit le véhicule » hors du bateau.

---

## Annexe — Hypothèses à remplacer par du relevé, et ce que ce document ne dit pas

- Tous les prix de billets, nombres de passagers, nombres d'opérateurs et pratiques « ce qui est servi aujourd'hui » sont `[estimé]` ou `[supposé]` : 25–35 entretiens (§6) les remplacent.
- La DLC après découpe et l'autonomie de froid chez l'opérateur sont des inconnues qui **décident du rythme de livraison** (§4.4) : items 4 et 5 du backlog.
- Le prix par coco n'est pas fixé ici : **voir A1**.
- Le geste d'ouverture « sans machette » du diamond cut est supposé possible ; `process-engineer` doit le confirmer, sans quoi J2 perd une partie de sa valeur.
- Les noms d'opérateurs ne sont pas listés : sans web ni terrain, une liste serait inventée. Les sources de liste sont indiquées (hôtels, Tahiti Tourisme, comités du tourisme, agences réceptives) ; la première semaine du plan sert à la constituer.
- Ce document ne traite pas du CHR (item 13, palier 2) : la sunset cruise d'hôtel y est mentionnée uniquement comme pont, et l'anti-pattern « vendre le palier 2 à un prospect du palier 1 » s'applique.
