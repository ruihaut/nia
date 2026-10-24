# Matrice des risques — NĪĀ, étapes 1 et 2 (et préparation des étapes 3 et 4)

> v1 du 2026-10-24. Consolide les annexes A4 (R01–R19), A9 (R20–R29), les risques du collègue et ceux de l'étape 1 (vente au détail à la pointe Vénus). Échelles : probabilité P et impact I de 1 à 5 ; score = P × I ; zone rouge ≥ 15, orange 9–14, verte ≤ 8. Coûts en XPF, estimés. Stratégies : **Évit** évitement · **Mit** mitigation · **Trans** transfert · **Acc** acceptation · **Esc** escalade. Revue mensuelle et à chaque gate ; propriétaire = qui porte la réponse. Une opportunité est un risque positif : elle a sa section.

## 1. Filière amont (cocos)

| Id | Risque | Cause | Conséquence | P | I | Score | Coût si survient | Stratégie | Réponse | Propriétaire | Déclencheur | Étape |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R04 | Cocoteraie hors stade nīā ou irrégulière | Sélection sur l'arbre coûteuse, producteur orienté coprah, un seul fournisseur | Rejets, ruptures, perte du client | 4 | 4 | 16 | 30–90 k/mois de rejets ; 150–400 k de revenu perdu | Mit + Trans | Deux producteurs ; fiche nīā coécrite ; check-list et droit de refus ; prime de sélection 20–50 ; essai de 50 cocos triés | Chef de projet, supply-analyst | Rejet > 20 % sur deux livraisons ; un seul fournisseur en janvier | 1–4 |
| R30 | Prix d'achat au-dessus de 200 XPF | Rareté des cocos jeunes triés, concurrence du lait de coco et du coprah subventionné (165 XPF/kg) | Marge écrasée, surtout en excursion | 3 | 4 | 12 | −0,35 M de VAN par 24 XPF d'écart | Mit | Trois devis écrits ; contrat de volume contre prix stable ; seconde source ; cocos bruts d'une île à fret gratuit | supply-analyst | Devis > 200 | 1–3 |
| R18 | Qualité gustative variable (variété, stade mal calibré) | Pas de critère mesurable (Brix, âge du régime) | Le touriste ne perçoit pas la différence ; argument premium perdu | 3 | 3 | 9 | Réfractomètre 10–30 k ; perte de l'argument | Mit | Réfractomètre et grille de stade à réception ; goûter chaque lot ; deux cocoteraies comparées | supply-analyst | Brix ou goût variable entre deux lots | 1–4 |
| R31 | Ravageurs ou maladie dans la cocoteraie partenaire (Oryctes, Brontispa) | Statut inconnu en Polynésie | Source indisponible | 2 | 3 | 6 | Changement de source, 1–2 semaines | Acc + Mit | Deux sources sur deux zones ; question à la DAG | supply-analyst | Signalement DAG | 1–4 |
| R32 | Saisonnalité de la production de cocos jeunes | Creux saisonnier non connu | Rupture en haute saison touristique | 2 | 4 | 8 | Perte de 2–4 semaines de ventes | Mit | Demander la variation mensuelle à deux producteurs ; stock tampon limité par la DLC | supply-analyst | Producteur qui annonce un creux | 1–2 |

## 2. Production, conservation, hygiène

