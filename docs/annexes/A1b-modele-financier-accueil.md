# Annexe A1b — Modèle financier de l'option « accueil premium via agences réceptives » (palier 1, cible prioritaire révisée)

> Statut : v0, estimations de bureau, **aucun chiffre relevé sur le terrain**. Rédigé le 2026-10-24 par `financial-modeler` pour `business-director`, à la suite du changement de cible décidé par le fondateur le 2026-10-24 : la cible prioritaire du palier 1 devient l'**accueil premium via les agences réceptives** (l'agence achète le coco nīā diamond cut froide marquée NĪĀ, l'intègre à sa prestation de transfert, son agent la remet au touriste à l'arrivée à l'hôtel ; l'hôtel gère la coque et peut servir de froid tampon). Les opérateurs d'excursion deviennent la seconde cible.
>
> Cette annexe **ne remplace pas A1** : elle en garde toutes les hypothèses unitaires, la méthode (VAN à trois flux, raccourcis de sensibilité, format de trésorerie) et ne reconstruit que ce qui change. Les hypothèses de volume sont posées **en fourchettes** et renvoient à l'**annexe A8** (`market-scout` : journeys, volumes de marché, objections) pour validation. Monnaie : XPF hors TVA. Horizon : 12 mois de pilote (novembre 2026 → octobre 2027) + 12 mois de régime.
>
> Étiquettes : **[relevé]** mesuré sur le terrain (aucun ici) · **[estimé : …]** déduit d'un raisonnement ou d'un ordre de grandeur connu de la Polynésie française · **[estimé : source web]** chiffre public, URL donnée · **[supposé]** hypothèse de travail à vérifier. **« A8 »** = à valider par l'annexe A8.

**Repères (scénario réaliste, découpe manuelle, Tahiti)** : coût variable livré hôtel **≈ 365 XPF** (220–620) · prix cible **700 XPF** par passager accueilli (plancher 500, fourchette 600–900) · marge **≈ 335 XPF (48 %)** · point mort **≈ 285 cocos/mois (≈ 10/jour)** · point bas de trésorerie **−1,87 M en juin 2027** (−2,35 M si les agences paient à 60 jours) · VAN à 12 % sur 24 mois **+1,6 M** contre −0,84 M pour les excursions (A1), **à condition** d'un prix net ≥ 590 XPF et d'un coco par passager (pas par dossier).

---

## 1. Ce qui change dans l'économie unitaire (par rapport à A1 § 1)

### 1.1 Les sept différences de canal et leur traduction en coût

