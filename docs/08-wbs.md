# WBS consolidé — NĪĀ, projet « étape 1 + préparation de l'étape 2 »

> v1 du 2026-10-24. Fusion des 15 lots du collègue (règle des 100 %) et des 32 work packages du dépôt (annexe A2, dictionnaire complet), plus le lot propre à l'étape 1 (vente au détail à la pointe Vénus). Niveau 1 = lot ; niveau 2 = work package (WP). Chaque WP a un livrable, un critère d'acceptation, une durée de travail effectif, un coût estimé hors temps du binôme, ses dépendances et sa gate. Coûts en XPF, estimés ; durées en semaines ; M0 = novembre 2026. Le digital est hors projet.

## Arborescence

```
NĪĀ — étape 1 (vente au détail pointe Vénus) + préparation étape 2 (agences réceptives)
├── 1  Management du projet
├── 2  Cadrage business
├── 3  Structure, administratif et marque (dépôt)
├── 4  Approvisionnement (cocos nīā)
├── 5  Production (découpe, atelier, froid)
├── 6  Réglementaire et hygiène
├── 7  Logistique et chaîne du froid
├── 8  Étape 1 : stand NĪĀ à la pointe Vénus
├── 9  Étape 2 : commercial agences réceptives
├── 10 Étape 2 : formats d'accueil (stops, aéroport ou hôtel)
├── 11 Marque et présentation
├── 12 Mesure de la satisfaction (CSAT, NPS)
├── 13 Zéro gaspillage et déchets
├── 14 Financement et équipe
└── 15 Études des étapes 3 et 4
```

## Dictionnaire par lot

### 1. Management du projet (gates G0 → G4)

| WP | Livrable | Critère d'acceptation | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 1.1 Charte, business case, plan (les trois documents) | Trois documents signés, synthèse binôme, présentation | Signés par le sponsor par intérim et le chef de projet ; relus par le challenger | 2 | 0 | — | G0 |
| 1.2 Registre des hypothèses et des risques | H1–H10, matrice de 65 risques, revue mensuelle | Chaque hypothèse a une vérification et une gate ; chaque risque rouge a une action datée | 1 puis récurrent | 0 | 1.1 | G0 |
| 1.3 Pilotage : tableau de bord, revues sponsor, comité de changement | Tableau de bord mensuel d'une page, comptes rendus, journal des décisions | Revue tenue chaque mois ; chaque chiffre passe de « estimé » à « relevé » | 2 h/semaine, 52 semaines | 0 | 1.1 | continu |
| 1.4 Demande de changement du pivot | Fiche avant / après (client, moment, étapes), impacts, validation | Validée au comité ; vision amendée | 1 | 0 | 1.1 | G0 |
| 1.5 Clôture : PV de recette, bilan, leçons apprises | PV signé par l'agence (et l'hôtel ou la commune), bilan en chiffres relevés, rétrospectives | Chaque chiffre du bilan est relevé ; décision tracée | 2 | 0–10 k | tout | G4 |

