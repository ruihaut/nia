# Synthèse binôme — fusion de la version du collègue (recap et slides du 23–24 octobre) et de la version du dépôt

> Rédigée le 2026-10-24 par le Director-General, à chaud, pour la soutenance PMBOK + Agile (CSC Tahiti, 20 à 30 min en binôme, trois documents et une démo, fil rouge NPS et CSAT). Règle de langue adoptée partout : **le coco**, un coco, le NĪĀ. Les documents du collègue sont versés dans `docs/notes/2026-10-24-collegue/`.
> Lecture : **✅ convergent** (on garde), **⚖️ à trancher** (les deux versions diffèrent, recommandation donnée), **➕ apport du collègue** (absent du dépôt, à intégrer).

## 1. Ce qui converge ✅

| Sujet | Les deux versions disent |
|---|---|
| Le nom et le ton | nīā = le stade exact ; marque sobre, fierté plutôt qu'exotisme ; « En France ils ont le raisin, en Polynésie nous avons le coco » |
| Le client du palier 1 | Les agences réceptives paient, dans leur forfait ; l'opérateur d'excursion est un marché secondaire (Could) |
| Le produit | Coco nīā diamond cut, froid, présenté façon NĪĀ, origine dite ; découpe à la main au palier 1, machine seulement au-delà d'un seuil (collègue : ≈ 500 par semaine ; dépôt : ≈ 650 par mois sur trois mois, à aligner sur les mesures) |
| Le marché | ISPF 2025 : 281 227 touristes, ≈ 70 000 croisiéristes, 42 % Amérique du Nord |
| L'économie | Prix autour de 650–700 XPF ; à 500 on perd de l'argent ; point mort ≈ 70 cocos par semaine (collègue) = ≈ 285 par mois (dépôt) ; frais fixes ≈ 100 k par mois en structure légère ; le binôme ne se paie pas au palier 1 ; aucun chiffre relevé, tout à confirmer par des devis |
| L'approvisionnement | Pas de cocoteraie en propre ; producteurs payés au juste prix ; critère de stade nīā écrit ; ≥ 2 producteurs ; MOUʻA (Tahiti, Moorea) comme base, MOTU plus tard |
| Les garde-fous | Le palier 1 n'est pas une fin en soi ; gates avec preuves ; pré-mortem « pourquoi ça n'existe pas déjà » ; test de conservation avant toute remise payante ; hygiène et autorisations en prédictif, rituel et service en agile |
| Le pivot tracé | Le changement de client (excursions → accueil) est une demande de changement PMBOK : quoi, pourquoi, impacts, qui valide (dépôt : comité de changement ; collègue : tableau avant / après) |

## 2. Ce qui diverge ⚖️ et la recommandation

