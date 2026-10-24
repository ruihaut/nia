# Annexe A1 — Modèle financier du palier 1 (diamond cut aux opérateurs d'excursion)

> Statut : v0, estimations de bureau, **aucun chiffre relevé sur le terrain**. Rédigé le 2026-10-23 par `financial-modeler` pour `business-director` (item 6 du backlog). Monnaie : XPF, montants hors TVA. Horizon : 12 mois de pilote (novembre 2026 → octobre 2027) + 12 mois de régime pour la VAN. Le palier 2 est hors chiffrage.
>
> Étiquettes : **[relevé]** mesuré sur le terrain (aucun ici) · **[estimé : …]** déduit d'un raisonnement ou d'un ordre de grandeur connu de la Polynésie française · **[estimé : source web]** chiffre public trouvé par le DG, URL donnée, non vérifié sur le terrain · **[supposé]** hypothèse de travail à vérifier. Les fourchettes importent plus que la valeur centrale.

## 0. Réponses aux décisions du business case (lecture en 2 minutes)

| Décision | Réponse du modèle (scénario réaliste, variante A « manuel ») | Confiance |
|---|---|---|
| Coût de revient d'un diamond cut livré à Tahiti | **≈ 350 XPF** en coûts variables (fourchette 250–500) ; ≈ 430 XPF en coût complet à 900 cocos/mois | Faible : 6 hypothèses sur 7 sont [estimé] ou [supposé] |
| Prix plancher / prix cible à l'opérateur | Plancher **400 XPF** (couvre le variable et une part des fixes) ; cible **500 XPF** (fourchette 450–600) ; Moorea +60 à +100 XPF | Faible : à relever par `market-scout` |
| Marge unitaire | **150 XPF/coco à Tahiti (30 %)**, 90 XPF à Moorea au même prix | — |
| Point mort mensuel (variante A) | **≈ 500 cocos/mois (≈ 23/jour)** pour couvrir 75 000 XPF de fixes ; atteint au mois 8 (juin 2027) dans le scénario réaliste | Moyenne |
| Investissement initial | **A manuel ≈ 1,04 M XPF** ; **B avec machine ≈ 2,0 M XPF** ; C sous-traitance ≈ 0,93 M XPF. Toutes dans l'enveloppe 2–5 M en CAPEX seul | Moyenne |
| Besoin de trésorerie maximal (CAPEX + pertes + créances) | **A ≈ 1,8 M XPF** (point bas en juillet 2027) ; B ≈ 2,65 M ; C ≈ 1,65 M. Scénario optimiste A : ≈ 2,1 M (la croissance consomme du cash). **Recommandation : 2,3–2,5 M disponibles pour A**, 3,2 M pour B | Moyenne |
| Le palier 1 finance-t-il les machines ? | **Non aux volumes réalistes** : ≈ 0,6 M XPF/an d'excédent en année 2, soit une machine de découpe en 2 ans, pas la ligne du palier 2. **Oui en optimiste** (≈ 2 M/an). | — |
| Machine de découpe : acheter quand ? | **Pas au lancement.** Seuil de bascule ≈ **650 cocos/mois durables (≈ 30/jour)**. Décider en juillet–août 2027 sur volumes observés | Moyenne |
| VAN à 12 % sur 24 mois, scénario réaliste | **A −0,84 M · B −1,05 M · C −0,89 M · option 0 : 0.** Le palier 1 seul ne se rembourse pas en 24 mois ; il s'équilibre (VAN = 0) à un prix de vente ≈ 570 XPF ou à +50 % de volume | — |
| Fret inter-îles | Deux variantes : **payant** ≈ 60 XPF/coco [estimé] ou **gratuit « produits agricoles »** ≈ 20 XPF/coco [supposé, à vérifier Lexpol]. Le dispositif connu (arrêté n° 1586 CM) couvre les produits **non transformés**, dans le sens **îles → Tahiti** : il ne couvre probablement pas une coco découpée à Tahiti et expédiée à Moorea, mais ouvre une **opportunité d'achat de cocos brutes dans une île productrice** (§ 1.5) | Faible : préalable à vérifier |
| Les 3 chiffres qui décident | 1) prix accepté par l'opérateur, 2) prix d'achat de la coco nīā (aucune source, même web), 3) volume (passagers/jour × opérateurs). Puis main-d'œuvre et durée de conservation. Préalable hors sensibilité : les conditions du fret agricole gratuit | — |

**Lecture.** Pris isolément, le palier 1 est un petit projet à marge mince qui couvre ses frais à partir d'une vingtaine de cocos par jour et rend quelques dizaines de milliers de XPF par mois ; il ne rémunère pas le fondateur et ne finance pas le palier 2. Sa valeur est ailleurs : apprentissage de la filière, laboratoire de marque, premiers clients, qualification des chiffres qui manquent ici. C'est l'option « continuer » (palier 2), hors de ce chiffrage, qui justifie ou non la mise de 1,8 à 2,5 M XPF. Le signaler est le rôle de cette annexe : si le palier 1 devenait une fin en soi, ces chiffres disent qu'il ne vaut pas la peine.

---

## 1. Hypothèses unitaires et coût de revient

### 1.1 Postes variables par coco (XPF)