### 2. Cadrage business

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 2.1 Pré-mortems (« pourquoi ça n'existe pas déjà », « octobre 2027, échec ») | Deux pré-mortems relus avec les relevés | Chaque cause a un signal précoce et une vérification | 1 | 0 | 8.1, 9.1 | G1 |
| 2.2 Modèle économique v1 (base 100 cocos par semaine, scénarios 500 / 650 / 800, sans aides) | Tableur et note | Chaque ligne relevée ou datée ; point mort, trésorerie, seuil d'arrêt | 2 (v0) + 2 (v1) | 0 | 4.2, 5.1, 9.2 | G1 |
| 2.3 Concurrence et vérifications terrain (liste DAG des producteurs, prix de rue, interdiction d'import confirmée) | Note de concurrence mise à jour | Cinq vérifications faites | 2 | 0–10 k | — | G1 |

### 3. Structure, administratif et marque (dépôt)

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 3.1 Création de l'entité (CDFE, RCS, patente, n° TAHITI, CPS) | Extrait, patente | L'entité peut facturer, encaisser et employer | 4 | 30–150 k | 1.1 | G1 |
| 3.2 Assurances (RC professionnelle denrées et livraison, accident) | Attestations | Intoxication et livraison couvertes | 2–4 | 60–200 k/an | 3.1 | G2 |
| 3.3 Banque, caisse, terminal de paiement | Compte, TPE | Encaissement possible au stand | 2 | 10–30 k | 3.1 | G2 |
| 3.4 Dépôt de marque (après vérification H9 : nom descriptif) | Avis, dépôt du logo et de la présentation | Décision prise avant la première facture | 2 | 0–100 k | 11.1 | G2 |

### 4. Approvisionnement (cocos nīā)

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 4.1 Critère de stade nīā écrit et testé (par variété) | Fiche illustrée FR / tahitien, grille, lot de 30 ouverts | Deux personnes classent 30 cocos avec ≥ 90 % d'accord ; Brix mesuré | 4 | 15–45 k | — | G1 |
| 4.2 Cartographie et sélection de ≥ 2 producteurs (Tahiti ; fournisseur de Huahine et coopérative de Arue rencontrés) | ≥ 4 fiches visitées, 2 retenues, prix écrits | Prix et volume relevés ; source principale ≥ 100 nīā/semaine | 6 | 20–60 k | 4.1 | G1 |
| 4.3 Contrat producteur principal + lettre d'intention de la seconde source | Contrat 2–3 pages | Fiche nīā annexée, règle de refus, prix ≤ cible | 4 | 0–100 k d'acompte | 4.2, 2.2 | G1 |
| 4.4 Achat et contrôle à réception (check-list 12 points, lots, registre) | Protocole, registre | Chaque lot numéroté ; refus ≤ 10 % en régime | 2 puis récurrent | 0 | 4.3 | G2 |
| 4.5 Dégustation comparative variétés × terroirs (MOUʻA / MOTU, test triangulaire) | Rapport, décision de gamme | Critères écrits à l'avance ; 12 juges à l'aveugle | 6–8 | 40–90 k | 4.2 | G3 |

### 5. Production (découpe, atelier, froid)

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 5.1 Protocole diamond cut manuel mesuré (ouverture sans outil) | Protocole illustré, mesures | ≤ 3 min/coco, ≤ 10 % de perte, 0 blessure, reproductible par un tiers | 5 | 60–200 k | 4.1 | G1 |
| 5.2 Test de conservation (2–4 °C, 6–8 °C, réfrigérateur d'hôtel, glacière de nuit ; analyses) | Rapport, DLC, rythme découpe → livraison | DLC fixée avec marge ; décision lieu et rythme | 7 | 130–420 k | 5.1 | G1 (lot 1), G2 |
| 5.3 Atelier ou cuisine agréée partagée + froid (deux réfrigérateurs professionnels, d'occasion si possible) | Convention, atelier aménagé, froid à 2–4 °C ou 6–8 °C selon 5.2 | Conforme aux points du CHSP ; capacité une semaine | 8 | 0,5–1,5 M (légère) ; 1–2,45 M (local loué) | 14.1, 5.2 | G1 → G2 |
| 5.4 Recrutement et formation du découpeur (à la tâche puis temps partiel) | Fiche de poste, contrat, formation hygiène | 20 cocos/h sans blessure sur 40 cocos ; une personne de secours | 5 | 60–150 k | 5.1, 5.3 | G2 |
| 5.5 Production des lots (à blanc puis payants) | Registre de production | À blanc n° 2 : 100 % conformes et au froid en moins d'une heure | 2 puis récurrent | 60–130 k | 4.4, 5.3, 5.4 | G2 |
| 5.6 Note make or buy machine (seuil ≈ 500 cocos/semaine) | Note chiffrée | Seuil de bascule et options rendues Tahiti | 2 | 0 | 5.1, 5.5 | G3 |

### 6. Réglementaire et hygiène

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 6.1 Cadrage réglementaire : CHSP (semaine 2), DGAE, biosécurité, DICP (TVA), 19 questions | Note réglementaire, comptes rendus | Chaque obligation confirmée, infirmée ou en attente avec interlocuteur et date | 6 | 0–20 k | 1.1 | G1 |
| 6.2 Plan de maîtrise sanitaire simplifié (HACCP), formation hygiène | Classeur PMS ≤ 10 pages, fiches | Appliqué sans aide par le découpeur ; relu par le CHSP | 4 | 0–80 k | 6.1, 5.1 | G2 |
| 6.3 Étiquetage, DLC, carte, bon de livraison | Maquettes validées | Lisibles après 14 jours au froid humide ; DLC justifiée | 3 | 30–100 k | 5.2, 6.1 | G2 |
| 6.4 Déclaration d'établissement déposée et obtenue ; vente ambulante déclarée | Récépissé | NĪĀ peut légalement préparer, vendre et livrer | 6 | 0–30 k | 6.1–6.3, 5.3, 3.1 | G2 |
| 6.5 Autorisation d'occupation du domaine public (mairie de Mahina, puis Paea) | Autorisation écrite | Obtenue avant la première vente | 4–8 | 0–50 k de redevance | 6.1 | G2 |

### 7. Logistique et chaîne du froid

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 7.1 Chaîne du froid de bout en bout (10 glacières, plaques, enregistreurs, sonde ; protocole) | Protocole, rapport de test | ≤ 7 °C à cœur pendant ≥ 6 h sur le trajet le plus long | 4 | 150–380 k | 5.2 | G2 |
| 7.2 Transport routier Tahiti (véhicule du binôme, tournée, livraison au dépôt de l'agence ou à l'hôtel de jour) | Plan de tournée | ≥ 95 % des livraisons à l'heure | 2 puis récurrent | 20–40 k/mois | 7.1 | G2 |
| 7.3 Processus commande → préparation → livraison → retours (liste des passagers à J−7 / J−1, bons, consigne des caisses) | Fiche de processus, modèles | Traçabilité de la facture au lot de récolte en 5 minutes | 2 | 0–20 k | 4.4, 6.3 | G2 |
| 7.4 Inter-îles (Moorea, MOTU) : deux variantes selon le fret agricole, test de froid | Procédure, grille de coûts | Décision écrite ; rien d'acheté avant | 4 | 20–50 k | 6.1 | G3 |

### 8. Étape 1 : stand NĪĀ à la pointe Vénus

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 8.1 Observation du site et des escales (calendrier du Port autonome, bus, vendeurs présents, durée de l'arrêt) | Fiche de site, calendrier | Deux escales observées, comptages faits | 2 | 0–10 k | — | G1 |
| 8.2 Accord avec les vendeurs locaux ou option B (partenaire sur site contre commission) | Accord oral puis écrit | Aucun conflit à la première escale | 3 | 0 | 8.1, 6.5 | G2 |
| 8.3 Stand et kit de vente (abri, glacières, TPE, caisse, affichage sobre, carte, pailles) | Stand prêt | Monté et démonté en 30 minutes ; deux personnes aux heures de pointe | 2 | 100–250 k | 3.3, 11.1 | G2 |
| 8.4 Test de prix (600 / 800) et premières ventes sur deux escales | Relevés de ventes, verbatims | ≥ 50 ventes par escale à 3 bus ; conversion mesurée | 2 | Cocos et glace | 5.5, 8.3 | G2 |
| 8.5 Pilote détail : un mois, jours de paquebot, 100 cocos/semaine | Journal des ventes, CSAT, photos, cocos vides repris | Marge par coco positive ; 100 % de collecte ; CSAT ≥ 4,5 | 4 puis selon décision | Fonds de roulement 100–200 k | 8.4 | G3 |
| 8.6 Critère de sortie vers l'étape 2 (durée écrite, pas de point de vente permanent) | Décision au comité | Date et conditions tenues | 1 | 0 | 8.5 | G3 |

### 9. Étape 2 : commercial agences réceptives

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 9.1 Qualification : entretien terrain (contact du fondateur), entretien décideur (Marama Tours, Te Manu Tours, Tahiti Nui Travel…), 2–3 hôtels d'arrivée | Fiches, prix dit à haute voix, dates de clôture 2027 / 2028, pièces exigées par l'hôtel | Un décideur nommé ; prix net ≥ 590 ; consentement écrit d'un hôtel | 6 | 20–60 k | — | G1 (15 décembre) |
| 9.2 Offre et prix net par passager (650 base, 500–800), conditions (J−7, 30 jours ou acompte) | Fiche offre | Testée auprès de ≥ 1 décideur sans refus | 2 | 0 | 2.2, 9.1 | G1 |
| 9.3 Accord à trois agence – hôtel – NĪĀ (froid tampon, geste, coque, welcome drink retiré, prix, paiement) ; validation du périmètre | Accord d'une page signé | Première remise datée ≤ 30 avril 2027 | 4 | 20–50 k | 9.2, 5.2, 11.1 | G2 |
| 9.4 Prise en main : fiche de remise de 15 minutes (agent, guide, night staff), vingt remises test observées | Fiche, rapport d'observation | ≥ 70 % de cocos bus ; geste reproduit sans aide | 2 | 30–100 k | 9.3, 11.2 | G2 |
| 9.5 Pilote agence : remises régulières ≥ 20 semaines, indicateurs | Journal, tableau d'indicateurs | ≥ 95 % des arrivées prévues servies ; marge positive 8 semaines | 20 | Fonds de roulement 0,3–0,8 M | 9.4, 5.5, 6.4, 7.3 | G3 → G4 |
| 9.6 Seconde agence ou hôtel en direct ; opérateurs d'excursion en appoint (à date écrite) | Deuxième accord | Un second compte qui commande avant octobre 2027 | 6 | 20–50 k | 9.5 | G3 |

### 10. Étape 2 : formats d'accueil

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 10.1 Stop pointe Vénus pour les bus des agences partenaires (option A : glacière dans le bus, le guide sert et reprend) | Procédure, formation des guides | 95 % des bus prévus servis | 3 | 20–50 k | 6.5, 9.3 | G2 |
| 10.2 Stop grottes de Maraa | Procédure, autorisation Paea | Idem | 3 | 20–50 k | 10.1 | G3 |
| 10.3 Accueil aéroport (autorisation du terminal, remise avec le collier, livraison la veille au dépôt) **ou** remise au lobby de l'hôtel après le check-in | Décision de format, procédure | Autorisation obtenue ; remises observées | 4 | 20–50 k | 9.1, 6.1 | G3 |

### 11. Marque et présentation

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 11.1 Présentation « façon NĪĀ » minimale : marquage, carte avec récit (pointe Vénus 1769, Maraa) et QR code, phrase FR/EN, fiche d'origine (cocoteraie, île, semaine) | Fiche, prototypes sur 10 cocos, coût unitaire ≤ 60 XPF | « J'en serais fier » auprès de 5 personnes dont des Polynésiens ; lisible après 7 jours au froid | 6 | 30–120 k | 5.1 | G2 |
| 11.2 Kit et marquage testés en conditions réelles (sel, soleil, bus) | Kit v1 ×2, rapport | Marquage intact sur ≥ 95 % des cocos | 3 | 40–120 k | 11.1, 5.5 | G2 |
| 11.3 Lexique tahitien validé (locuteur puis Fare Vānaʻa) ; mots motu et mouʻa réservés | Lexique | Validé par écrit | 2 | 0–20 k | 11.1 | G2 |

### 12. Mesure de la satisfaction

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 12.1 CSAT touristes par QR code sur la carte (une question, cinq étoiles, un mot) | Formulaire, tableau | ≥ 4,5 / 5 ; taux de réponse mesuré | 1 | 0–10 k | 11.1 | G2 |
| 12.2 NPS agences (et hôtels) : « recommanderiez-vous NĪĀ ? » 0–10 | Mesure à chaque sprint | ≥ +30 à G3, ≥ +50 à G4 | récurrent | 0 | 9.5 | G3, G4 |
| 12.3 Grille d'observation à la remise (bu, posé, photographié, nommé) et photos partagées (#NĪĀ) | Grille, comptage | 20 remises puis 2 séances par mois | récurrent | 0 | 9.4 | G2 |

### 13. Zéro gaspillage et déchets

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 13.1 Collecte des cocos vides (sac dans le bus, point NĪĀ au stand, accord de reprise avec 1–2 hôtels) | Procédure, accords | 100 % des cocos vides récupérés | 3 | 10 XPF/coco | 9.3, 10.1 | G2 |
| 13.2 Bourre en compost et paillage chez les producteurs | Accord producteur | Aucun déchet en décharge | 1 | 0 | 4.3 | G2 |
| 13.3 Cocos déclassés en glaces avec un glacier partenaire (Buy) ; pailles papier ou bambou ; pas de charbon | Accord, fournisseur de pailles | Un preneur identifié | 2 | 0 | 5.5 | G3 |

### 14. Financement et équipe

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 14.1 Besoin de financement et plan de trésorerie (1,9 M ; 2,5 M à 60 jours), seuil d'arrêt | Plan mensuel | Fonds disponibles ≥ besoin du scénario sobre | 2 | 0 | 2.2 | G1 |
| 14.2 Apport du binôme, acompte d'agence, microcrédit ; dossier sponsor sur preuves | Dossier, lettres | Seuils du sponsor annoncés ; pas d'argent externe avant une vente | 8 | 0–50 k | 14.1, 8.4, 9.3 | G1 → G3 |
| 14.3 Rôles du binôme (sponsor par intérim, Product Owner, chef de projet), relais à la tâche, journal de temps | Charte des rôles | Rôles écrits ; terrain ≥ 50 % | 1 puis récurrent | 0 | 1.1 | G0 |
| 14.4 Recrutements et statut (découpeur, relais du soir, temps partiel à ≈ 580 cocos/mois) | Contrats déclarés | Statut clarifié avant le premier paiement | 4 | 30–80 k/mois en régime | 5.4 | G2 → G3 |

### 15. Études des étapes 3 et 4

| WP | Livrable | Critère | Durée | Coût | Dépend de | Gate |
|---|---|---|---|---|---|---|
| 15.1 Étape 3 : coco entier co-marqué « Hôtel × NĪĀ » : cartographie CHR, prix, co-marquage contractuel, un hôtel intéressé | Note, lettre d'intérêt | Un hôtel intéressé à G4 | 4 | 0–20 k | 9.5 | G4 |
| 15.2 Étape 4 : faisabilité de l'eau extraite (durée de vie, process, froid, agréments), bouteille et verre, cépages (résultat de 4.5) ; **démarre au plus tard en juillet 2027** | Note de faisabilité, ordre de grandeur d'investissement | Décision documentée continuer / étendre / arrêter | 6 | 0–50 k | 4.5, 5.2 | G4 |
| 15.3 Dossier de décision G4 (bilan en chiffres relevés, make or buy, financement identifié) | Dossier sponsor | Décision tracée en octobre 2027 | 2 | 0 | 1.5, 15.1, 15.2 | G4 |

## Synthèse chiffrée

| | Valeur |
|---|---|
| Lots | 15 |
| Work packages | 62 |
| Jalons / gates | G0 charte signée (fait) · G1 investir, 4 janvier 2027 · G2 premières ventes et remises payantes, avril 2027 (limite 30 avril) · G3 étendre, après un mois de pilote (mai–juin 2027) · G4 étape suivante, octobre 2027 |
| Enveloppe, structure légère | ≈ 1,6 M d'investissement + ≈ 100 k/mois de fixes ; besoin de financement 1,9 M (2,5 M si paiement à 60 jours) ; phase de vérification ≤ 150 k |
| Postes qui font l'écart | L'atelier (cuisine partagée 40 k/mois contre local loué 60–150 k) et le fonds de roulement (délai de paiement) |
| Chemin critique | 9.1 qualification agence et hôtel + 6.5 autorisation du site → 5.2 conservation → 5.3 atelier et froid → 6.4 déclaration CHSP → 5.5 production à blanc → 8.4 / 9.4 premières ventes et remises |
| Must (MoSCoW) | Lots 1, 2, 4, 5, 6, 7, 8, 9 (9.1–9.5), 11.1, 12, 13.1, 14 |
| Should | 10.2 Maraa, 10.3 aéroport ou lobby, 13.2–13.3, 4.5 dégustation, 15 |
| Could | 7.4 inter-îles, 9.6 excursions, 5.6 machine |
| Won't (ce projet) | Bouteille, hôtels co-marqués en exécution, digital, export, grande distribution, vente en ligne, cocoteraie en propre, charbon de bourre, point de vente permanent |