| Id | Risque | Cause | Conséquence | P | I | Score | Coût si survient | Stratégie | Réponse | Propriétaire | Déclencheur | Étape |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | Conservation du coco taillé < 5 jours au froid | Brunissement de la bourre, fermentation au point de coupe ; température mal choisie (chilling injury à 4 °C signalé) | Flux tendu quotidien, pertes, canal agences non opérable sous 3 jours | 4 | 5 | 20 | 0,3–0,65 M de surcoût sur 6 mois | Mit puis Évit | Lot test dès la première quinzaine à 2–4 °C, 6–8 °C et en réfrigérateur d'hôtel ; découpe à J−1 ; film ; stock ≤ 3 jours ; DLC prudente | process-engineer | Brunissement avant J5 | 1–3 |
| R10 | Découpeur introuvable ou instable | Volume 2–3 h/jour, geste technique et dangereux | Le binôme coupe ; qualité variable | 3 | 4 | 12 | Formation 50–100 k ; jour sans livraison 10–20 k | Mit | Trois candidats testés sur 10 cocos ; deux personnes formées ; rémunération à la pièce lisible | chef de projet | Aucun candidat à 20 cocos/h sans blessure en janvier | 1–3 |
| R11 | Accident de travail à la découpe | Lames, bourre dure, cadence | Arrêt, responsabilité, image | 2 | 5 | 10 | 100 k–1 M | Trans + Mit | Gants anti-coupure, plan de travail stable, outil dédié, procédure écrite, assurance selon statut | chef de projet | Avant la première séance rémunérée | 1–4 |
| R12 | Incident sanitaire chez un consommateur | Froid rompu, DLC dépassée, hygiène de découpe, trois mains successives | Fin de la marque avant d'exister ; réclamation via l'agence ou l'hôtel | 2 | 5 | 10 | 0,5–3 M ; perte des relations | Mit + Trans | Plan de maîtrise sanitaire, DLC courte, étiquetage par lot, consigne de froid remise au client, RC produit couvrant l'intoxication, retrait de lot | operations-director | Toute réclamation ou coco fermenté | 1–4 |
| R33 | Protocole de découpe non reproductible (temps > 3 min, perte > 10 %) | Geste non maîtrisé, outils inadaptés | Coût de revient qui explose, cut irrégulier devant le client | 3 | 3 | 9 | +50–100 XPF par coco | Mit | Trois lots de 20 mesurés, demi-journée avec un vendeur expérimenté, outils fixés, photo de référence | process-engineer | > 3 min ou > 10 % après 60 cocos | 1–2 |
| R34 | Panne du froid unique | Armoire d'occasion sans SAV, coupure électrique | Lot perdu, livraison manquée | 2 | 4 | 8 | 20–50 k par lot | Mit | SAV local, alarme de température, glacières et plaques en secours, second réfrigérateur dès que possible | process-engineer | Alarme | 1–3 |

## 3. Réglementaire et autorisations

| Id | Risque | Cause | Conséquence | P | I | Score | Coût si survient | Stratégie | Réponse | Propriétaire | Déclencheur | Étape |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R05 | Délai ou refus du CHSP | Déclaration d'établissement non anticipée, local non conforme, DLC à justifier | Première vente repoussée | 3 | 5 | 15 | 0,3–1 M (1–3 mois de charges) | Mit + Esc | Rendez-vous CHSP en semaine 2 ; préconisations « denrées végétales » traduites en travaux chiffrés ; cuisine partagée déjà conforme | operations-director | Pas de réponse écrite en janvier | 1–4 |
| R35 | Refus de la commune de Mahina (pointe Vénus) ou de Paea (Maraa) pour l'occupation du domaine public | Site protégé, vendeurs présents, propreté | Pas de stand ; étape 1 impossible sur ce site | 3 | 5 | 15 | Étape 1 décalée ou déplacée | Évit + Mit | Rendez-vous mairie avant toute vente ; option « glacière dans le bus » sans installation ; autre site (Vaipahi, marae d'Arahurahu) ; associer un vendeur présent | chef de projet | Refus ou silence à quatre semaines | 1 |
| R36 | Vente ambulante non conforme (patente, caisse, CHSP) | Formalités ignorées | Amende, fermeture, image | 3 | 4 | 12 | 50–300 k | Mit | Patente et déclaration avant la première vente ; caisse ou terminal de paiement ; CHSP vente ambulante | chef de projet | Première vente sans récépissé | 1 |
| R37 | Refus du gestionnaire de l'aéroport de distribuer dans le terminal ; liquides en correspondance | Règles aéroportuaires | Format aéroport impossible | 3 | 3 | 9 | Format abandonné, pas de coût direct | Évit | Format aéroport en Should seulement ; remise au dépôt de l'agence ou au lobby de l'hôtel ; cibler les touristes qui dorment à Tahiti | business-director | Réponse du gestionnaire | 2 |
| R38 | Biosécurité : transfert de végétaux entre îles encadré | Ravageurs du cocotier | MOTU et Moorea bloqués ou retardés | 2 | 3 | 6 | Extension décalée | Mit | Question à la Direction de la biosécurité avant toute expédition | operations-director | Réponse défavorable | 2–4 |
| R19 | Statut du découpeur à la tâche requalifié | Travail dissimulé | Redressement | 2 | 4 | 8 | 200 k–1 M | Mit + Esc | Statut clarifié avant le premier paiement (CPS, patente ou prestation de la cocoteraie) | chef de projet | Avant le premier paiement | 1–4 |
| R39 | Marque NĪĀ non protégeable (nom commun tahitien) | Nom descriptif | Copie du nom | 3 | 3 | 9 | Perte d'exclusivité du nom | Mit | Vérification avant dépôt ; protéger le logo et la présentation ; pas de dépôt avant la première facture | brand-director | Avis de l'INPI ou du conseil | 1–4 |
| R40 | TVA et régime fiscal mal anticipés | Taux applicable incertain (5, 13 ou 16 %) | Prix HT mal posé, marge rognée | 2 | 3 | 6 | 5–16 % du CA | Mit | Question à la DICP ; prix annoncés HT | financial-modeler | Création de l'entité | 1–2 |