| # | Sujet | Version du collègue | Version du dépôt | Recommandation |
|---|---|---|---|---|
| 1 | **Équipe** | Un binôme : sponsor, chef de projet, Product Owner | « Fondateur seul » | ➜ **Binôme.** Charte : A et B, l'un sponsor par intérim et PO, l'autre chef de projet ; à nommer |
| 2 | **Formats du palier 1** | Deux formats : (1) accueil à l'aéroport, remis avec le collier à la sortie de la douane, livré la veille au dépôt de l'agence ; (2) premier stop du tour de l'île (pointe Vénus, puis Maraa), glacière dans le bus, le guide sert et reprend les cocos vides ; « un accueil, pas un point de vente » | Remise au lobby de l'hôtel après le check-in ; aéroport écarté (score 3,0 : file, bagages, nuit) ; hôtel = veto de fait | ➜ **Pilote = le stop pointe Vénus** (concret, de jour, jours de paquebot connus des mois à l'avance, collecte facile, aucun hôtel à convaincre). **Should** : Maraa, puis aéroport **ou** lobby d'hôtel : les deux analyses s'accordent sur les objections de l'aéroport (nuit, correspondances, liquides, autorisation du terminal) ; garder le lobby d'hôtel comme variante du format aéroport, à tester en G3 |
| 3 | **Paliers 2 et 3** | Palier 2 = le même coco servi à l'hôtel, co-marqué « Hôtel × NĪĀ » ; palier 3 = la bouteille, « à trancher » | Palier 2 = la bouteille à la carte des CHR (finalité de `VISION.md`) | ➜ **Trois paliers** : la finalité reste la bouteille à la carte ; le coco co-marqué dans les hôtels devient le palier 2 (pont naturel : le décideur hôtelier voit le produit), la bouteille le palier 3. **Décision du mainteneur : amender `VISION.md` (gate ①)** |
| 4 | **Prix de vente** | 650 XPF HT (500–800) | 700 (net ≥ 590 après commission) ; message du fondateur ce jour : 800 | ➜ Présenter **650 en base, 500 et 800 en sensibilité** (tableau du collègue) ; c'est cohérent avec « VAN nulle à ≈ 590 » du dépôt ; 800 = cas optimiste, à tester à haute voix |
| 5 | **Coût par coco** | ≈ 300 (découpe 45 à 1 min 45 par coco, carte 25, paille 15, froid 10, livraison 25, collecte 10, pertes 15) | ≈ 365 (découpe 100 à 3 min, présentation 60) | ➜ Fourchette **300–365**, le temps de découpe (1 min 45 ou 3 min) et la présentation sont à mesurer sur le lot test |
| 6 | **Volume de base** | 100 cocos par semaine, 400 par mois ; 1 jour de paquebot à 3 bus ≈ 100 cocos | 5 280 la première année (≈ 440 par mois en moyenne, 1 000 en régime) | ➜ **400 par mois en base du pilote** (collègue), 1 000 par mois comme régime à G3 (dépôt) ; ≈ 90 cocotiers pour 5 200 par an, 1 producteur suffit, 2 pour la sécurité |
| 7 | **Arrivées par jour** | ≈ 620 (hébergement à terre 227 286 ÷ 365) | ≈ 770 (tous touristes) | ➜ **620** pour les arrivées à terre, c'est le bon dénominateur ; 1 agence à 10 % ≈ 60 cocos par jour |
| 8 | **Besoin de financement** | ≈ 1,9 M (1,6 M d'investissement + 3 mois de fixes) ; remboursement ≈ 40 mois à 400 par mois | 1,28 M d'investissement ; 2,5 M à disposer (3 M à 60 jours) à cause du point bas de trésorerie | ➜ **1,9 à 2,5 M** selon le délai de paiement des agences ; dire les deux hypothèses |
| 9 | **Satisfaction** | Fil rouge : CSAT touristes ≥ 4,5 (QR code sur la carte), NPS agences ≥ +50, NPS en direct avec le jury | KPI opérationnels (remises / arrivées ≥ 95 %, prix net, marge, livraisons à l'heure) ; pas de NPS grand public | ➜ **Les deux** : CSAT et NPS comme critères de succès de la charte (exigence de la formation et bons signaux de marque), KPI opérationnels dans le plan |
| 10 | **Gates** | G0 lancer · G1 investir · G2 premières remises · G3 étendre · G4 palier 2 | Go-0 (validé) · Go-1 le 4 janvier 2027 · J1–J8 · Go-2 | ➜ **Nommer G0–G4 à la manière du collègue** (lisible PMBOK) et garder les dates du dépôt : G0 = charte signée (fait pour la phase de vérification) ; G1 = 4 janvier 2027 ; G2 = conformité + autorisation du stop + CSAT ≥ 4,5 au test (mars) ; G3 = après un mois de pilote (mai) ; G4 = octobre 2027 |
| 11 | **WBS** | 15 lots (règle des 100 %, dont management, déchets, satisfaction, études palier 2) | 8 branches, 32 work packages avec dictionnaire | ➜ Présenter les **15 lots** (plus parlants au jury), garder le dictionnaire du dépôt comme détail ; ajouter au dépôt les lots déchets, satisfaction, accueil aéroport, stops |
| 12 | **MOTU / MOUʻA** | Deux cuvées d'origine ; dégustation à l'aveugle MOUʻA contre MOTU dans la démo | Aucune promesse gustative avant un test triangulaire ; une seule référence d'abord | ➜ Compatible : présenter MOUʻA et MOTU comme **origines** (lieu, transport, fraîcheur 48–72 h), et la dégustation de la démo comme ce qu'elle est : un test, pas une preuve |

## 3. Apports du collègue à intégrer ➕

- **Zéro gaspillage** : carte attachée au coco (« gardez-le pour la photo, puis déposez-le au point NĪĀ, il retournera à la cocoteraie » + QR code CSAT), sac de collecte dans le bus, reprise à l'hôtel partenaire, bourre en compost chez les producteurs, cocos déclassés en glaces avec un glacier (Buy), pailles papier ou bambou, pas de charbon de bourre.
- **Horaires d'arrivée relevés** (à vérifier selon jour et saison) : TN Los Angeles 21 h 30 et 4 h 10 ; AF Los Angeles ≈ 5 h ; TN Tokyo 6 h 25 ; TN Auckland 22 h ; NZ 2 h 25 ; UA San Francisco 18 h 55 : surtout le soir et la nuit, d'où « pas de nuit chez NĪĀ, livraison la veille au dépôt de l'agence ».
- **Agences identifiées** : Marama Tours (≈ 400 places, 18 véhicules, aéroport, paquebots, tours de l'île : candidat pilote), Tahiti Nui Travel, Te Manu Tours (accueil avec pancarte, collier et eau fraîche à la sortie de la douane), Tahiti Tours, Tahiti Travel Services, Tahiti Expert DMC, Paradise Tours, Polynésie Voyages, Manaventura, Tekura, Moana Voyages, Tahiti Experiences (liste officielle service-public.pf).
- **Les stops** : pointe Vénus (Mahina, ≈ 10 km du port, premier arrêt, ≈ 15 min, récit « 1769 : Cook observe ici le passage de Vénus. Aujourd'hui, votre premier NĪĀ ») et grottes de Maraa (Paea, ≈ 28 km, 20–30 min, à l'abri de la pluie) ; trois options de service (A glacière dans le bus, B partenaire local contre commission, C hôte NĪĀ sur site) ; 5 bus de 20–45 passagers = 150–200 cocos un jour de paquebot ; autorisations commune de Mahina et Paea à vérifier.
- **Registre d'hypothèses H1–H10** rattachées à des gates, **MoSCoW**, **questions probables du jury** avec réponses, **déroulé minuté en alternance A/B** (25 min), **démo** (collier + vrai NĪĀ taillé, dégustation, QR code, NPS en direct, reprise des cocos vides devant le jury).
- **Références HBR** utiles pour la soutenance : Pine et Gilmore (expérience), Kim et Mauborgne (océan bleu), Porter et Kramer (valeur partagée), Flyvbjerg et Budzier (dérapage des projets), Reichheld (NPS), Embracing Agile.

## 4. Ce que le dépôt apporte au collègue

Le modèle financier complet (A1, A1b : VAN, TRI, point bas, sensibilités), la comparaison des canaux et les risques du pivot (A9), les customer journeys (A5, A8), la concurrence sourcée (A10 : import d'eau de coco interdit depuis 2023, ≈ 10 producteurs artisanaux, Hanahana Tours déjà sur le créneau « collier + bouteille + serviette », coco de rue à 200 XPF), le réglementaire (A2 § 7 : CHSP, DGAE, biosécurité, fret agricole), variétés et terroirs (A6), architecture de gamme (A7), la fiche des chiffres clés (04), et la chaîne de références PMBOK (baselines, comité de changement, RACI, Definition of Done, PV de recette).

## 5. Les chiffres à dire en soutenance (base commune)

| | Valeur | Statut |
|---|---|---|
| Arrivées à terre par jour | ≈ 620 ; 1 agence à 10 % ≈ 60 NĪĀ par jour | ISPF, calcul |
| Base du pilote | 100 cocos par semaine, 400 par mois ; 1 jour de paquebot à 3 bus ≈ 100 cocos | décision binôme |
| Achat au producteur | ≈ 150 XPF (100 à 200 ; 300 pessimiste) | à relever |
| Prix à l'agence | ≈ 650 XPF HT (500 à 800) | à tester |
| Coût par coco | ≈ 300 à 365 XPF | à mesurer |
| Marge par coco | ≈ 350 XPF (54 %) | déduit |
| Frais fixes, structure légère | ≈ 100 000 XPF par mois | devis à faire |
| Point mort | ≈ 70 cocos par semaine (≈ 290 par mois) | déduit |
| Résultat mensuel à 400 cocos | +40 000 à 650 ; −20 000 à 500 ; +100 000 à 800 | déduit |
| Et si ça marche | 250 par semaine : +170 000 par mois ; 500 par semaine avec machine : +450 000 | projection |
| Besoin de financement | ≈ 1,9 M (2,5 M si les agences paient à 60 jours) | déduit |
| Approvisionnement | ≈ 5 200 cocos par an ≈ 90 cocotiers ≈ 1 ha ; 1 producteur suffit, 2 pour la sécurité | calcul |
| Découpe | 1 min 45 à 3 min par coco ; ≈ 3 à 6 h par semaine à la main ; machine seulement au-delà de ≈ 500 par semaine | à mesurer |
| Succès du pilote | 95 % des bus servis · CSAT ≥ 4,5 · NPS agence ≥ +50 · 100 % des cocos vides récupérés · marge positive | charte |

## 6. À trancher aujourd'hui par le binôme

1. Les trois paliers (coco co-marqué à l'hôtel en 2, bouteille en 3) → amendement de `VISION.md`.
2. Le second format : aéroport (collègue) ou lobby d'hôtel (dépôt), ou les deux en Should.
3. Le prix de base en soutenance : 650.
4. Qui est sponsor, qui est chef de projet, qui est PO dans le binôme.
5. Le pilote : 1 agence (Marama Tours à contacter) × pointe Vénus × jours de paquebot × 1 mois × option A.

## 7. À faire avant la soutenance (fusion des deux listes)

- Contacter une agence réceptive (Marama Tours), prix dit à haute voix ; mairie de Mahina ; devis frigos et cuisine partagée ; 2–3 prix producteurs.
- Lot test de conservation et protocole de découpe (temps réel par coco ; température 2–4 °C contre 6–8 °C).
- Mettre à jour `VISION.md`, la charte et le plan : binôme, trois paliers, formats, 15 lots, gates G0–G4, NPS / CSAT, zéro gaspillage.
- Préparer la démo (vrais NĪĀ, colliers, cartes avec QR code) et répéter en chronométrant (25 min, alternance A/B).