| Différence | Excursions (A1) | Accueil via agence (A1b) | Effet retenu dans le modèle |
|---|---|---|---|
| Lieu et heure de livraison | Quai ou base de l'opérateur, avant 7 h 30, 25–40 cocos par point | 1 à 3 hôtels de Tahiti (Papeete, Punaauia, Faa'a) et de Moorea, **60–100 cocos par tournée**, **livraison de jour** si l'hôtel accepte un stock tampon | Transport Tahiti **30 XPF/coco** au lieu de 40 [estimé : tournée de 40 km ≈ 1 600 XPF répartie sur 60 cocos ≈ 27] ; glace **15** au lieu de 20 (temps en glacière plus court) |
| Régularité | 20–24 jours d'activité/mois, dépend de la météo et du remplissage | **7 jours sur 7 toute l'année**, pics aux jours d'arrivée des vols long-courriers et des têtes de ligne croisière à Papeete (jusqu'à ×2 la moyenne un jour donné [estimé : 150–330 passagers d'un paquebot en embarquement, cf. A8]) | Les fixes sont mieux absorbés ; mais quelqu'un doit livrer 7/7 : poste « relais de livraison » dans les fixes (§ 3) |
| Froid tampon | Chez l'opérateur, souvent inexistant (glacière à bord) | **Réfrigérateur de l'hôtel** (ou petit réfrigérateur NĪĀ prêté) : 2–3 jours de stock sur place | Découpe **3 séances/semaine** au lieu de 2 ; DLC exigée **≥ 5 jours** après découpe (jour J + 2–3 j de tampon + 1 j de marge) contre ≥ 7 j pour Moorea en A1 ; **invendus plus faibles** car l'agence connaît ses arrivées à J−1 (manifestes) |
| Perte | 15 % (hors stade, casse, invendus) | **12 %** (8–20) : invendus en baisse (volumes connus d'avance), mais **refus à réception plus sévères** (présentation hôtelière) | ÷ 0,88 au lieu de ÷ 0,85 |
| Présentation | Film + étiquette DLC + bandeau minimal (25 XPF) | **Accueil hôtelier** : étiquette ou bandeau NĪĀ soigné, **fiche** (le fruit, le geste, 2 langues), **paille** (papier ou bambou), éventuellement support ou manchon | **60 XPF/coco** (35–120) [supposé : étiquette imprimée localement 20–40, fiche 10–20, paille 10–30, manchon 0–40 ; borne haute 120 à ne pas dépasser, au-delà la marge Moorea disparaît] |
| Prix de référence du client | Coût actuel d'un coco servi par l'opérateur : 230–370 XPF | **Coût d'un geste d'accueil** par passager : lei de fleurs, welcome drink (§ 1.3) | Prix cible **700** au lieu de 500 |
| Main-d'œuvre | À la tâche (100 XPF/coco), pas de poste à remplir | Flux régulier : un **temps partiel salarié** devient possible (§ 1.4) | Année 1 : **100** (tâche) ; année 2 : **80** (contrat temps partiel sous-utilisé en basse saison) |

### 1.2 Coût de revient d'un diamond cut livré hôtel (XPF)

Formule inchangée : (achat + main-d'œuvre + glace + présentation) ÷ (1 − perte) + transport.

| Poste | Bas | **Central** | Haut | Source (A1 § 1.1 sauf mention) |
|---|---|---|---|---|
| Achat coco nīā au stade demandé | 80 | **120** | 160 | A1 [estimé], aucune source même web |
| Main-d'œuvre : réception, découpe, nettoyage, présentation, mise au froid | 60 | **100** (80 en année 2) | 150 | A1 [estimé : 3 min/coco] ; § 1.4 pour le salarié |
| Glace | 5 | **15** | 30 | [estimé : livraison de jour, 60 cocos, 1 sac de 5 kg ≈ 500 XPF] |
| Présentation NĪĀ accueil (étiquette, fiche, paille, support) | 35 | **60** | 120 | [supposé], à chiffrer par `brand-director` avec un imprimeur local |
| Sous-total avant perte | 180 | **295** | 460 | |
| Perte | 8 % | **12 %** | 20 % | [supposé] |
| Sous-total après perte | 196 | **335** | 575 | |
| Transport Tahiti (tournée groupée hôtels) | 15 | **30** | 50 | [estimé] ; 50 si livraison calée sur une arrivée de nuit sans tampon |
| **Coût variable livré hôtel, Tahiti** | **≈ 210** | **≈ 365** | **≈ 625** | A1 excursions : 350 (250–500) |
| **Moorea, variante « fret payant »** (+60, A1 § 1.5) | 250 | **≈ 425** | 745 | Variante **retenue** (prudente) |
| Moorea, variante « fret agricole gratuit » (+20) | 215 | ≈ 385 | 665 | [supposé, à vérifier Lexpol] : peu probable (sens Tahiti → Moorea, coco découpé) |
| **Moorea, variante « l'agence transporte »** (+0) : la glacière NĪĀ voyage dans le transfert de l'agence (van + ferry avec l'accompagnateur), remise à l'hôtel de Moorea | 210 | **≈ 365** | 625 | [supposé] : coût nul pour NĪĀ, mais glacière de prêt (§ 3), responsabilité de la chaîne du froid transférée, DLC à +1 jour ; **à poser à l'agence dès le premier entretien** |
| Coût complet Tahiti à 1 000 cocos/mois (fixes 95 k alloués) | | **≈ 460** | | |
| Coût complet Tahiti à 660 cocos/mois (moyenne M5–M12 du réaliste) | | ≈ 510 | | |

Le coût variable central ne bouge presque pas par rapport à A1 (**365 contre 350**) : la présentation hôtelière (+35) est compensée par la perte (−10), la glace (−5) et le transport (−10). Ce qui change, c'est le **prix**, la **régularité** et le **besoin de fonds** (§ 4).

### 1.3 Prix par passager accueilli : à quoi l'agence compare

L'agence ne revend pas le coco à l'unité : elle l'inclut dans un transfert ou un « welcome » vendu au tour-opérateur, ou l'offre comme signature. Le prix NĪĀ se compare au **coût d'un geste d'accueil par passager**, pas à un coco de roulotte.

| Référence | Coût pour l'agence ou l'hôtel | Source |
|---|---|---|
| Lei de fleurs fraîches (collier de tiare ou de fleurs) remis à l'aéroport | **400–800 XPF** (détail aux vendeuses de Faa'a et du marché : 500–1 500) | [estimé], à relever (A8, entretien agence) |
| Couronne de fleurs | 800–1 500 | [estimé] |
| Welcome drink à l'hôtel (jus, cocktail sans alcool) | 0 si offert par l'hôtel ; 500–1 200 s'il est facturé à l'agence ; coût matière 150–400 | [estimé] |
| Coco à boire : roulotte ou snack / bar d'hôtel | 300–500 / 800–1 200 | [estimé] |
| Transfert aéroport–hôtel vendu : partagé / privé | 2 000–4 000 / 6 000–12 000 par passager | [estimé] |
| Séjour de 10 nuits vendu par le tour-opérateur | 300 000–600 000 par personne : 700 XPF = **0,1–0,2 %** | [estimé] |

| Niveau de prix NĪĀ (HT, livré hôtel) | Tahiti | Moorea | Lecture |
|---|---|---|---|
| **Plancher** (couvre le variable + ≈ 135 XPF de fixes) | **500** | 560 | C'est le prix cible d'A1 : en dessous, le canal accueil ne vaut pas mieux que les excursions avec un CAPEX plus lourd (§ 5.4) |
| **Cible** | **700** | 700 (760 si le fret payant est refacturé) | Dans la fourchette du lei de fleurs, sous le welcome drink facturé ; **proposer 600 / 700 / 900** en entretien |
| Haut | 900 | 960 | Transferts privés, voyages de noces, clientèle nord-américaine (42 % des touristes [estimé : source web ISPF 2025, https://www.ispf.pf/content//uploads/1517_PC_Tourisme_2025_12_9e5f74a421.pdf]) |

| Marge unitaire à 700 XPF (année 1) | Tahiti | Moorea fret payant | Moorea « l'agence transporte » |
|---|---|---|---|
| Coût variable | 365 | 425 | 365 |
| **Marge sur coût variable** | **335 (48 %)** | 275 (39 %) | 335 (48 %) |

**Marge par livraison type** (60 cocos à un hôtel de Tahiti) : CA 42 000, variables 21 900, **marge 20 100 XPF**, contre 6 000 pour une livraison de 40 cocos à un opérateur (A1 § 1.3). Une commission ou remise d'agence s'impute directement : à 20 %, la marge Tahiti tombe à 195 (§ 5.5).

### 1.4 Main-d'œuvre : le temps partiel salarié devient-il possible ?

Base A1 : 3 min/coco → 20 cocos/h ; tâche ≈ 2 000 XPF/h soit **100 XPF/coco** ; salarié : SMIG **1 024,74 XPF brut/h au 01/05/2024** [estimé : source web, arrêté n° 580 CM, https://www.service-public.pf/trav/wp-content/uploads/sites/23/2024/05/Arrete-n°-580-CM-du-30_04_2024.pdf], retenu 1 050–1 100 en 2026 [supposé] + charges CPS ≈ 30–35 % → **≈ 1 450 XPF/h chargé → 75 XPF/coco si le poste est plein**.

| Contrat temps partiel (heures/mois) | Coût mensuel chargé | Capacité (20 cocos/h) | Coût/coco à 500 cocos/mois | à 800 | à 1 000 | à 1 500 |
|---|---|---|---|---|---|---|
| Tâche (référence) | proportionnel | illimitée | **100** | **100** | **100** | **100** |
| 40 h (≈ 10 h/semaine) | 58 000 | 800 | 116 | **73** | dépassé | dépassé |
| 52 h (≈ 12 h/semaine) | 75 400 | 1 040 | 151 | 94 | **75** | dépassé |
| 80 h (≈ 20 h/semaine) | 116 000 | 1 600 | 232 | 145 | 116 | **77** |

Lecture : un contrat de 40 h/mois devient moins cher que la tâche à partir de **≈ 580 cocos/mois durables**, un contrat de 52 h à partir de ≈ 750. Le flux 7/7 de l'accueil atteint ces seuils en **juillet 2027** dans le réaliste (§ 2.3), contre jamais vraiment pour un seul opérateur d'excursion. Mais la saisonnalité (indice 0,7 en février–mars) sous-utilise le contrat trois mois par an, et 7/7 suppose un remplaçant (congés, maladie) : le modèle retient **100 XPF en année 1 (tâche)** et **80 XPF en année 2** (contrat 52 h + tâche en pic), pas 75. Un salarié à temps partiel transforme aussi 60–75 k/mois de variable en **fixe** : le point mort monte d'autant si le volume recule (§ 3).

### 1.5 Transport vers les hôtels de Moorea

Trois variantes, même logique qu'A1 § 1.5 ; le modèle retient la variante payante (prudente) pour 20 % du volume à partir d'août 2027 et 25 % en année 2.

| Variante | Coût/coco | Condition | Qui vérifie |
|---|---|---|---|
| Fret payant (bac sur Aremiti/Terevau, remise au quai ou livraison par un relais à Moorea) | **+60** [estimé] | Devis fret, relais à Vaiare | `supply-analyst` |
| Fret agricole gratuit | +20 [supposé] | Éligibilité improbable (sens Tahiti → Moorea, produit découpé) | `supply-analyst` + `operations-director` (Lexpol, DGAE) |
| **L'agence transporte** dans son propre transfert (van + ferry, accompagnateur) | **0** [supposé] | Glacière NĪĀ prêtée, procédure écrite, DLC ≥ 6 j, l'hôtel de Moorea stocke | **Premier entretien agence** |
| Découpe à Moorea (option C d'A1 avec une cocoteraie de Moorea) | ≈ +20 (coût C − A) | Cocoteraie partenaire à Moorea | `supply-analyst` |

---

## 2. Hypothèses de volume, en fourchettes (à valider par A8)

### 2.1 De 281 227 touristes à des cocos par jour

| Étape | Valeur | Source |
|---|---|---|
| Touristes 2025 (arrivées internationales à Faa'a, hors excursionnistes de croisière) | 281 227 (+6,6 %), dont 227 286 en hébergement terrestre et 53 941 en tourisme flottant | [estimé : source web ISPF 2025, URL § 1.3] |
| Arrivées moyennes par jour | **≈ 770** ; par mois ≈ 23 400 × indice saisonnier | 281 227 ÷ 365 |
| Saisonnalité (indice, moyenne 1,0) | nov 0,9 · déc 1,0 · jan 0,9 · **fév 0,7 · mar 0,7** · avr 0,8 · mai 1,0 · juin 1,1 · **juil 1,3 · août 1,3** · sep 1,2 · oct 1,1 | A1 § 2.1 [estimé] ; A8 à recaler sur les arrivées mensuelles ISPF |
| Arrivées par jour selon la saison | ≈ 540 (indice 0,7) à ≈ 1 000 (indice 1,3) ; jours de vols long-courriers et têtes de ligne croisière jusqu'à ×1,5–2 la moyenne | [estimé] A8 |
| Part des arrivées prises en charge par **une** agence réceptive (accueil, transfert) | **3 niveaux : petite 3 % (≈ 23 pax/jour) · moyenne 8 % (≈ 60) · grande 15 % (≈ 115)** | [supposé] : une dizaine d'agences réceptives à Tahiti, une très grande et plusieurs moyennes ; A8 |
| Part des passagers accueillis dont la première nuit est à Tahiti ou Moorea (et non en correspondance directe vers une autre île) | **60 %** (50–70) | [supposé] : arrivées tardives, capacité hôtelière de Tahiti ; A8 |
| Un coco par **passager adulte** (90 % des passagers) ou par **dossier** (≈ 2,1 passagers) | **Central : par passager adulte** ; variante par dossier = volume ÷ 2,3 | [supposé] : le lei est remis par personne ; A8 et entretien agence. **Variable décisive**, cf. § 5.5 |
| **Cocos « équipables » par mois pour une agence qui équipe 100 % de ses passagers éligibles** | petite **≈ 375 × indice** · moyenne **≈ 1 000 × indice** · grande ≈ 1 875 × indice | 23 400 × part agence × 60 % × 90 % |
| Têtes de ligne croisière à Papeete (embarquements et débarquements, Paul Gauguin, Windstar, Aranui, etc.) | 53 941 touristes flottants/an ≈ 150/jour en moyenne, par pics de 150–330 un jour donné | [estimé : source web ISPF] ; **hors scénarios** (pics absorbés par le tampon de 2 jours ; opportunité A8) |
| Délai de paiement des agences | 30 jours (base) / **60 jours** (variante, § 5.5) | [supposé : les agences paient souvent à 30–60 jours] |

Ordre de grandeur du marché adressable par ce canal : 281 227 × 60 % première nuit Tahiti–Moorea × 90 % adultes ≈ **150 000 cocos/an**, dont la part passant par des agences réceptives (50–70 % [supposé], A8) ≈ 75 000–105 000. Le réaliste en année 2 (12 000) en prend 11–16 % ; le marché n'est pas la contrainte, **l'accès à une agence et le prix** le sont.

### 2.2 Trois scénarios

| | Minimal | **Réaliste** | Optimiste |
|---|---|---|---|
| Comptes | 1 agence (moyenne) qui n'équipe que 25 % de ses passagers éligibles et ne grossit pas | **1 agence moyenne** de mars 2027, montée de 20 % à 60 % de ses passagers éligibles ; **2e agence (petite)** à partir d'août 2027 | 2 agences moyennes (la 2e à 50 %) + 1 petite + **1 hôtel en direct** (≈ 20 arrivées/jour × 50 %) |
| Premières livraisons payantes | avril 2027 (M6) | **mars 2027 (M5)** | mars 2027 |
| Part Moorea | 0 % | 20 % à partir d'août 2027, 25 % en année 2 | 20 %, 25 % |
| Cocos année 1 | 1 950 | **5 280** | 13 490 |
| Cocos/mois en régime (année 2) | 250 | **1 000** (≈ 33/jour, 23 en février, 43 en août) | ≈ 2 500 (machine et équipe nécessaires) |
| Cocos année 2 | 3 000 | **12 000** | 30 000 |

### 2.3 Montée en charge mois par mois (cocos facturés)

Mois 1 = novembre 2026. M1–M3 : préparation (cocoteraie, protocole, test de conservation, réglementaire, **accord de principe de l'agence et de 2–3 hôtels sur le froid tampon**). M4 (février 2027) : 60 échantillons premium remis avec l'agence à ses propres clients, retours. **M5 (mars 2027) : premières livraisons payantes** sur un hôtel, segment premium de l'agence ; au plus tard fin avril 2027.

| Mois | Indice | Minimal | **Réaliste** (agence 1 : taux d'équipement × 1 000 × indice ; agence 2 : × 375 × indice) | Optimiste |
|---|---|---|---|---|
| M1 nov-26 | 0,9 | 0 | 0 | 0 |
| M2 déc-26 | 1,0 | 0 | 0 | 0 |
| M3 jan-27 | 0,9 | 0 | 0 | 0 |
| M4 fév-27 | 0,7 | 0 (échantillons) | 0 (60 échantillons) | 0 (échantillons) |
| M5 mar-27 | 0,7 | 0 | **140** (20 %) | 210 |
| M6 avr-27 | 0,8 | 200 | **240** (30 %) | 400 |
| M7 mai-27 | 1,0 | 250 | **400** (40 %) | 700 |
| M8 juin-27 | 1,1 | 275 | **550** (50 %) | 1 090 |
| M9 juil-27 | 1,3 | 325 | **780** (60 %) | 2 180 |
| M10 août-27 | 1,3 | 325 | **1 020** (780 + agence 2 à 50 %, dont 204 Moorea) | 3 220 |
| M11 sep-27 | 1,2 | 300 | **1 080** (720 + 360, dont 216 Moorea) | 2 970 |
| M12 oct-27 | 1,1 | 275 | **1 070** (660 + 410, dont 214 Moorea) | 2 720 |
| **Total année 1** | | **1 950** | **5 280** (dont ≈ 634 Moorea) | **13 490** (dont ≈ 2 220 Moorea) |

Tout [supposé] ; A8 doit confirmer la part de marché d'une agence moyenne, la part « première nuit à Tahiti–Moorea » et la règle « un coco par passager ». Le réaliste accueil fait **+21 % de volume en année 1 et +11 % en année 2** par rapport au réaliste excursions d'A1 (4 360 / 10 800), avec une courbe plus lisse (pas de zéro en février : indice 0,7, pas 0).

---

## 3. CAPEX et coûts fixes révisés

### 3.1 CAPEX (XPF, décaissés M1–M4)

Base A1 § 3 variante A (1 040 000), plus les postes propres au canal :

| Poste ajouté ou modifié | Montant | Source |
|---|---|---|
| Glacières de prêt dans les hôtels et pour les transferts de l'agence (6 × 10 000–15 000) | +60 000 | [estimé] |
| Froid tampon : 2 petits réfrigérateurs d'occasion dédiés NĪĀ si l'hôtel n'alloue pas d'espace dans son froid | +80 000 | [estimé : 30 000–50 000 pièce] ; 0 si les hôtels prêtent une étagère |
| Supports de présentation (présentoir ou plateau NĪĀ pour la remise, 3 × 15 000) | +45 000 | [supposé] |
| Matériel de marquage initial : étiquettes, fiches bilingues, pailles, premier lot de 1 000 | 100 000 au lieu de 50 000 | [supposé] |
| Imprévus ≈ 10 % | 105 000 au lieu de 100 000 | |
| **Total CAPEX A-accueil** | **≈ 1 280 000** (fourchette 0,9–1,8 M) | A1 : 1 040 000 |

Calendrier retenu : M1 380 k · M2 700 k · M3 150 k · M4 50 k (installation des glacières et présentoirs dans les hôtels avant le pilote). Pas de véhicule, pas de machine (seuil de bascule A1 : ≈ 650 cocos/mois durables, atteint en **juillet 2027** dans le réaliste accueil : la décision machine se pose **plus tôt** que pour les excursions, à instruire par `process-engineer`).

### 3.2 Coûts fixes mensuels (XPF/mois)

| Poste | A1 (A manuel) | A-accueil | Source |
|---|---|---|---|
| Local de préparation et stockage froid | 40 000 | 40 000 | [supposé : 0 si prêté – 80 000] |
| Électricité, eau | 8 000 | 8 000 | [estimé] |
| Consommables hygiène, téléphone, petit matériel | 12 000 | 12 000 | [estimé] |
| Comptable | 15 000 | 15 000 | [estimé] |
| **Relais de livraison 7/7** : livreur à la tâche 2 jours/semaine (week-end, congés), ≈ 8 tournées × 2 500 | — | **20 000** | [estimé] ; à partir de M5. Si l'hôtel refuse le tampon et que les livraisons se calent sur les arrivées de nuit (20 h–1 h, 4 h–6 h) : majoration ≈ 1 000/tournée de nuit, soit +10 000/mois, ou coût du temps de nuit du fondateur non chiffré (le **froid tampon évite les livraisons de nuit** : c'est son premier intérêt) |
| **Total** | **75 000** | **95 000** (75 000 M2–M4) | |
| Rémunération du fondateur | 0 | 0 | Coût d'opportunité en sensibilité (§ 5.5), comme en A1 |

**Point mort mensuel** (fixes ÷ marge unitaire) : à 700 XPF, **95 000 ÷ 335 ≈ 285 cocos/mois (≈ 10/jour)** ; avec 25 % Moorea en fret payant, marge moyenne 320 → ≈ 300. À 600 XPF : ≈ 405. À 500 XPF : ≈ 705 (A1 : 500). Atteint en **mai 2027 (M7)** dans le réaliste, contre juin 2027 (M8) en A1. Avec un découpeur salarié 52 h (75 400 de fixes en plus, variable −100 → marge 435) : point mort ≈ 390 cocos/mois, plus haut et plus fragile en basse saison.

---

## 4. Compte de résultat et trésorerie mensuels, scénario réaliste accueil

En **k XPF**. Prix 700 partout ; variables 365 (Tahiti) et 425 (Moorea, fret payant) ; encaissement à 30 jours (colonne de droite : à 60 jours) ; variables, fixes et CAPEX payés le mois même ; échantillons de M4 = 25 k ; apport du fondateur 2 000 k au mois 1.

| Mois | Cocos | CA | Variables | Marge brute | Fixes + échant. | EBITDA | CAPEX | Encaiss. | Décaiss. | Flux du mois | Cumul sans apport | Tréso avec apport 2 000 | Cumul si paiement à 60 j |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| M1 nov-26 | 0 | 0 | 0 | 0 | 25 | −25 | 380 | 0 | 405 | −405 | −405 | 1 595 | −405 |
| M2 déc-26 | 0 | 0 | 0 | 0 | 75 | −75 | 700 | 0 | 775 | −775 | −1 180 | 820 | −1 180 |
| M3 jan-27 | 0 | 0 | 0 | 0 | 75 | −75 | 150 | 0 | 225 | −225 | −1 405 | 595 | −1 405 |
| M4 fév-27 | 0 | 0 | 0 | 0 | 100 | −100 | 50 | 0 | 150 | −150 | −1 555 | 445 | −1 555 |
| M5 mar-27 | 140 | 98 | 51,1 | 46,9 | 95 | −48,1 | 0 | 0 | 146,1 | −146,1 | −1 701,1 | 299 | −1 701,1 |
| M6 avr-27 | 240 | 168 | 87,6 | 80,4 | 95 | −14,6 | 0 | 98 | 182,6 | −84,6 | −1 785,7 | 214 | −1 883,7 |
| M7 mai-27 | 400 | 280 | 146 | 134 | 95 | +39 | 0 | 168 | 241 | −73 | −1 858,7 | 141 | −2 026,7 |
| **M8 juin-27** | 550 | 385 | 200,8 | 184,2 | 95 | +89,2 | 0 | 280 | 295,8 | −15,8 | **−1 874,5 (point bas)** | **126** | −2 154,5 |
| M9 juil-27 | 780 | 546 | 284,7 | 261,3 | 95 | +166,3 | 0 | 385 | 379,7 | +5,3 | −1 869,2 | 131 | −2 254,2 |
| M10 août-27 | 1 020 | 714 | 384,5 | 329,5 | 95 | +234,5 | 0 | 546 | 479,5 | +66,5 | −1 802,7 | 197 | **−2 348,7 (point bas 60 j)** |
| M11 sep-27 | 1 080 | 756 | 407,2 | 348,8 | 95 | +253,8 | 0 | 714 | 502,2 | +211,8 | −1 590,9 | 409 | −2 304,9 |
| M12 oct-27 | 1 070 | 749 | 403,4 | 345,6 | 95 | +250,6 | 0 | 756 | 498,4 | +257,6 | −1 333,3 | 667 | −2 089,3 |
| **Total** | **5 280** | **3 696** | **1 965,3** | **1 730,7** | **1 035** | **+695,7** | **1 280** | **2 947** | **4 280,3** | **−1 333,3** | | | |

Notes : variables = 365 × cocos Tahiti + 425 × cocos Moorea (204 / 216 / 214 en M10–M12). Créances en fin de M12 : 749 k (1 505 k à 60 jours). Amortissement ≈ 12 k/mois à partir de M2 (≈ 700 k de matériel sur 5 ans) : résultat comptable année 1 ≈ **+0,2 à +0,6 M** selon que les frais de lancement (création, assurance, tests, formation ≈ 350 k) sont passés en charges ou immobilisés. Fiscalité non modélisée.

Lecture : l'exploitation passe au-dessus du point mort en **mai 2027 (M7)** et l'EBITDA de l'année 1 est **positif (+0,7 M)**, contre −0,23 M pour les excursions. Mais le point bas de trésorerie est **plus profond** qu'en A1 (**−1,87 M en juin 2027** contre −1,78 M) : CAPEX +240 k et fixes +20 k/mois sont décaissés avant que le prix de 700 ne produise ses effets. **Avec 2 M d'apport, il reste 126 k au point bas : insuffisant.** Si les agences paient à **60 jours**, le point bas descend à **−2,35 M en août 2027** et 2 M d'apport ne suffisent plus (découvert de 350 k). En contrepartie, la remontée est rapide : −1,33 M fin octobre 2027 contre −1,62 M en A1.

### 4.1 Totaux des trois scénarios accueil (année 1, k XPF)

| | Minimal | **Réaliste** | Optimiste |
|---|---|---|---|
| Cocos | 1 950 | **5 280** | 13 490 |
| CA | 1 365 | **3 696** | 9 443 |
| Coûts variables | 712 | **1 965** | 5 057 |
| Marge brute | 653 | **1 731** | 4 386 |
| Fixes + échantillons | 1 035 | **1 035** | 1 435 (livreur et local plus grand dès M9 : +100 k/mois) |
| **EBITDA année 1** | **−382** | **+696** | **+2 951** |
| CAPEX | 1 280 | **1 280** | 1 630 (2e réfrigérateur en M8, glacières et présentoirs supplémentaires) |
| Créances en fin de M12 (30 j) | 193 | **749** | 1 904 |
| Cumul de trésorerie fin M12 | −1 854 | **−1 333** | −583 |
| **Point bas de trésorerie (30 j)** | **−1 906 en M9**, puis stagnation vers −1 850 et rechute en février–mars 2028 | **−1 874 en M8** | **−2 500 en M9** |
| Reste avec 2 000 d'apport au point bas | 94 | 126 | **−500 : découvert** |

Même enseignement qu'A1, accentué : le minimal (une agence qui n'équipe qu'un quart de ses passagers) reste **sous le point mort** (250 contre 285 cocos/mois) et doit déclencher un pivot ; le réaliste tient si le fondateur dispose de **≈ 2,5 M (30 jours) ou ≈ 3,1 M (60 jours)**, ou d'un préfinancement d'agence ; l'optimiste **ne tient pas sans financement de croissance** (créances d'un mois à 2 500 cocos ≈ 1,75 M) ni sans machine et équipe.

### 4.2 Besoin de fonds, scénario réaliste (k XPF)

| Variante | CAPEX | Point bas | Mois | Fonds disponibles recommandés (+30 %) |
|---|---|---|---|---|
| A-accueil, paiement à 30 jours | 1 280 | ≈ −1 875 | M8 | **≈ 2 450** |
| A-accueil, paiement à 60 jours | 1 280 | ≈ −2 350 | M10 | **≈ 3 050**, ou 2 450 + acompte d'agence d'un mois de livraisons (≈ 0,5–0,7 M en haute saison) |
| A-accueil, l'hôtel prête le froid et l'agence transporte vers Moorea | 1 200 | ≈ −1 780 | M8 | ≈ 2 300 |
| A1, A-excursions (rappel) | 1 040 | ≈ −1 780 | M9 | ≈ 2 300 |

---

## 5. VAN, TRI, retour : A-accueil contre A-excursions et option combinée

### 5.1 Méthode et régime d'année 2

Méthode A1 § 5.1 inchangée (F0 = −CAPEX ; F1 = EBITDA année 1 − CAPEX supplémentaire − Δcréances ; F2 = EBITDA année 2 − renouvellement − Δcréances + récupération des créances ; VAN = F0 + F1 ÷ (1 + r) + F2 ÷ (1 + r)² ; valeur résiduelle nulle ; fondateur non rémunéré ; 12 % [supposé]).

Régime réaliste accueil, année 2 : 12 000 cocos (9 000 Tahiti + 3 000 Moorea fret payant), main-d'œuvre 80 → variable Tahiti 342,5 et Moorea 402,5, marge moyenne **342,5** ; fixes 95 k × 12 = 1 140 ; **EBITDA année 2 ≈ 2 970 k** (à 600 XPF : 1 770 ; à 500 XPF : 570, soit le niveau d'A1). Créances en fin d'année 2 : 700 k (un mois de CA lissé).

Option « accueil + excursions en seconde cible à partir de M9 » : volumes d'excursions ajoutés **au prix et aux coûts d'A1** (500 XPF, variable 350, marge 150), M9 200 · M10 250 · M11 400 · M12 400 (1 250 en année 1), 2 opérateurs en année 2 (6 000 cocos, Tahiti seulement) ; CAPEX +30 k (glacières) ; fixes +10 k/mois (tournées) ; mêmes délais de paiement. Le volume total d'année 2 (18 000, ≈ 1 500/mois) **dépasse le seuil machine** et exige un découpeur à mi-temps ; la décision machine d'A1 § 5.5 se pose alors au printemps 2027.

### 5.2 Flux (k XPF, scénario réaliste)

| Option | F0 | F1 | F2 | Somme brute | Détail |
|---|---|---|---|---|---|
| **A-excursions** (A1) | −1 040 | −575 | +890 | −725 | A1 § 5.2 |
| **A-accueil** | −1 280 | **−53** | **+3 669** | +2 336 | F1 = 696 EBITDA − 749 créances ; F2 = 2 970 − 50 renouvellement + 49 (créances 749 → 700) + 700 récupération |
| **A-accueil + excursions dès M9** | −1 310 | −106 | +4 649 | +3 233 | Excursions : F1 = 1 250 × 150 − 40 fixes − 200 créances = −52 ; F2 = 900 − 120 − 50 + 250 = +980 |

### 5.3 Résultats (scénario réaliste)

| Option | CAPEX | Point bas (30 j / 60 j) | VAN 8 % | **VAN 12 %** | VAN 20 % | TRI | Délai de retour |
|---|---|---|---|---|---|---|---|
| 0 — Ne rien faire | 0 | 0 | 0 | **0** | 0 | — | — |
| A-excursions (A1) | 1 040 | −1 776 / ≈ −2 100 | −809 | **−844** | −901 | négatif | > 24 mois (≈ 4–5 ans) |
| **A-accueil** | 1 280 | **−1 874 / −2 349** | **+1 816** | **+1 598** | **+1 224** | **≈ 67 %** | **≈ 18 mois** (avril 2028) |
| A-accueil + excursions dès M9 | 1 310 | ≈ −1 980 / ≈ −2 500 | +2 578 | **+2 302** | +1 830 | ≈ 84 % | ≈ 17 mois |

Exemple de recalcul (A-accueil, 12 %) : −1 280 − 53 × 0,8929 + 3 669 × 0,7972 = −1 280 − 47 + 2 925 = **+1 598**. TRI : 3 669 x² − 53 x − 1 280 = 0 → x ≈ 0,598 → r ≈ 67 % ; ce TRI élevé tient au regroupement des flux en fin d'année et à un CAPEX faible devant l'EBITDA d'année 2 ; le délai de retour (≈ 18 mois) est l'indicateur à retenir. L'option combinée ajoute ≈ +0,7 M de VAN parce que l'atelier, le froid et le découpeur sont déjà payés par l'accueil : les excursions deviennent rentables **en marge d'un flux régulier**, ce qu'elles n'étaient pas seules. L'agence réceptive vend elle-même des excursions à ses clients : elle peut prescrire NĪĀ à ses opérateurs (levier à documenter dans A8).

### 5.4 VAN à 12 % selon le scénario de volume (k XPF)

| Option | Minimal | **Réaliste** | Optimiste |
|---|---|---|---|
| A-excursions (A1) | −1 943 | **−844** | +467 |
| **A-accueil** | **−1 787** | **+1 598** | **≈ +6 100** (avec 300 k/mois de fixes en année 2 : livreur, 2e découpeur, local ; ordre de grandeur, la structure de coûts n'est plus celle d'un pilote manuel) |

Flux accueil : minimal (−1 280 ; −575 ; +8), optimiste (−1 280 ; +697 ; +8 529).

### 5.5 Pont A1 → A-accueil et sensibilité

**Pont (k XPF, VAN à 12 %, approximations par le raccourci ΔVAN ≈ Δmarge × cocos actualisés ; cocos actualisés accueil = 5 280 × 0,8929 + 12 000 × 0,7972 ≈ 14 280, soit « 1 XPF de marge = 14,3 k de VAN » contre 12,5 k en A1).**

| Étape | Effet | VAN |
|---|---|---|
| A-excursions (A1, réaliste) | | −844 |
| Volume +21 % / +11 %, aux marges d'A1 | ≈ +220 | −624 |
| **Prix 500 → 700** | **≈ +2 830** | +2 206 |
| Présentation hôtelière 25 → 60 (÷ 0,88) | ≈ −570 | +1 636 |
| Perte 15 → 12 %, glace −5, transport −10 | ≈ +380 | +2 016 |
| CAPEX +240 k | −240 | +1 776 |
| Fixes +20 k/mois (relais 7/7), échantillons +5 | ≈ −340 | +1 436 |
| Main-d'œuvre 100 → 80 en année 2 | ≈ +220 | ≈ +1 650 (calcul direct : +1 598, écart d'arrondis) |

**Le canal ne change pas le coût de revient ; il change le prix.** Tout le gain tient à 200 XPF de prix par passager : s'il n'est pas obtenu, le canal accueil est **moins bon** que les excursions (présentation, CAPEX et fixes en plus). **Prix net d'équilibre (VAN = 0) : ≈ 590 XPF** (700 − 1 598 ÷ 14,3).

**Sensibilité (A-accueil, réaliste, VAN à 12 %, base +1 598 k).**

| Rang | Variable | Base | Bas | Haut | ΔVAN bas | ΔVAN haut | VAN bas | VAN haut |
|---|---|---|---|---|---|---|---|---|
| **1** | **Prix par passager accueilli** (±20 %) | 700 | 560 | 840 | **−2 000** | **+2 000** | **−400** | +3 600 |
| **1 ex.** | **Commission ou remise exigée par l'agence** (variable de canal) | 0 % | 10 % | 20 % | −1 000 | −2 000 | +600 | **−400** |
| **1 ex.** | **Un coco par dossier au lieu d'une par passager** (volume ÷ 2,3) | par passager | par dossier | — | ≈ −2 500 | — | **≈ −900** | — |
| 2 | Volume (toutes années, ±20 %) | 5 280 / 12 000 | −20 % | +20 % | −950 | +950 | +650 | +2 550 |
| 3 | Présentation (variable de canal) | 60 | 35 | 120 | +410 | −970 | +2 010 | +630 |
| 4 | Prix d'achat de le coco (±20 %, ÷ 0,88) | 120 | 96 | 144 | +390 | −390 | +1 990 | +1 210 |
| 5 | Coûts fixes mensuels (±20 %) | 95 k | 76 k | 114 k | +320 | −320 | +1 920 | +1 280 |
| 6 | Main-d'œuvre (±20 %) | 100 / 80 | 80 / 64 | 120 / 96 | +280 | −280 | +1 880 | +1 320 |
| 7 | Taux de perte (±3 points) | 12 % | 9 % | 15 % | +160 | −170 | +1 760 | +1 430 |
| 8 | **Délai de paiement** (variable de canal) | 30 j | — | 60 j | — | −70 sur la VAN, mais **−475 k sur le point bas** (−2 349 au lieu de −1 874) | — | +1 530 |

Compléments hors ±20 % :

| Cas | Effet | VAN |
|---|---|---|
| A-accueil vendu **500 XPF** (prix cible d'A1) | −200 × 14,3 | **≈ −1 250** : pire qu'A-excursions (−844) |
| Pas de froid tampon à l'hôtel : livraisons calées sur les arrivées (nuit), découpe quasi quotidienne, +30 XPF de transport et +3 points de perte | ≈ −42 × 14,3 | ≈ +1 000 |
| Conservation réelle **< 5 jours** : le tampon hôtel ne tient plus, découpe et livraison quotidiennes, Moorea impossible | ≈ −50 XPF/coco et −25 % de volume Moorea | ≈ +600 ; sous 3 jours le canal n'est pas opérable 7/7 par un fondateur seul |
| Rémunérer le fondateur 150 k/mois chargé en année 2 | −1 800 × 0,7972 = −1 435 | **+165 : reste positif**, contrairement à toutes les options d'A1 |
| Local prêté (0 au lieu de 40 k/mois) | +40 k × 16,7 mois actualisés | ≈ +2 270 |
| Moorea « l'agence transporte » (0 au lieu de +60 sur 3 634 cocos Moorea actualisées ≈ 2 900) | +60 × 2,9 | ≈ +1 770 |
| Prix Moorea 760 (fret refacturé) | idem | ≈ +1 770 |

Les trois variables qui décident sont **toutes du côté de l'agence** : le prix net (prix affiché moins commission), la règle « par passager ou par dossier », et le délai de paiement (pour le besoin de fonds, pas pour la VAN). Elles sortent du premier entretien (§ 7), avant tout relevé de terrain sur le coco.

---

## 6. Ce que le canal change pour le financement

| Question | Réponse [supposé / estimé], à vérifier auprès des banques locales (Socredo, Banque de Tahiti, Banque de Polynésie), de l'ADIE et de la DGAE | Effet chiffré |
|---|---|---|
| Un contrat d'agence avec volume annuel est-il « bancable » ? | **Partiellement.** Un contrat signé de 12 mois (ex. 10 000 cocos × 700 = 7 M XPF de CA, même sans volume garanti) est la **meilleure pièce** d'un dossier de prêt création ou de microcrédit ADIE (A1 § 7) : il transforme un projet en carnet de commandes. Il ne suffit pas seul à une banque pour un créateur sans historique ; attendre un prêt sur contrat à l'ouverture est irréaliste | Améliore l'accès au microcrédit (≈ 1 M, 7–9 %) et au prêt machine en 2027–2028 |
| Préfinancement par l'agence | **Le plus réaliste et le plus rapide** : acompte d'un mois de livraisons ou paiement à réception pendant 6 mois contre une remise de 5 % ou une exclusivité d'accueil de 12 mois | Acompte ≈ 0,3–0,7 M selon la saison ; une remise de 5 % coûte ≈ 500 k de VAN (−35 × 14,3) : **moins cher qu'un découvert** et que le risque de rupture de trésorerie en août 2027 |
| Affacturage ou cession de créances (Dailly) | Offres bancaires locales [supposé] réservées aux entreprises établies, souvent au-dessus de 10–20 M de CA ; coût 1,5–3 % du montant cédé + taux. **Pas au lancement** ; possible en année 2 si une seconde agence signe | À 60 jours de paiement, céder les créances ramènerait le point bas de −2,35 à ≈ −1,9 M pour ≈ 100–150 k/an de frais |
| Délai de paiement | Négocier **30 jours** ou acompte ; sinon prévoir +0,5 M de fonds (§ 4.2) | Un passage de 30 à 60 jours vaut −475 k sur le point bas et −70 k seulement sur la VAN |
| Commission ou remise | Clarifier le modèle en entretien : l'agence **refacture** NĪĀ au tour-opérateur (sa marge est son affaire, prix NĪĀ intact) ou l'**absorbe** dans son transfert (elle demandera une remise). À 20 % de remise sur 700, la VAN s'annule | −1 000 k par tranche de 10 % |
| Dépendance à un gros compte | Année 1 réaliste : **l'agence 1 pèse 80–100 % du CA jusqu'en août 2027, ≈ 70 % en année 2**. Un désengagement ramène au scénario minimal (VAN −1,8 M). Parades : contrat 12 mois avec préavis de 3 mois et volume indicatif mensuel ; deuxième agence et un hôtel en direct avant octobre 2027 ; excursions en seconde cible dès M9 (§ 5.3) ; règle : **aucun client au-dessus de 50 % du CA après M18** | Le scénario combiné ramène la part de l'agence 1 à ≈ 50 % en année 2 |
| Ce que voit un sponsor | Un contrat d'agence et un hôtel partenaire sont une **preuve de traction** plus lisible pour le palier 2 (CHR) que trois opérateurs de lagon : l'hôtel qui sert NĪĀ à l'accueil est le premier compte CHR du palier 2 | Non chiffré ; c'est l'argument de la finalité, pas de la VAN du palier 1 |

Montage suggéré pour A-accueil réaliste : **apport 2 M + préfinancement de l'agence 0,3–0,5 M (ou microcrédit 0,5 M)** pour disposer de ≈ 2,5 M à 30 jours ; si l'agence impose 60 jours, exiger l'acompte ou porter les fonds à ≈ 3 M.

---

## 7. Les 10 chiffres à relever, par impact (★ = doit sortir du premier entretien avec l'agence du fondateur)

| Rang | Chiffre | Impact sur la VAN ou le cash | Qui | Comment |
|---|---|---|---|---|
| **1 ★** | **Prix net accepté par passager accueilli** (600 / 700 / 900 dits à voix haute), et qui paie : l'agence l'absorbe, le refacture au tour-opérateur, ou le vend en option | ±2 000 k ; VAN = 0 à ≈ 590 net | fondateur + `market-scout` (A8) | Entretien : « que vous coûte aujourd'hui l'accueil d'un passager : lei, boisson, temps de l'agent ? » puis les trois niveaux |
| **2 ★** | **Commission ou remise** attendue (0 / 10 / 20 %), exclusivité, durée de contrat possible | −1 000 k par 10 % | fondateur | Même entretien |
| **3 ★** | **Passagers accueillis par jour et par mois** par l'agence en 2025–2026, part dont la première nuit est à Tahiti ou Moorea, les 5 hôtels principaux, part des transferts privés | ±950 k à ±20 % de volume | fondateur, puis A8 | Demander les statistiques d'arrivées de l'agence par mois et par hôtel |
| **4 ★** | **Un coco par passager, par adulte ou par dossier** ; enfants ; que fait-on des couples | −2 500 k si par dossier | fondateur | Entretien : comment est remis le lei aujourd'hui |
| **5 ★** | **Délai de paiement, mode de commande (J−1 ? hebdomadaire ?), qui réceptionne à l'hôtel, acompte possible** | −475 k de point bas à 60 j | fondateur | Entretien |
| **6 ★** | **Logistique Moorea et nuit** : l'agence peut-elle transporter les glacières dans ses transferts ; heures d'arrivée des vols accueillis ; les hôtels acceptent-ils un froid tampon NĪĀ | +60 XPF/coco Moorea (+≈ 1 770 k à 25 % Moorea) ; évite les livraisons de nuit (−40 XPF/coco) | fondateur, puis `operations-director` avec 2–3 hôtels | Entretien, puis visite des hôtels |
| 7 | **Prix d'achat de le coco nīā** au stade demandé, par 100, livrée (inchangé d'A1, toujours aucune source) | ±390 k | `supply-analyst` | 3 cocoteraies, devis écrit |
| 8 | **Durée de conservation réelle** après découpe au froid, avec 2–3 jours en réfrigérateur d'hôtel (DLC exigée ≥ 5 j, ≥ 6 j pour Moorea) | ≈ −600 k sous 5 j ; canal non opérable sous 3 j | `process-engineer` | Lot test (item 4) avec un passage en réfrigérateur ménager à 4–6 °C |
| 9 | **Coût de la présentation hôtelière** : devis étiquettes, fiches bilingues, pailles, support, par 1 000 | +410 k à 35, −970 k à 120 | `brand-director` + `operations-director` | 2 imprimeurs locaux, 1 fournisseur de pailles |
| 10 | **Temps de découpe + présentation** par coco et **disponibilité d'un découpeur** à la tâche puis à temps partiel 7/7 (prix, statut, remplaçant) | ±280 k ; décide du passage au salarié vers 600 cocos/mois | `process-engineer` + `operations-director` | Chronométrage sur le lot test ; 3 candidats |

Préalable inchangé d'A1 (rang 0) : conditions du fret agricole gratuit (Lexpol, DGAE), qui décident où l'on achète et où l'on découpe. Les six chiffres ★ coûtent un entretien de deux heures et pèsent plus sur la décision que tous les relevés de terrain réunis : **le faire avant le lot test**.

---

## 8. Ce que ce scénario dit au business case

1. **VAN** : le canal accueil passe la VAN à 12 % de −0,84 M (excursions) à **≈ +1,6 M** au scénario réaliste, +2,3 M avec les excursions en seconde cible dès juillet 2027 ; le gain vient à 100 % du **prix par passager (700 contre 500)**, pas du coût de revient (365 contre 350), ni du volume (+10–20 %).
2. **Point mort** : ≈ 285 cocos/mois (10/jour) au lieu de 500, atteint en mai 2027 au lieu de juin ; l'EBITDA de l'année 1 devient positif (+0,7 M au lieu de −0,2 M) et le palier 1 peut, en année 2, rémunérer un mi-temps du fondateur en restant positif, ce qu'aucune option d'A1 ne permettait.
3. **Point bas** : il **s'aggrave** (−1,87 M en juin 2027 au lieu de −1,78 M ; −2,35 M si les agences paient à 60 jours) : il faut **≈ 2,5 M à 30 jours, ≈ 3 M à 60 jours**, ou un acompte d'agence ; 2 M d'apport ne suffisent pas.
4. **Régularité** : 7 jours sur 7 toute l'année avec un creux à 0,7 en février–mars au lieu d'une activité à 20–24 jours dépendante de la météo ; les fixes sont mieux absorbés, un découpeur à temps partiel devient possible dès juillet 2027 et la décision machine (650 cocos/mois) se pose plus tôt.
5. **Conditions** : prix net ≥ **590 XPF** après commission ; **un coco par passager** (par dossier, la VAN retombe à ≈ −0,9 M) ; froid tampon accepté par les hôtels et DLC ≥ 5 jours ; une deuxième agence ou un hôtel en direct avant octobre 2027 pour sortir de la dépendance à un seul compte.
6. **Retour** : ≈ 18 mois (avril 2028) au lieu de > 24 mois ; le palier 1 accueil **finance une machine de découpe en 2028** et une partie de la trésorerie du palier 2, ce que les excursions ne faisaient pas.
7. **Si le prix de 700 n'est pas obtenu** (500 accepté seulement), l'accueil est **moins bon** que les excursions (VAN ≈ −1,25 M) : présentation, CAPEX et fixes en plus pour la même marge.
8. **Finalité** : l'hôtel qui remet NĪĀ à l'arrivée est le premier compte CHR du palier 2 ; le canal sert la finalité mieux que le lagon, à condition de ne pas transformer NĪĀ en fournisseur de goodies d'accueil.

**Limites**

1. Aucun chiffre relevé ; les trois variables décisives (prix net, par passager ou par dossier, délai de paiement) sont des [supposé] qui tiennent à un entretien que le fondateur n'a pas encore eu.
2. La part de marché d'une agence réceptive (3 / 8 / 15 %) et la part « première nuit à Tahiti–Moorea » (60 %) sont posées sans source : A8 doit les remplacer.
3. Le coût de la présentation hôtelière (60, borne 120) et l'acceptation du froid tampon par les hôtels sont supposés ; sans tampon, le canal impose des livraisons de nuit non chiffrées en temps du fondateur.
4. Méthode d'A1 conservée (flux annuels, saisonnalité lissée en année 2, valeur résiduelle nulle, fiscalité et TVA non modélisées, fondateur non rémunéré sauf en sensibilité) ; le TRI de 67 % est un artefact du regroupement des flux, le délai de retour de 18 mois est l'indicateur à retenir.
5. La dépendance à un seul compte n'est pas probabilisée : si l'agence se retire, le scénario est le minimal (VAN −1,8 M), pas le réaliste.