## 4. Logistique et froid

| Id | Risque | Cause | Conséquence | P | I | Score | Coût si survient | Stratégie | Réponse | Propriétaire | Déclencheur | Étape |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R24 | Horaires de nuit, vols retardés, 7 jours sur 7 | Arrivées long-courriers le soir et la nuit | Épuisement, coco tiède, remise manquée | 4 | 4 | 16 | Relais du soir 80–200 k/mois ou arrêt | Évit + Mit | « Pas de nuit chez NĪĀ » : découpe la veille, livraison en fin de journée au dépôt de l'agence ou à la chambre froide de l'hôtel ; relais à la tâche | operations-director | Hôtel ou agence sans froid tampon | 2 |
| R41 | Bus en retard, itinéraire changé, stop raccourci | Aléas des tours | Coco trop longtemps hors du froid, invendus | 3 | 3 | 9 | 10–40 k/mois | Mit + Acc | Planning partagé avec l'agence ; règle « coco jeté au-delà de X heures hors froid » ; cocos repris | chef de projet | Deux retards dans la semaine | 1–2 |
| R42 | Pic d'un gros paquebot | 500–2 000 passagers à terre le même jour | Demande non servie ou surproduction perdue | 3 | 3 | 9 | 20–60 k par escale | Mit | Seulement les bus des agences partenaires ; plafond par jour ; calendrier des escales connu des mois à l'avance | business-director | Escale > 1 000 passagers | 1–2 |
| R09 | Fret inter-îles payant ou froid rompu (Moorea, MOTU) | Arrêté 1586 CM : produits non transformés, îles → Tahiti ; coco paré probablement « transformé » | Marge Moorea négative, qualité dégradée | 4 | 4 | 16 | 15–80 k/mois | Mit + Évit | Fret compté plein ; demande au cas par cas à la DGAE ; sonde sur un trajet réel ; découpe sur l'île ; MOTU en Could | operations-director | Silence ou refus DGAE ; > 8 °C à l'arrivée | 2–4 |
| R43 | Rotation de cargo annulée (MOTU) | Météo, planning | Cuvée MOTU indisponible | 3 | 2 | 6 | Pas de coût direct | Acc | MOUʻA reste la base ; MOTU annoncé comme édition | supply-analyst | Annulation | 4 |
| R14 | Météo et houle | Saison des pluies novembre–avril | Excursions annulées, stock périssable | 3 | 3 | 9 | 10–40 k/mois | Acc + Mit | Stock ≤ 3 jours ; commande confirmée la veille ; 5–10 % de pertes budgétées | operations-director | Deux annulations la même semaine | 1–2 |
| R44 | Glacières perdues ou non rendues | Trois mains, bus, hôtels | Coût récurrent | 3 | 2 | 6 | 10–15 k par glacière | Mit | Glacières marquées, consigne, inventaire hebdomadaire | chef de projet | Deux glacières manquantes | 1–2 |

## 5. Commercial : étape 1, vente au détail à la pointe Vénus