| Poste | Bas | **Central** | Haut | Source et raisonnement |
|---|---|---|---|---|
| Achat coco nīā à la cocoteraie, récoltée au stade demandé | 80 | **120** | 160 | [estimé : coco à boire 150–250 XPF au bord de route ou au marché de Papeete ; prix producteur en gros ≈ 50–60 % de ce prix ; + prime de sélection du stade nīā et de récolte sur commande] |
| Main-d'œuvre : contrôle à réception, découpe diamond cut, nettoyage, filmage, mise au froid | 60 | **100** | 150 | [estimé : 2,5–4 min/coco toutes opérations, central 3 min = 20 cocos/h ; découpeur **à la tâche** facturé ≈ 2 000 XPF/h ou 100 XPF/coco ; en **temps partiel salarié**, SMIG retenu 1 050–1 100 XPF/h brut en 2026 + charges patronales CPS ≈ 30–35 % ≈ 1 400–1 500 XPF/h chargé → 75 XPF/coco. Le central retient la tâche : pas d'engagement tant que le volume ne remplit pas un poste]. SMIG [estimé : source web] : 964,34 XPF brut/h au 01/10/2022 (arrêté n° 1931 CM du 21/09/2022, https://www.service-public.pf/trav/wp-content/uploads/sites/23/2022/10/Arrete-n°-1931-CM-du-21_09_2022-SMIG-oct-22.pdf) ; **1 024,74 XPF brut/h au 01/05/2024, soit 173 182 XPF/mois pour 169 h** (arrêté n° 580 CM du 30/04/2024, https://www.service-public.pf/trav/wp-content/uploads/sites/23/2024/05/Arrete-n°-580-CM-du-30_04_2024.pdf) ; relevé à nouveau en mai 2025, montant non lu (https://www.service-public.pf/trav/wp-content/uploads/sites/23/2025/05/FPCG-SMIG-2025-05.pdf) |
| Glace pour le transport | 10 | **20** | 35 | [estimé : sac de glace 5 kg ≈ 500 XPF pour une livraison de 25–40 cocos] |
| Marquage NĪĀ minimal : film alimentaire, étiquette DLC, bandeau ou tampon | 10 | **25** | 50 | [supposé : dépend du choix de `brand-director` ; un bandeau imprimé localement coûte vite 50 XPF] |
| Transport Tahiti : tournée en véhicule du fondateur | 15 | **40** | 60 | [estimé : tournée de 40 km, essence ≈ 150 XPF/L → 600 XPF + usure ≈ 1 000 XPF ≈ 1 600 XPF pour 40 cocos] |
| **Supplément Moorea, variante « fret payant »** : bac sur ferry Aremiti/Terevau + remise au quai de Vaiare | 40 | **60** | 120 | [estimé : passager ≈ 1 500 XPF l'aller, colis/bac fret ≈ 1 500–3 000 XPF le trajet, pour un bac de 40 cocos ; glace supplémentaire ; aucune grille tarifaire fret publique trouvée, devis à demander. Suppose que l'opérateur vient chercher au quai]. **Variante retenue dans le modèle** (prudente) |
| **Supplément Moorea, variante « fret gratuit produits agricoles »** : seuls restent la glace, le passage au port et la manutention | 10 | **20** | 40 | [supposé, à vérifier Lexpol : prise en charge du fret maritime par le Pays, cf. § 1.5 ; elle ne couvre probablement **ni le sens Tahiti → Moorea ni une coco découpée**] |
| Perte : cocos hors stade à réception, casse à la découpe, invendus (DLC dépassée) | 8 % | **15 %** | 25 % | [supposé : sans mesure. Les invendus dépendent directement de la durée de conservation, cf. § 6] |
| Électricité du réfrigérateur | — | (fixe) | — | [estimé : armoire pro 3–4 kWh/jour × ≈ 40 XPF/kWh ≈ 5 000 XPF/mois, comptée dans les fixes pour ne pas la compter deux fois] |

### 1.2 Coût de revient d'un diamond cut livré (central)

Formule : (achat + main-d'œuvre + glace + marquage) ÷ (1 − perte) + transport. La perte s'applique aux coûts engagés sur des cocos qui ne seront pas facturées.

| Étape | Variante A manuel | Variante B machine | Variante C découpe à la cocoteraie |
|---|---|---|---|
| Achat coco | 120 | 120 | 220 (coco **déjà découpée** par la cocoteraie : 120 + ≈ 70 de main-d'œuvre locale + ≈ 30 de marge) [supposé] |
| Main-d'œuvre NĪĀ | 100 | 40 (≈ 1 min : machine 10–20 s + manutention) | 30 (contrôle, filmage, marquage ≈ 1 min) |
| Glace | 20 | 20 | 20 |
| Marquage | 25 | 25 | 25 |
| Sous-total avant perte | 265 | 205 | 295 |
| Taux de perte | 15 % | 12 % (coupe régulière, moins de casse) [supposé] | 10 % (la cocoteraie ne livre que les conformes) [supposé] |
| Sous-total après perte | 312 | 233 | 328 |
| Transport Tahiti | 40 | 40 | 40 |
| **Coût variable Tahiti** | **≈ 350** | **≈ 275** | **≈ 370** |
| **Coût variable Moorea** (+60) | **≈ 410** | ≈ 335 | ≈ 430 |
| Fixes alloués à 900 cocos/mois (régime réaliste) | +83 | +94 | +78 |
| Fixes alloués à 545 cocos/mois (moyenne du pilote M5–M12) | +138 | +156 | +128 |
| **Coût complet Tahiti, régime** | **≈ 430** | ≈ 370 | ≈ 450 |

Fourchette du coût variable Tahiti, variante A : **≈ 250 XPF** (tout en bas) à **≈ 500 XPF** (tout en haut). La valeur centrale est au milieu d'une incertitude de ±40 %.

### 1.3 Prix de vente cible et marge

Le client ne revend pas la coco : il la sert, incluse dans une excursion vendue 8 000–15 000 XPF par passager [estimé]. Le prix NĪĀ se compare donc à **son coût actuel par passager**.

| Coût actuel de l'opérateur par coco servie | Estimation |
|---|---|
| Coco achetée au bord de route, au marché ou à un producteur | 150–250 [estimé] |
| Ouverture par le guide ou un équipier (2–3 min à ≈ 1 500 XPF/h chargé) | 50–75 [estimé] |
| Perte (stade raté, casse, cocos jetées) | 10–15 % [supposé] |
| **Total actuel** | **≈ 230–370 XPF** |

| Niveau de prix NĪĀ (HT, livré) | Tahiti | Moorea | Lecture |
|---|---|---|---|
| **Plancher** (couvre le variable + ≈ 50 XPF de fixes) | **400** | 460 | En dessous, on perd de l'argent à chaque coco |
| **Cible** | **500** | 560–600 | +35 à +115 % par rapport au coût actuel de l'opérateur ; justifié par stade garanti, froid, prêt à servir, zéro manipulation à bord, DLC, marque. ≈ 4–6 % du prix de l'excursion |
| Haut | 600 | 700 | Opérateurs premium (petits groupes, lagon privé). À tester |

| Marge unitaire (variante A, prix 500) | Tahiti | Moorea à 500 | Moorea à 560 |
|---|---|---|---|
| Prix | 500 | 500 | 560 |
| Coût variable | 350 | 410 | 410 |
| **Marge sur coût variable** | **150 (30 %)** | 90 (18 %) | 150 (27 %) |

**Marge par livraison type** (40 cocos, Tahiti, variante A) : CA 20 000 XPF, coûts variables 14 000 XPF, **marge 6 000 XPF**. Une tournée Tahiti doit grouper au moins 25–30 cocos pour que le transport ne mange pas la marge. À Moorea au même prix : 3 600 XPF par livraison ; **facturer le supplément inter-îles** est nécessaire.

TVA : taux de Polynésie française 5 % / 13 % / 16 % ; le taux applicable à une coco fraîche découpée est [supposé] 5 % (produit alimentaire), à vérifier par `operations-director` (item 5). Neutre en trésorerie si l'entreprise est assujettie ; non modélisée.

### 1.4 Coûts fixes mensuels (XPF/mois)

| Poste | A manuel | B machine | C cocoteraie | Source |
|---|---|---|---|---|
| Local de préparation et de stockage froid (dépendance, garage aménagé, espace chez la cocoteraie) | 40 000 | 40 000 | 40 000 | [supposé : fourchette 0 si prêté – 80 000 si loué ; levier important] |
| Électricité (réfrigérateur) et eau | 8 000 | 13 000 | 8 000 | [estimé : ≈ 40 XPF/kWh] |
| Consommables hygiène, téléphone, petit matériel | 12 000 | 12 000 | 7 000 | [estimé] |
| Comptable / tenue des obligations | 15 000 | 15 000 | 15 000 | [estimé : forfait TPE] |
| Entretien machine, lames | — | 5 000 | — | [supposé] |
| **Total** | **75 000** | **85 000** | **70 000** | |
| Rémunération du fondateur | **0** | 0 | 0 | Décision de modélisation : le fondateur n'est pas rémunéré pendant le pilote ; c'est un **coût d'opportunité** chiffré à l'option 0 (§ 5) et en sensibilité (§ 6) |

**Point mort mensuel** = fixes ÷ marge unitaire : A 75 000 ÷ 150 = **500 cocos/mois** (≈ 23/jour sur 22 jours) ; B 85 000 ÷ 225 = 378 ; C 70 000 ÷ 130 = 538. Avec 20 % de cocos Moorea à 500 XPF, la marge moyenne tombe à 138 et le point mort A monte à ≈ 545.

### 1.5 Fret inter-îles : deux variantes et une opportunité

**Ce que dit la réglementation** [estimé : source web, lu par le DG, non vérifié sur Lexpol ni auprès de la DGAE]. Arrêté n° 1586 CM du 13/09/2023, modifié par l'arrêté n° 586 CM du 07/05/2026 (note n° 6022 MEF-DGAE du 11/05/2026), en application de la délibération n° 95-118 AT du 24/08/1995 : le Pays prend en charge **100 % du fret maritime**, payé directement aux armateurs, pour les **produits agricoles non transformés**, l'artisanat et certains produits transformés listés au cas par cas en Conseil des ministres ; expéditions **des îles vers Tahiti ou entre îles** ; bénéficiaires : titulaires d'une carte CAPL valide, sociétés inscrites au RCS qui revendent, transforment ou utilisent ces produits, restauration collective. Sources : https://www.service-public.pf/dgae/aides/prise-en-charge-du-fret-maritime-par-le-pays/ et https://service-public.pf/dgae/wp-content/uploads/sites/44/2024/05/Arrete-n°-1586-CM-du-13_09_2023.pdf

| Flux | Variante « fret payant » [estimé] | Variante « fret gratuit produits agricoles » [supposé, à vérifier Lexpol] | Lecture |
|---|---|---|---|
| Cocos **découpées à Tahiti → opérateur à Moorea** (flux du modèle) | +60 XPF/coco | +20 XPF/coco **si** le sens Tahiti → Moorea et la coco parée sont éligibles | Deux doutes cumulés : le sens couvert est îles → Tahiti et entre îles ; une coco parée est probablement « transformée ». **Le modèle garde 60 XPF.** Si l'éligibilité agricole se perd à la découpe, **la découpe devrait se faire après le transport**, c'est-à-dire à Moorea (poste de découpe local ou cocoteraie partenaire de Moorea, option C sur place) |
| Cocos **brutes nīā d'une île productrice → atelier de Tahiti** (opportunité) | ≈ +40–75 XPF/coco de fret [estimé] | **0 XPF de fret** : produit agricole brut, sens îles → Tahiti, NĪĀ inscrite au RCS comme transformateur | Permet d'acheter là où la coco jeune est abondante et moins chère que sur Tahiti ; la coco non ouverte supporte plusieurs jours de transport sans froid [supposé] |

**Chiffrage.** Variante gratuite sur le flux Moorea du modèle : marge Moorea 130 au lieu de 90 XPF ; effet sur la VAN A réaliste ≈ +40 × 2 310 cocos Moorea actualisées ≈ **+90 k XPF** (VAN −754 au lieu de −844). Opportunité d'achat dans une île productrice [supposé] : prix d'achat 80 au lieu de 120 XPF, fret 0 → coût de revient −47 XPF/coco (÷ 0,85 de perte) → VAN ≈ **+590 k XPF** (−254) ; c'est le deuxième levier après le prix de vente, **si** la régularité et la qualité à réception tiennent sur un approvisionnement distant, et si la carte CAPL ou l'inscription RCS ouvre le droit. À instruire par `supply-analyst` avec l'item 2 (cartographie des sources : Tahiti, Moorea, Raiatea, Tuamotu).

---

## 2. Scénarios de volume

### 2.1 Hypothèses de marché

| Hypothèse | Valeur | Source |
|---|---|---|
| Passagers servis par opérateur et par jour d'activité | 8–20, central 12 | [estimé : lagon 10–20 pax, 4x4 8–16 pax ; 1 coco par passager] |
| Jours d'activité par mois | 20–24 | [estimé] |
| Cocos par opérateur et par mois en saison moyenne | ≈ 250–300 | 12 × 22 |
| Saisonnalité touristique (indice, moyenne = 1,0) | nov 0,9 · déc 1,0 · jan 0,9 · **fév 0,7 · mar 0,7** · avr 0,8 · mai 1,0 · juin 1,1 · **juil 1,3 · août 1,3** · sep 1,2 · oct 1,1 | [estimé : haute saison juin–octobre, creux février–mars, fêtes en décembre] |
| Délai de paiement des opérateurs | 30 jours | [supposé : petites structures, paiement à facture mensuelle] |

**Bornes de marché** [estimé : source web ISPF, bilan tourisme 2025, https://www.ispf.pf/content//uploads/1517_PC_Tourisme_2025_12_9e5f74a421.pdf] : 281 227 touristes en 2025 (+6,6 %), dont 227 286 en hébergement terrestre ; 70 062 excursionnistes de croisière ; 351 289 visiteurs au total ; Amérique du Nord 42 % ; chiffre d'affaires touristique 217 Mds XPF.

| Borne | Calcul | Résultat | Lecture des scénarios |
|---|---|---|---|
| Touristes susceptibles d'une excursion avec coco à Tahiti ou Moorea | 281 227 × 60 % passant par Tahiti–Moorea × 50 % faisant une excursion payante [supposé] | ≈ **85 000 cocos/an** de marché adressable, hors croisière | Minimal 3 600/an = 4 % ; **réaliste 10 800/an = 13 %** ; optimiste 24 000/an = 28 % du marché adressable en année 2 |
| Croisiéristes (escales Papeete et Moorea, excursions groupées) | 70 062 × 50 % en excursion [supposé] | ≈ 35 000 cocos/an, mais par pics de 500–2 000 passagers par escale | Hors scénarios : volumes trop irréguliers pour le pilote ; opportunité pour l'année 2 si la conservation ≥ 10 jours permet de constituer un stock |
| Touristes présents en moyenne un jour donné | 281 227 × séjour ≈ 15 jours ÷ 365 [supposé] | ≈ 11 500 personnes | Le réaliste (≈ 40 cocos/jour en haute saison) touche < 1 % des touristes présents : le marché n'est pas la contrainte, **l'accès aux opérateurs et le prix le sont** |

### 2.2 Calendrier et montée en charge (cocos facturées par mois)

Mois 1 = novembre 2026. Mois 1–3 : préparation (cocoteraie partenaire, protocole de découpe, test de conservation, réglementaire). Mois 4 : échantillons gratuits et dégustations (≈ 60 cocos). **Mois 5 (mars 2027) : premières livraisons payantes**, soit dans les 6 mois.

| Mois | Minimal (1 opérateur, 6–10/jour, Tahiti) | **Réaliste** (1 → 3 opérateurs, dont 1 Moorea en M12) | Optimiste (2 → 6 opérateurs, dont 2 Moorea) |
|---|---|---|---|
| M1 nov-26 | 0 | 0 | 0 |
| M2 déc-26 | 0 | 0 | 0 |
| M3 jan-27 | 0 | 0 | 0 |
| M4 fév-27 | 0 (échantillons) | 0 (60 échantillons) | 0 (échantillons) |
| M5 mar-27 | 120 | **160** (1 op., 8/j, basse saison) | 300 |
| M6 avr-27 | 150 | **200** (1 op., 10/j) | 400 |
| M7 mai-27 | 180 | **400** (2 op.) | 700 |
| M8 juin-27 | 200 | **500** | 900 |
| M9 juil-27 | 250 | **800** (3 op., haute saison) | 1 400 |
| M10 août-27 | 250 | **850** | 1 500 |
| M11 sep-27 | 220 | **750** | 1 300 |
| M12 oct-27 | 200 | **700** (dont 150 Moorea) | 1 200 (dont 300 Moorea) |
| **Total année 1** | **1 570** | **4 360** | **7 700** (dont ≈ 1 000 Moorea) |

### 2.3 Régime (année 2, novembre 2027 → octobre 2028) pour la VAN

| | Minimal | **Réaliste** | Optimiste |
|---|---|---|---|
| Opérateurs | 2 (Tahiti) | **4 (3 Tahiti + 1 Moorea)** | 8 (6 Tahiti + 2 Moorea) |
| Cocos/mois (moyenne lissée) | 300 | **900** | 2 000 |
| Cocos/an | 3 600 | **10 800** | 24 000 |
| Part Moorea | 0 % | 20 % | 25 % |
| Fixes/mois (A) | 75 000 | 75 000 | 100 000 (local plus grand) |
| CAPEX de renouvellement année 2 | 50 000 | 50 000 | 50 000 |
| Créances clients en fin d'année 2 (1 mois de CA) | 150 000 | 450 000 | 1 000 000 |

Tout [supposé]. La saisonnalité est lissée en année 2 (on raisonne en annuel).

---

## 3. Investissement initial (CAPEX)

Montants en XPF, décaissés aux mois 1–3.

| Poste | A manuel | B avec machine d'occasion | C découpe à la cocoteraie | Source |
|---|---|---|---|---|
| Réfrigérateur professionnel d'occasion (armoire 600–1 400 L) | 250 000 | 250 000 | 250 000 | [estimé : neuf 400 000–700 000 rendu Tahiti, occasion ≈ 50 %. Une chambre froide d'occasion ≈ 600 000–1 200 000 : pas nécessaire au pilote] |
| Outils de découpe : couteaux et machettes pro, planches, affûtage, gants anti-coupure | 40 000 | 40 000 | — | [estimé] |
| Glacières (4–6 × 60–100 L) | 60 000 | 60 000 | 60 000 | [estimé : 10 000–15 000 pièce] |
| Table inox d'occasion, bacs alimentaires, évier | 80 000 | 80 000 | 40 000 | [estimé] |
| Petit matériel d'hygiène (thermomètres, blouses, désinfectant) | 30 000 | 30 000 | 30 000 | [estimé] |
| Matériel de marquage NĪĀ initial (tampon, étiquettes, bandeaux) | 50 000 | 50 000 | 50 000 | [supposé] |
| Véhicule | 0 (véhicule du fondateur, indemnisé dans le variable) | 0 | 0 | Un utilitaire d'occasion coûterait 800 000–1 500 000 [estimé] : exclu du pilote |
| Caution du local (2 mois) | 80 000 | 80 000 | 80 000 | [supposé] |
| Création d'entreprise (statuts, enregistrement, greffe, annonce, CCISM) | 100 000 | 100 000 | 100 000 | [estimé : 20 000 en patente simple, jusqu'à 150 000 en SARL avec conseil] |
| Assurance RC professionnelle, 1re année | 100 000 | 100 000 | 100 000 | [estimé : 60 000–120 000/an] |
| Tests de conservation : analyses microbiologiques d'un lot sur 3 semaines | 100 000 | 100 000 | 100 000 | [estimé : 6–8 analyses à 10 000–20 000] |
| Formation hygiène alimentaire (fondateur + découpeur) | 50 000 | 50 000 | 25 000 | [estimé] |
| **Machine de découpe de coco jeune** (type trimming machine asiatique, neuve d'entrée de gamme ou occasion importée), rendue et dédouanée | — | 800 000 | — | [estimé : 2 000–6 000 USD FOB soit 250 000–700 000 XPF ; fret, droits et TVA à l'import ≈ +40–60 % ; pas de marché de l'occasion en PF] |
| Pièces de rechange, lames, installation électrique | — | 150 000 | — | [supposé] |
| Imprévus ≈ 10 % | 100 000 | 100 000 | 95 000 | |
| **Total CAPEX** | **≈ 1 040 000** | **≈ 1 990 000** | **≈ 930 000** | |
| Fourchette | 0,7–1,5 M | 1,5–2,8 M | 0,6–1,4 M | |

Les trois variantes tiennent dans l'enveloppe de 2–5 M XPF **en CAPEX**. Mais le CAPEX n'est pas le besoin de financement : il faut y ajouter les pertes d'exploitation des premiers mois et les créances clients (§ 4). La variante B **dépasse un apport de 2 M XPF** dès que l'on ajoute ces éléments (besoin ≈ 2,65 M).

---

## 4. Compte de résultat et trésorerie mensuels, scénario réaliste, variante A

En **milliers de XPF (k XPF)**. Encaissements à 30 jours (le CA du mois M rentre en M+1) ; coûts variables, fixes et CAPEX payés le mois même ; apport du fondateur 2 000 k au mois 1 pour la colonne de droite.

| Mois | Cocos | CA | Variables | Marge brute | Fixes + échant. | EBITDA | CAPEX | Encaiss. | Décaiss. | Flux du mois | Cumul sans apport | Tréso avec apport 2 000 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| M1 nov-26 | 0 | 0 | 0 | 0 | 25 | −25 | 330 | 0 | 355 | −355 | −355 | 1 645 |
| M2 déc-26 | 0 | 0 | 0 | 0 | 75 | −75 | 560 | 0 | 635 | −635 | −990 | 1 010 |
| M3 jan-27 | 0 | 0 | 0 | 0 | 75 | −75 | 150 | 0 | 225 | −225 | −1 215 | 785 |
| M4 fév-27 | 0 | 0 | 0 | 0 | 95 | −95 | 0 | 0 | 95 | −95 | −1 310 | 690 |
| M5 mar-27 | 160 | 80 | 56 | 24 | 75 | −51 | 0 | 0 | 131 | −131 | −1 441 | 559 |
| M6 avr-27 | 200 | 100 | 70 | 30 | 75 | −45 | 0 | 80 | 145 | −65 | −1 506 | 494 |
| M7 mai-27 | 400 | 200 | 140 | 60 | 75 | −15 | 0 | 100 | 215 | −115 | −1 621 | 379 |
| M8 juin-27 | 500 | 250 | 175 | 75 | 75 | 0 | 0 | 200 | 250 | −50 | −1 671 | 329 |
| **M9 juil-27** | 800 | 400 | 280 | 120 | 75 | +45 | 0 | 250 | 355 | −105 | **−1 776 (point bas)** | **224** |
| M10 août-27 | 850 | 425 | 297,5 | 127,5 | 75 | +52,5 | 0 | 400 | 372,5 | +27,5 | −1 748,5 | 251,5 |
| M11 sep-27 | 750 | 375 | 262,5 | 112,5 | 75 | +37,5 | 0 | 425 | 337,5 | +87,5 | −1 661 | 339 |
| M12 oct-27 | 700 | 350 | 254 | 96 | 75 | +21 | 0 | 375 | 329 | +46 | −1 615 | 385 |
| **Total** | **4 360** | **2 180** | **1 535** | **645** | **870** | **−225** | **1 040** | **1 830** | **3 445** | **−1 615** | | |

Notes : variables = 350 × cocos (+ 60 × 150 cocos Moorea en M12) ; échantillons de M4 = 20 k ; fixes M1 = 25 k (pas encore de local). Amortissement du matériel ≈ 8 k/mois à partir de M2 (≈ 460 k sur 5 ans), soit un **résultat comptable année 1 ≈ −313 k**. 350 k de créances restent à encaisser en fin de M12. Fiscalité non modélisée (pertes en année 1).

Lecture : l'exploitation s'équilibre au mois 8 (juin 2027) et devient positive en haute saison. Le point bas de trésorerie tombe en **juillet 2027, à −1,78 M XPF**, au moment où le volume monte : les cocos de juillet sont payées aux fournisseurs en juillet, encaissées en août. **Avec 2 M d'apport, il reste 224 k de marge au point bas : trop peu.** Un impayé, une panne de réfrigérateur ou un mois de perte à 25 % et la trésorerie casse. D'où la recommandation de 2,3–2,5 M disponibles, ou d'une ligne complémentaire (§ 7).

### 4.1 Totaux des trois scénarios (année 1, variante A, k XPF)

| | Minimal | **Réaliste** | Optimiste |
|---|---|---|---|
| Cocos | 1 570 | **4 360** | 7 700 |
| CA | 785 | **2 180** | 3 850 |
| Coûts variables | 549,5 | **1 535** | 2 755 |
| Marge brute | 235,5 | **645** | 1 095 |
| Fixes + échantillons | 870 | **870** | 870 |
| **EBITDA année 1** | **−634,5** | **−225** | **+225** |
| CAPEX | 1 040 | **1 040** | 1 290 (2e réfrigérateur en M9) |
| Créances en fin de M12 | 100 | **350** | 600 |
| Cumul de trésorerie fin M12 | −1 774,5 | **−1 615** | −1 665 |
| **Point bas de trésorerie** | **−1 775 en M12, et ça continue de baisser (≈ −45 k/mois)** | **−1 776 en M9** | **−2 095 en M9** |
| Reste avec 2 000 d'apport au point bas | 225 | 224 | **−95 : découvert** |

Trois enseignements : le scénario minimal (un seul opérateur qui ne grossit pas) **n'est pas viable** et doit déclencher un arrêt ou un pivot avant la fin de 2027 ; le scénario réaliste tient de justesse ; le scénario optimiste **consomme plus de trésorerie** que le réaliste pendant la montée (créances et deuxième réfrigérateur) avant de rapporter beaucoup plus. La croissance se finance.

### 4.2 Point bas de trésorerie par variante (scénario réaliste, k XPF)

| Variante | CAPEX | Point bas | Mois | Recommandation de fonds disponibles (+30 %) |
|---|---|---|---|---|
| A manuel | 1 040 | ≈ −1 780 | M9 | **≈ 2 300** |
| B machine | 1 990 | ≈ −2 650 | M9 | ≈ 3 400 |
| C cocoteraie | 930 | ≈ −1 650 | M9 | ≈ 2 150 |

---

## 5. VAN, TRI et délai de retour par option (24 mois)

### 5.1 Méthode

Trois flux annuels, actualisation annuelle :

- **F0** (aujourd'hui) = − CAPEX initial.
- **F1** (fin de l'année 1) = EBITDA année 1 − CAPEX supplémentaire année 1 − variation des créances clients (ΔBFR).
- **F2** (fin de l'année 2) = EBITDA année 2 − CAPEX de renouvellement − variation des créances + **récupération des créances** en fin d'horizon (on encaisse ce qui est dû). Valeur résiduelle du matériel = 0 [supposé, prudent : un réfrigérateur et une machine revendables ajouteraient 0,1–0,3 M].

**VAN(r) = F0 + F1 ÷ (1 + r) + F2 ÷ (1 + r)².** Facteurs : à 8 % → 0,9259 et 0,8573 ; à 12 % → 0,8929 et 0,7972 ; à 20 % → 0,8333 et 0,6944.

**TRI** = r tel que VAN = 0. Avec trois flux, poser x = 1 ÷ (1 + r) et résoudre F2·x² + F1·x + F0 = 0 ; TRI = 1 ÷ x − 1. Si F0 + F1 + F2 < 0, le TRI est négatif (le projet ne rend pas sa mise sur l'horizon).

**Délai de retour** = mois où le cumul de trésorerie redevient ≥ 0.

Le taux de 12 % est [supposé] : il reflète un petit projet non coté, risqué, porté par un fondateur seul. Le regroupement des flux en fin d'année est une simplification (les pertes de l'année 1 sont en réalité décaissées plus tôt).

### 5.2 Détail des flux, scénario réaliste (k XPF)

| Option | Composition | F0 | F1 | F2 | Somme brute |
|---|---|---|---|---|---|
| **0 — Ne rien faire** | Aucun flux | 0 | 0 | 0 | 0 |
| **A — Palier 1 manuel** | F1 = −225 EBITDA − 350 créances ; F2 = 590 EBITDA (10 800 × 150 − 130 Moorea − 900 fixes) − 50 CAPEX − 100 Δcréances + 450 récupération | −1 040 | −575 | +890 | **−725** |
| **B — Palier 1 avec machine** | F1 = −8 EBITDA (4 360 × 225 − 9 − 980 fixes) − 350 ; F2 = 1 280 EBITDA (10 800 × 225 − 130 − 1 020) − 50 − 100 + 450 | −1 990 | −358 | +1 580 | **−768** |
| **C — Découpe sous-traitée à la cocoteraie** | F1 = −257 EBITDA (4 360 × 130 − 9 − 815 fixes) − 350 ; F2 = 434 EBITDA (10 800 × 130 − 130 − 840) − 50 − 100 + 450 | −930 | −607 | +734 | **−803** |

### 5.3 Résultats, scénario réaliste

| Option | VAN 8 % | **VAN 12 %** | VAN 20 % | TRI | Délai de retour |
|---|---|---|---|---|---|
| 0 — Ne rien faire | 0 | **0** | 0 | — | — |
| A — Manuel | −809 | **−844** | −901 | négatif | > 24 mois (≈ 4–5 ans au rythme de l'année 2 : ≈ 440 k/an) |
| B — Machine | −967 | **−1 050** | −1 191 | négatif | > 24 mois (≈ 37 mois) |
| C — Cocoteraie | −863 | **−887** | −926 | négatif | > 24 mois (≈ 5 ans) |

Exemple de recalcul (A, 12 %) : −1 040 − 575 × 0,8929 + 890 × 0,7972 = −1 040 − 513 + 710 = **−844**.

### 5.4 VAN à 12 % selon le scénario de volume (k XPF)

| Option | Minimal | **Réaliste** | Optimiste | TRI optimiste | Retour optimiste |
|---|---|---|---|---|---|
| 0 | 0 | **0** | 0 | — | — |
| A — Manuel | −1 943 | **−844** | **+467** | ≈ 31 % | ≈ 24 mois |
| B — Machine | −2 766 | **−1 050** | **+1 273** | ≈ 43 % | ≈ 20 mois |
| C — Cocoteraie | −1 821 | **−887** | +153 | ≈ 19 % | ≈ 26 mois |

Flux optimistes utilisés : A (−1 040 ; −625 ; +2 590), B (−1 990 ; −158 ; +4 270), C (−930 ; −724 ; +2 170). Flux minimaux : A (−1 040 ; −735 ; −310), B (−1 990 ; −727 ; −160), C (−930 ; −711 ; −322).

### 5.5 Ce que disent ces chiffres

- **Option 0.** VAN nulle, mais pas gratuite : si le fondateur consacre un mi-temps au palier 1 pendant 12 mois au lieu d'un emploi tech, il renonce à ≈ 2–4 M XPF de revenu [estimé : 250 000–400 000 XPF/mois à mi-temps]. Ce coût d'opportunité **n'est pas dans les VAN de A, B et C** (fondateur non rémunéré) ; il les aggraverait d'autant. Inversement, ne rien faire, c'est renoncer à l'apprentissage de la filière, au laboratoire de marque et aux premiers clients : la valeur de l'option « continuer vers le palier 2 », non chiffrée ici, est la vraie raison de faire le palier 1.
- **A vs C.** Équivalentes à ±50 k : C coûte ≈ 20 XPF de marge par coco mais 110 k de CAPEX en moins et moins de gestion de main-d'œuvre. La décision n'est pas financière : elle porte sur le contrôle de la qualité, du geste et de la marque, et sur le risque que la cocoteraie apprenne le métier et se passe de NĪĀ.
- **B.** La machine économise ≈ 75 XPF/coco mais coûte ≈ 950 k + 10 k/mois. **Seuil de bascule** : (950 + 10 × 24) ÷ 75 ≈ 15 900 cocos sur 24 mois, soit **≈ 650 cocos/mois en moyenne (≈ 30/jour)**. Le réaliste cumule 15 160 cocos : juste en dessous. Règle de décision : ne pas acheter au lancement ; acheter quand trois mois consécutifs dépassent 650 cocos, ce qui arriverait en juillet–août 2027 dans le réaliste et en mai 2027 dans l'optimiste.
- **Prix d'équilibre.** Pour A réaliste, VAN = 0 à 12 % demande ≈ +67 XPF de marge par coco (844 ÷ 12,5 ; cf. § 6), soit un **prix ≈ 570 XPF**, ou ≈ +50 % de volume, ou un local gratuit et un prix de 540.

---

## 6. Sensibilité (option A, scénario réaliste, VAN à 12 %)

Raccourci de calcul : un écart de **Δ XPF de marge par coco** vaut **ΔVAN ≈ Δ × 12,5 k XPF** (4 360 × 0,8929 + 10 800 × 0,7972 ≈ 12 500 cocos actualisées). Base : −844 k.

| Rang | Variable | Base | −20 % | +20 % | ΔVAN à −20 % | ΔVAN à +20 % | VAN à −20 % | VAN à +20 % |
|---|---|---|---|---|---|---|---|---|
| **1** | **Prix de vente** | 500 | 400 | 600 | **−1 250** | **+1 250** | −2 094 | **+406** |
| **2** | **Volume** (toutes années) | 4 360 / 10 800 | −20 % | +20 % | −353 | +353 | −1 197 | −491 |
| **2 ex.** | **Prix d'achat de la coco** (effet ÷ 0,85 de perte) | 120 | 96 | 144 | +353 | −353 | −491 | −1 197 |
| 4 | Main-d'œuvre de découpe | 100 | 80 | 120 | +294 | −294 | −550 | −1 138 |
| 4 ex. | Coûts fixes mensuels | 75 k | 60 k | 90 k | +290 | −290 | −554 | −1 134 |
| 6 | Durée de conservation (rythme de découpe et invendus) | 14 j | 11 j | 17 j | −175 | +60 | −1 019 | −784 |
| 7 | Taux de perte | 15 % | 12 % | 18 % | +134 | −143 | −710 | −987 |

Compléments hors ±20 % :

| Cas | Effet | VAN |
|---|---|---|
| Conservation réelle **7 jours** (falaise : découpe presque quotidienne, +1 500 XPF de mise en route par séance, invendus +5 points, Moorea difficile) | ≈ +30 XPF/coco → −375 k | −1 219 |
| Rémunérer le fondateur 150 k/mois chargé en année 2 seulement | −1 800 × 0,7972 = −1 435 k | −2 279 |
| Local prêté (0 au lieu de 40 k/mois) | +40 k × (11 × 0,8929 + 12 × 0,7972) ≈ +775 k | −69 |
| Facturer Moorea 560 XPF au lieu de 500 | +60 × 2 310 cocos Moorea actualisées ≈ +105 k | −739 |

Pourquoi la conservation n'est pas linéaire : à 14 jours, deux séances de découpe par semaine suffisent et les invendus restent faibles ; à 11 jours il en faut trois ; sous 7 jours la découpe devient quotidienne, le coût fixe de chaque séance (déplacement, nettoyage) se répartit sur moins de cocos et les livraisons à Moorea perdent leur marge de sécurité. **La durée de conservation ne fait pas beaucoup bouger la VAN tant qu'elle est ≥ 10 jours ; elle devient le premier risque si elle est < 7 jours.** C'est pourquoi le test de lot (item 4) précède le pilote.

---

## 7. Modes de financement possibles

Montants et conditions [estimé] ou [supposé] ; tout dispositif public est à **vérifier auprès de la DGAE, du SEFI, de la Direction de l'agriculture et de la CCISM** (noms, plafonds et critères changent).

| Source | Pour quoi | Montant plausible | Coût | Délai | Conditions et remarques |
|---|---|---|---|---|---|
| **Apport du fondateur** | CAPEX A + trésorerie | 2–5 M (acquis dans l'énoncé) | 0 en cash ; coût d'opportunité du placement ≈ 1–2 %/an et du temps | Immédiat | Garder 0,5 M de réserve personnelle hors projet ; ne pas tout mettre au mois 1 |
| **Microcrédit professionnel (ADIE Polynésie)** | Compléter la trésorerie de A | jusqu'à ≈ 1–1,2 M | Taux ≈ 7–9 % + frais [estimé] | 3–6 semaines | Accessible à un créateur sans historique ; accompagnement inclus ; à vérifier |
| **Prêt bancaire création (Banque de Tahiti, Banque de Polynésie, Socredo)** | Machine (B) ou véhicule | 1–3 M sur 3–5 ans | Taux ≈ 4–7 % [estimé] + garantie personnelle ; possible garantie SOGEFOM (fonds de garantie outre-mer, AFD) [à vérifier] | 1–3 mois | Apport 20–30 %, business plan, souvent 6–12 mois d'activité : plutôt pour la machine en 2027–2028 que pour le lancement |
| **Crédit-bail / leasing de la machine** | Variante B sans sortir 950 k | 0,8–1,2 M | ≈ 6–8 %/an [supposé] | 1–2 mois | Évite le point bas à −2,65 M ; conditionné à l'existence d'un fournisseur acceptant le montage ; à vérifier |
| **Aide à l'équipement des petites entreprises (AEPE, Pays / DGAE)** | Réfrigérateur, machine, matériel | subvention d'une part de l'équipement, plafond de l'ordre de 1–3 M [à vérifier] | 0 | 2–4 mois d'instruction, versement après facture | Patente à jour, entreprise créée ; **préfinancer l'achat** |
| **Dispositifs d'insertion par la création (SEFI, type ICRA)** | Aide au créateur | de l'ordre de 0,3–0,6 M [à vérifier] | 0 | 1–3 mois | Réservé aux demandeurs d'emploi inscrits ; dépend du statut du fondateur |
| **Aides à l'agro-transformation (Direction de l'agriculture, programmes d'équipement)** | Chambre froide, atelier, machine | à relever | 0 | Long (dossier annuel) | NĪĀ n'est pas producteur agricole : éligibilité incertaine ; la cocoteraie partenaire pourrait l'être pour la découpe (option C) |
| **Prêt d'honneur (réseau Initiative, s'il est présent en PF)** | Fonds propres complémentaires | 0,5–1,5 M [à vérifier] | 0 % | 2–3 mois | Comité d'engagement ; effet de levier sur la banque |
| **Associé** | Métier manquant (filière coco, agro, commercial) + cash | 1–3 M contre 20–40 % du capital [supposé] | Dilution, gouvernance | 1–3 mois | La bonne raison est le métier, pas le cash ; à décider avant la création de la société |
| **Financement participatif (don contre récompense, Ulule ou équivalent)** | Laboratoire de marque, petit cash | 0,5–1,5 M | ≈ 8 % de commission + récompenses + temps | 2–3 mois | Pas de prévente B2B ; utile pour tester l'adhésion polynésienne à la marque ; risque d'exposition prématurée |
| **Préfinancement par un opérateur** | Trésorerie du pilote | 1–3 mois de livraisons, ≈ 0,2–0,5 M | Remise 5–10 % ou exclusivité temporaire | 2–4 semaines | Nécessite la confiance et un pilote écrit ; le plus rapide et le plus parlant pour un sponsor |
| **Délai fournisseur** | Réduire le BFR | 30 jours de paiement à la cocoteraie ≈ 0,1–0,15 M | Prime au prix possible | Négociation | Peu probable au départ avec un petit producteur |
| **Prise en charge du fret maritime par le Pays** (arrêté n° 1586 CM, § 1.5) | Aide en nature sur les cocos brutes achetées dans une île | ≈ 40–75 XPF/coco de fret évités, soit 0,1–0,5 M/an selon le volume [estimé] | 0 | Dossier DGAE, carte CAPL ou inscription RCS [à vérifier] | Sens îles → Tahiti, produit non transformé ; ne couvre probablement pas la livraison de cocos découpées vers Moorea |

**Montage suggéré pour A (réaliste)** : apport 2 M + préfinancement d'un opérateur 0,3 M ou microcrédit 0,5 M, pour disposer de ≈ 2,3–2,5 M. **Pour la machine (B ou A → B en 2027–2028)** : AEPE préfinancée par un prêt bancaire ou un leasing, décidés une fois le seuil de 650 cocos/mois observé.

---

## 8. Les 10 chiffres à relever sur le terrain, par impact sur la VAN

| Rang | Chiffre | Impact VAN (±20 %) | Qui | Comment |
|---|---|---|---|---|
| **0 — préalable** | **Conditions du fret agricole gratuit** : produits éligibles (coco parée = produit agricole brut ou transformé ?), sens couverts (îles → Tahiti seulement ? Tahiti → Moorea ?), compagnies conventionnées, formalités (carte CAPL, RCS, dossier DGAE) | Pas une sensibilité : décide **où l'on découpe** (avant ou après le transport), **où l'on achète** (île productrice à fret nul : jusqu'à +590 k) et la marge Moorea (+90 k) | supply-analyst, avec operations-director pour le réglementaire | Lire l'arrêté n° 1586 CM et sa modification de 2026 sur Lexpol ; appeler la DGAE ; demander à Aremiti et Terevau la procédure et un devis fret payant |
| 1 | **Prix accepté par l'opérateur** et son coût actuel par passager (achat, temps d'ouverture, perte) | ±1 250 k | market-scout | 5–8 entretiens avec grille : « combien vous coûte une coco servie aujourd'hui ? » puis test des trois niveaux 400 / 500 / 600 |
| 2 | **Prix d'achat de la coco nīā** récoltée au stade demandé, par 100, livrée ou à prendre ; prix d'une coco jeune à boire au marché de Papeete comme référence | ±353 k, **et aucune source trouvée, même web** | supply-analyst | 3 cocoteraies (Tahiti, Moorea, une île à fret gratuit), devis écrit, prime de sélection, régularité promise ; relevé au marché de Papeete et au bord de route |
| 3 | **Volume** : passagers/jour, jours d'activité/mois par saison, part de passagers qui prennent la coco | ±353 k | market-scout | Mêmes entretiens + calendrier d'activité 2026 ; recouper avec les plannings publiés et le bilan ISPF 2025 (§ 2.1) |
| 4 | **Temps de découpe + conditionnement** par coco, en série de 50, par un découpeur formé | ±294 k | process-engineer | Chronométrage sur le lot test (item 4), geste manuel, outils fixés |
| 5 | **Coût et disponibilité d'un découpeur** à la tâche vs temps partiel (prix demandé, statut, patente) | ±294 k | operations-director / process-engineer | 3 candidats ou prestataires ; cocoteraie pour l'option C |
| 6 | **Loyer et disponibilité d'un local** de préparation avec froid | ±290 k (via les fixes) | process-engineer | 3 pistes : dépendance, espace chez la cocoteraie, local commercial ; devis ou prêt |
| 7 | **Durée de conservation réelle** après découpe au froid | −175 k à 11 j, **−375 k sous 7 j** | process-engineer | Lot de 30 cocos, contrôle J+3/7/10/14/21, analyses labo ; fixe la DLC et le rythme |
| 8 | **Taux de non-conformité à réception et de casse** | ±140 k | supply-analyst + process-engineer | Check-list qualité appliquée sur 3 livraisons successives |
| 9 | **Coût réel du fret Tahiti–Moorea** d'un bac réfrigéré (variante payante) et conditions de chaîne du froid à bord | ≈ ±105 k (sur la part Moorea) | supply-analyst | Devis Aremiti et Terevau (aucune grille publique trouvée) ; test d'un bac ; qui réceptionne à Vaiare |
| 10 | **Délai de paiement et mode de commande** des opérateurs ; équipement froid chez eux | Décide du point bas (±0,35 M de BFR) plus que de la VAN | market-scout | Dans les entretiens : qui commande, quand, qui paie, à quel délai, où stockent-ils |

À relever aussi, pour la décision machine : prix rendu Tahiti d'une machine de découpe, débit et taux de casse (process-engineer, item 9).

---

## Limites de ce modèle

1. Aucun chiffre n'est relevé : le coût de revient central (350 XPF) a une incertitude d'au moins ±40 % et la VAN change de signe avec ±70 XPF sur le prix de vente.
2. Le fondateur n'est pas rémunéré sur 24 mois ; intégrer un mi-temps à 150 k/mois rend toutes les options négatives, y compris l'optimiste en année 1.
3. Les flux sont regroupés en fin d'année pour la VAN, la saisonnalité de l'année 2 est lissée, la valeur résiduelle du matériel est à zéro et la fiscalité (TVA, impôt sur les transactions ou IS) n'est pas modélisée.
4. La valeur de l'option « continuer vers le palier 2 » (apprentissage, marque, clients) n'est pas chiffrée : c'est pourtant elle qui décide, pas la VAN du palier 1 seul.
5. Les scénarios supposent qu'un opérateur signe au mois 5 et que la cocoteraie livre régulièrement : les deux risques majeurs de la vision ne sont pas probabilisés, seulement encadrés par le scénario minimal ; le fret inter-îles est modélisé en variante payante, l'éligibilité au fret agricole gratuit (sens, produit transformé ou non) n'étant pas vérifiée sur Lexpol.