| Id | Risque | Cause | Conséquence | P | I | Score | Coût si survient | Stratégie | Réponse | Propriétaire | Déclencheur | Étape |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R45 | Le touriste ne paie pas 800 XPF un coco | Ancrage à 200 XPF, vendeurs locaux à côté, arrêt de 15 minutes | Ventes < 100 par semaine, stock perdu | 4 | 4 | 16 | Invendus 20–40 % ; étape 1 non rentable | Mit | Tester 600 / 800 sur deux escales ; froid, diamond cut, ouverture propre, carte et origine visibles ; dégustation ; paiement par carte | chef de projet, market-scout | < 50 ventes sur une escale à 3 bus | 1 |
| R46 | Conflit avec les vendeurs locaux déjà présents | Concurrence frontale sur leur site | Blocage par la commune, image | 3 | 4 | 12 | Étape 1 arrêtée | Évit | Les associer (option B : un vendeur local garde le stock et sert contre commission) ; ne pas s'installer à côté d'eux | chef de projet | Plainte ou tension dès la première escale | 1 |
| R47 | Dérive vers un point de vente permanent | L'étape 1 marche un peu | Concurrence durable avec les vendeurs, dérive hors de la vision (pas de B2C permanent) | 3 | 3 | 9 | Coût d'opportunité : l'étape 2 | Mit | Durée écrite (un à trois mois), jours de paquebot seulement, critère de sortie vers l'étape 2 | sponsor, challenger | Troisième mois sans contact d'agence | 1 |
| R48 | Encaissement, monnaie, vol, pluie sur le stand | Vente de rue | Pertes, journée perdue | 3 | 2 | 6 | 5–20 k par incident | Mit | Terminal de paiement, fonds de caisse, abri, deux personnes aux heures de pointe | chef de projet | Premier incident | 1 |
| R49 | Correspondances : passagers de croisière qui ne peuvent pas emporter de liquide ou n'ont pas le temps | Arrêt court, règles du bateau | Cocos non bus, abandonnés | 3 | 3 | 9 | Pertes, déchets sur le site | Mit | Servir à boire sur place, coque reprise immédiatement, paille ; carte « déposez-le au point NĪĀ » | chef de projet | Cocos abandonnés comptés | 1 |

## 6. Commercial : étape 2, agences réceptives et hôtels

| Id | Risque | Cause | Conséquence | P | I | Score | Coût si survient | Stratégie | Réponse | Propriétaire | Déclencheur | Étape |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R20 | Dépendance à une seule agence et à un seul contact (rôle terrain, pas décideur) | Canal né d'un contact | Canal fermé du jour au lendemain ; 80–100 % du CA | 4 | 5 | 20 | 0,8–1,8 M (3–6 mois de charges) | Mit | Entretien décideur sous trois semaines ; seconde agence ou hôtel en direct avant octobre 2027 ; excursions en repli daté | chef de projet, business-director | Pas de décideur rencontré au 15 décembre | 2 |
| R21 | Commission, remise ou exclusivité exigée | Habitudes des réceptifs | Prix net < coût complet ; hôtel en direct interdit | 4 | 4 | 16 | 100–250 XPF/coco ; tout le canal hôtel | Mit | Prix net ≥ 590 ou pas de lancement ; pas d'exclusivité qui interdise l'hôtel | business-director | Commission > 10 % demandée | 2 |
| R27 | Décision 2027 déjà prise avec les tour-opérateurs | Brochures négociées un an à l'avance | Pas d'inclusion payée avant 2028 | 4 | 4 | 16 | 12 mois de décalage du cash du canal | Mit | Dates de clôture demandées au premier entretien ; test financé sur la marge de l'agence ; commande hôtel | business-director | Réponse « brochures 2028 » | 2 |
| R23 | Le coco est posé, pas bu : collier, welcome drink, fatigue, nuit de transit | Arrivée après 12–22 h de voyage | Pas d'effet perçu ; l'agence arrête à trois mois | 4 | 4 | 16 | Gaspillage 20–40 % ; 0,3–0,6 M | Mit | Vingt remises observées avant le pilote ; remise au lobby après le check-in ou au premier stop, jamais à l'aéroport ; moment alternatif (chambre, petit-déjeuner) | market-scout | < 70 % de cocos bus sur 20 remises | 2 |
| R22 | L'agence ou l'hôtel teste puis internalise | Barrière technique faible ; l'hôtel a une cuisine et un froid | NĪĀ a servi de preuve de concept gratuite | 3 | 5 | 15 | 0,5–1 M | Mit | Valeur portée par le stade, la régularité, l'origine, le nom et la collecte, pas par la découpe | business-director | Question « où achetez-vous, quel outil ? » à la deuxième rencontre | 2–3 |
| R26 | Exigences d'un hôtel cinq étoiles (pièces, présentation, audit) | Standards de chaîne | 2–3 mois de délai, coûts de présentation | 3 | 4 | 12 | 100–400 k ; 0,3–0,9 M de décalage | Mit | CHSP dès la semaine 2 ; liste des pièces obtenue à l'entretien ; marque minimale | operations-director | Liste de pièces hors de portée | 2–3 |
| R50 | Les guides ne jouent pas le jeu (rituel, hygiène, collecte) | Geste imposé par le patron | Coco mal servi, coques abandonnées | 3 | 4 | 12 | Perte du client | Mit | Patron et guide signent ensemble ; fiche de 15 minutes ; formation ; les nommer dans les retours | chef de projet | Première livraison sans collecte | 2 |
| R51 | Les hôtels refusent la reprise des cocos vides (fourmis, odeur, poids) | Déchet lourd et humide | Coques abandonnées, image | 3 | 3 | 9 | Collecte à organiser : 10 XPF/coco | Mit | Accord de reprise avec un ou deux hôtels ; sac de collecte dans le bus ; compost chez les producteurs | operations-director | Refus de deux hôtels | 2–3 |
| R02 | Non-adoption des opérateurs d'excursion (seconde cible) : le guide qui coupe est le spectacle | Coco perçu gratuit | Pas de client en appoint | 4 | 4 | 16 | Marché secondaire perdu | Évit | Viser les opérateurs sans « numéro coco » ; vendre stade, froid, régularité | market-scout | > 50 % des entretiens « on le fait nous-mêmes » | 2 |
| R28 | Dispersion du binôme entre plusieurs canaux | Détail, agences, hôtels, excursions en même temps | Aucun client signé à temps | 3 | 4 | 12 | 1–2 mois de retard | Mit | Une seule cible prospectée à la fois ; étapes datées ; MoSCoW | sponsor, challenger | Deux prospections ouvertes la même semaine | 1–2 |

## 7. Finances et financement

| Id | Risque | Cause | Conséquence | P | I | Score | Coût si survient | Stratégie | Réponse | Propriétaire | Déclencheur | Étape |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R03 | Coût complet > prix accepté | Froid, glace, tournée, pertes, présentation non comptés | Vente à perte | 4 | 4 | 16 | 100–375 k/mois | Mit | Coût complet relevé avant tout prix ; devis à trois niveaux ; marge ≥ 150 ou on ne lance pas | financial-modeler | Marge < 150 dans le modèle v1 | 1–3 |
| R07 | Trésorerie épuisée avant la première facture | Froid et local trop tôt, paiement à 30–60 jours | Arrêt faute de cash | 3 | 5 | 15 | Perte de l'apport, 2–5 M | Mit | Plan de trésorerie avec seuil d'arrêt ; froid d'occasion ou loué ; pas de chambre froide sans lettre d'intention ; acompte d'agence | chef de projet, financial-modeler | Dépenses > 40 % de l'apport sans commande | 1–2 |
| R52 | Délai de paiement des agences à 60 jours | Pratique du secteur | Point bas −2,35 M au lieu de −1,87 M | 3 | 4 | 12 | −0,48 M de besoin de fonds | Mit | Acompte d'un mois contre 5 % de remise ; facturation hebdomadaire ; microcrédit | financial-modeler | Conditions de paiement annoncées | 2 |
| R08 | Sponsor non trouvé | Projet trop petit pour un investisseur, trop risqué pour un prêteur | Extension et étape 3 non financées | 4 | 3 | 12 | Décalage 6–12 mois | Mit + Acc | Dossier sur preuves ; élargir la notion de sponsor (cocoteraie, hôtel, aides du Pays) ; le palier 1 doit tenir sur l'apport | business-director | Aucun rendez-vous obtenu en janvier | 2–3 |
| R53 | Le modèle ne tient pas sans aides publiques | Coûts fixes polynésiens | Dépendance aux subventions | 2 | 4 | 8 | Fragilité structurelle | Mit | Scénario « sans aides » dans le business case (H10) | financial-modeler | Modèle v1 | 1–3 |
| R54 | Coûts cachés : temps commercial, formation des guides, cocos préparés pour rien, glacières perdues, pénalités de contrat | Non budgétés | Marge réelle inférieure | 4 | 2 | 8 | 10–20 % de la marge | Acc + Mit | Comptabilité par lot ; ligne « imprévus » 10 % | financial-modeler | Écart > 10 % au tableau de bord | 1–2 |

## 8. Équipe et organisation

| Id | Risque | Cause | Conséquence | P | I | Score | Coût si survient | Stratégie | Réponse | Propriétaire | Déclencheur | Étape |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R06 | Épuisement ou dispersion du binôme (terrain, nuit, digital) | Tout repose sur deux personnes non rémunérées | Retards, erreurs qualité, arrêt | 3 | 5 | 15 | Arrêt : 1–3 M d'apport ; retard : 150–300 k/mois | Mit | Journal de temps, terrain ≥ 50 % ; relais à la tâche avant janvier ; « pas de code avant la première facture » | sponsor, challenger | Terrain < 50 % deux semaines de suite | 1–4 |
| R55 | Désaccord ou indisponibilité d'un des deux membres du binôme | Rôles non écrits, vie professionnelle | Projet bloqué | 2 | 5 | 10 | Arrêt | Mit | Rôles écrits dans la charte (sponsor, PO, chef de projet), pacte simple, décisions tracées | sponsor | Deux revues sans décision | 1–4 |
| R56 | Le métier manque (filière, agroalimentaire, hôtellerie) | Profils tech / produit | Angles morts : hygiène, cycle de vente, négociation producteur | 4 | 3 | 12 | Erreurs de 1–3 mois | Mit | Associé terrain ou mentor ; une semaine chez un vendeur de coco ou un producteur ; demander, ne pas supposer | chef de projet | Première erreur de métier coûteuse | 1–3 |
| R16 | Le palier 1 devient une fin en soi | Le détail ou l'accueil marche un peu | Étapes 3 et 4 repoussées ; la finalité n'est plus servie | 3 | 3 | 9 | Coût d'opportunité : la finalité | Mit | Gate G4 ; MoSCoW ; faisabilité de l'eau extraite au plus tard en juillet 2027 ; KPI « commandes hôtel en propre » | sponsor, challenger | Neuvième mois sans étude de l'étape suivante | 1–2 |
| R15 | Marque prématurée (temps et budget en identité avant le produit) | Compétence produit du binôme | Rien de vendable, marque à refaire | 3 | 3 | 9 | 100–300 k ; 1–2 mois | Évit | Un marquage et trois phrases avant la première facture ; séquence : protocole avant marque | DG, challenger | Livrable de marque validé avant le protocole | 1–2 |
| R57 | Soutenance : démo ratée, temps dépassé, chiffres contestés | Pas de répétition, cocos indisponibles | Note, crédibilité | 3 | 3 | 9 | — | Mit | Répéter en chronométrant ; plan B de démo (photo, main levée) ; dire que les chiffres sont estimés et comment on les relève | binôme | J−3 sans répétition | Soutenance |

## 9. Marque, marché, externe

| Id | Risque | Cause | Conséquence | P | I | Score | Coût si survient | Stratégie | Réponse | Propriétaire | Déclencheur | Étape |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R17 | Concurrence réactive (producteur, vendeur, embouteilleur local : Rotui, Brasserie de Tahiti) | Barrière faible | Prix tirés vers le bas | 2 | 3 | 6 | 100–150 k/mois | Acc | Accepter : la défense est la régularité, le stade, la relation et le nom ; pas de dépense de protection avant la première facture | business-director | Perte de deux clients au profit d'un copieur | 1–4 |
| R58 | Hanahana Tours ou un réceptif intègre lui-même un coco à son accueil VIP | Créneau « collier + boisson + serviette » déjà occupé | Place prise | 2 | 4 | 8 | Canal accueil plus dur | Mit | En faire un partenaire ou un client plutôt qu'un concurrent | business-director | Offre concurrente repérée | 2 |
| R59 | Appropriation culturelle mal perçue (nom tahitien, mots motu et mouʻa en décoration) | Ton, lexique approximatif | Rejet par la communauté, image | 2 | 4 | 8 | Marque à refaire | Évit | Lexique validé par un locuteur puis le Fare Vānaʻa ; fierté, pas exotisme ; producteurs payés correctement et on le dit | brand-director | Première critique publique | 1–4 |
| R60 | Promesse de terroir (Motu / Mouʻa) non tenue au goût | Aucune preuve de différence gustative | Confusion, perte de crédibilité au premium | 3 | 3 | 9 | Gamme à retirer | Évit | Aucune promesse gustative avant un test triangulaire à l'aveugle ; origines dites comme des lieux | brand-director | Test triangulaire négatif | 4 |
| R61 | Réglementation ou soutien public qui change (fret agricole, interdiction d'import, prix du coprah) | Décisions du Pays | Modèle à refaire | 2 | 3 | 6 | Variable | Acc | Veille DGAE et DAG ; ne pas construire le modèle sur une aide | DG | Arrêté modificatif | 2–4 |
| R13 | Saisonnalité : pilote construit en basse saison, lancé à l'entrée de la haute saison | Calendrier novembre–avril | Signature décalée d'une saison | 3 | 3 | 9 | 0,6–1,5 M de charges en attente | Mit | Signer en février–mars pour démarrer en avril ; demander la fenêtre de décision à chaque client | business-director | « Revenez après la saison » | 1–2 |

## 10. Étapes 3 et 4 (à instruire quand elles s'ouvrent)

| Id | Risque | Cause | Conséquence | P | I | Score | Réponse prévue | Étape |
|---|---|---|---|---|---|---|---|---|
| R62 | Le logo de l'hôtel efface NĪĀ | Co-marquage mal cadré | La marque disparaît au moment où elle entre en CHR | 3 | 4 | 12 | « Hôtel × NĪĀ » ou « Sélection NĪĀ pour l'Hôtel X » contractuel, comme pour un vin | 3 |
| R63 | Durée de vie de l'eau extraite insuffisante sans traitement | Eau de coco fraîche : 48 h non pasteurisée | Pas de bouteille sans process ou chaîne du froid lourde | 4 | 5 | 20 | Faisabilité dès juillet 2027 : pasteurisation douce, HPP, froid ; agréments | 4 |
| R64 | Investissement du premium hors de portée (20–50 M) | Extraction, conditionnement, laboratoire | Étape 4 non financée | 3 | 4 | 12 | Sponsor, banque sur bilan de deux cycles, aides à l'agro-transformation | 4 |
| R65 | Entrée d'un industriel local sur l'eau de coco premium | Marché prouvé par NĪĀ | Fenêtre refermée | 3 | 4 | 12 | Vitesse, relations CHR, origine et sélection comme différenciation | 3–4 |

## 11. Matrice probabilité × impact

```
Impact →           1            2              3                          4                                 5
Probabilité ↓
5                  –            –              –                          –                                 –
4                  –            R54            R08                        R03 R04 R09 R21 R23 R24 R27      R01 R20 R63
                                                                          R02 R45
3                  –            R43 R44 R48    R13 R14 R15 R16 R18 R33    R10 R26 R28 R30 R36 R41 R50      R05 R06 R07 R22 R35
                                               R37 R39 R42 R47 R49 R51    R52 R56 R60 R62 R64 R65
                                               R57
2                  –            –              R31 R17 R40 R61            R19 R32 R34 R38 R53 R58 R59      R11 R12 R55
1                  –            –              –                          –                                 –
```

**Zone rouge (≥ 15), par ordre** : R01 conservation (20) · R20 dépendance à une agence (20) · R63 durée de vie de l'eau extraite (20, étape 4) · R03 coût > prix (16) · R04 cocoteraie (16) · R09 fret inter-îles (16) · R21 commission (16) · R23 coco posé (16) · R24 nuit (16) · R27 décision 2027 (16) · R02 excursions (16) · R45 le touriste ne paie pas 800 (16) · R05 CHSP (15) · R06 binôme (15) · R07 trésorerie (15) · R22 internalisation (15) · R35 refus de la commune (15).

**Les onze risques rouges des étapes 1 et 2 se traitent avec huit actions**, moins de 150 k XPF et neuf semaines : lot test de conservation à deux températures ; rendez-vous mairie de Mahina ; rendez-vous CHSP ; entretien terrain puis décideur de l'agence avec prix dit à haute voix et dates de clôture ; entretien de deux ou trois hôtels ; devis de trois cocoteraies pour 50 cocos triés ; vingt remises et deux escales de vente observées à 600 / 800 ; plan de trésorerie avec seuil d'arrêt. R06 et R07 relèvent de la discipline du binôme.

## 12. Ce qu'on choisit de ne pas couvrir à 100 %

| Risque | Couverture | Pourquoi |
|---|---|---|
| R17 concurrence réactive, R58 Hanahana | Non couverts | Si un copieur gagne, la valeur n'était que dans la découpe : information utile pour la suite ; aucune dépense de protection avant la première facture |
| R14 météo, R41 bus en retard, R54 coûts cachés | Acceptés, budgétés | 5–10 % de pertes et 10 % d'imprévus dans le modèle ; un stock tampon aggraverait R01 |
| R11 accident, R12 sanitaire | Transfert minimal | Assurance et protocole ; pas de laboratoire aux normes industrielles au volume du pilote |
| R09 inter-îles, R43 cargo | Partiels | Tahiti d'abord ; rien d'acheté pour Moorea ou MOTU avant la réponse sur le fret et un test de froid |
| R16 dérive | Un seul garde-fou | La date de juillet 2027 pour l'étude de l'étape suivante ; dériver un trimestre est acceptable si c'est décidé, pas subi |
| R08 sponsor | Partiel | Le palier 1 doit tenir sur l'apport ; le sponsor sert l'accélération |
| R13 saisonnalité | Partiel | La date de départ ne bouge pas ; on accepte le risque d'un décalage d'une saison |

## 13. Opportunités (risques positifs)

| Id | Opportunité | Probabilité | Bénéfice | Action pour la saisir | Coût |
|---|---|---|---|---|---|
| O1 | L'hôtel comme client direct du geste d'accueil, l'agence comme prescripteur | 4 | Résout R20, R21, R24, R22 ; décideur de l'étape 3 | Le proposer dès les entretiens hôtels | 0 |
| O2 | Cocos bruts d'une île productrice à fret pris en charge par le Pays (arrêté 1586 CM) | 4 | Approvisionnement élargi, jusqu'à +0,59 M de VAN | Lexpol, DGAE, carte CAPL ou RCS, une cocoteraie desservie | 0–20 k |
| O3 | Sous-produits : cocos déclassés en glaces (glacier partenaire), bourre en compost chez les producteurs, coques | 3 | Zéro gaspillage, récit, revenu marginal | Un preneur identifié ; Buy, pas Make | 0 |
| O4 | La cocoteraie découpe elle-même sous protocole | 3 | Supprime local, découpeur, transport ; sponsor industriel naturel | Poser la question au premier entretien ; essai sur 50 cocos | 0 |
| O5 | L'agence prescrit NĪĀ à ses opérateurs d'excursion sous-traitants | 3 | Seconde cible ouverte sans prospection | Le demander au décideur | 0 |
| O6 | Mesures transférables au premium (Brix, rendement en eau, courbe de dégradation, relation producteurs) | 5 | Réduit les risques de l'étape 4 | Protocole du lot test conçu pour mesurer aussi l'eau et le Brix | 10–30 k |
| O7 | Visibilité gratuite : coco nommé et photographié, #NĪĀ | 3 | Notoriété avant le CHR | Carte, QR code, une phrase du guide | 5–10 XPF/coco |
| O8 | Soutien du Pays à la diversification hors coprah (la DAG veut diffuser des cocotiers nains pour l'eau) | 2 | Crédibilité, aide à l'équipement | Candidater avec une première facture | Temps |
| O9 | Une agence ou un hôtel préfinance le pilote (acompte, glacières) | 3 | Point bas réduit de 0,5–0,7 M | Le proposer contre 5 % de remise | 5 % |
| O10 | Vendeur local associé sur le site (option B) | 3 | Résout R46, R35 en partie ; valeur partagée | Commission ; formation | 10 % du prix |
