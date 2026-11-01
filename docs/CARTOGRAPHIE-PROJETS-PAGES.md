# Cartographie projets GitHub → Pages Facebook — préparation pour validation de Matt

Date : 2026-11-01 (~15:35 EST). Mission ordonnée par Matt (15:31 EST) : 1 dépôt GitHub = 1 projet = 1 client ; chaque projet doit avoir SA Page Facebook. **Préparation seulement — aucune Page créée, renommée ou recyclée.** Matt valide le tableau (bons / pas bons) et donne les courriels manquants ; la vague 2 viendra après son OK. Signé : Taktak.

## Note d'avant (état lu avant de commencer)

- Registre (section Facebook, tête du fichier) : liste des 57 Pages livrée à Matt ~15:30 EST (Drive Opérations 1X-nBkkg5QJdH5SR2avhLTNOf5yfEMoHO) ; retraits Casa Lach vérifiés 13:32 (Goose) et 15:21 (Mikey Cross, Virginia Mac) ; inventaire Casa 13:12 (Casa gère 0 Page, 9 invitations en attente, candidates LOC Actif / Fdeals / Rent Auto / Poulet Poulet NDG).
- Liste des 57 Pages (fichier du 2026-11-01) : source = liste en direct du compte Matt TakaTak, pagination 19+20+18 = 57, recoupée 57/57 avec l'audit du 2026-10-31.
- Audit 57 Pages (2026-10-31, fenêtre 3c8da357) : 38 déjà complètes · 2 ajoutées · 6 en attente · 11 bloquées (2 vérification de compte : EYEClean.ca, Takatak MUSIC ; 9 classiques bloquées au mot de passe : Qmaps.ca, Rent Auto Canada, MIMT, Fdeals.ca QC, Casa Lach, Leopard Lake Gold Corp., Taxi Chambly, Emploi Direct, LOC Actif). Hors portée : BP Taekwondo 1395058667296542, 0 personne assignée.
- Fichier maître « 00 » : 16 portefeuilles ouverts (takatak, Ooeuf Pitapita, AhM Verdun, takatak.ca, Rapide 2 Nette, Matthieu CubaResort, COMPLEXE HAVANA, Globe Telecom INC, Nutrition Shake Montréal Nord, Takatak INC, Gonflabe Zone, Estephanie Molina — 0 Page, Spray Foam Machine Canada, bardosh.ca, irqc.ca, Groupe Takatak — 0 Page).
- COMPANY-INFORMATION maître v3 (2026-10-31) : les 18 franchises et leurs courriels de marque (source des courriels restaurants du tableau).
- Captures de Matt (15:30) : conversation avec Umer Farooq (« Sir, please send me the links to all the pages ») ; on y voit une section « Deactivated Pages » avec **Miel Aissa — Not visible to the public — Activate** : une Page désactivée qui n'est PAS dans les 57. Matt signale des doublons et au moins une Page qui n'existe pas dans la liste livrée.
- Sweep A1 (2026-10-31, lecture seule) : 79 dépôts, 128 issues ouvertes. Base à compléter par l'inventaire vivant.

## Note pendant (travail fait, au fil de l'eau)

- Route GitHub qui a marché : `/opt/hatch/bin/github call-read-tool --name search_repositories --arguments-json '{"query":"user:takatakca","perPage":100,"page":1}'` → **total_count 81, 81 items retournés en une page**. Compte connecté : takatakca (get_me : 69 dépôts publics affichés au profil ; le total accessible via l'App = 81, publics + privés). A1 comptait 79 le 2026-10-31 → base complétée à **81 dépôts** (2 de plus : créations récentes ou comptage App élargi — non tranché, le vivant fait foi).
- Aucun champ `homepage` rempli sur les 81 dépôts (tous à None) ; descriptions rares. Les sites du tableau viennent donc du nom de domaine du dépôt (ex. BMBD.CA → bmbd.ca) et du fichier COMPANY-INFORMATION maître.
- Vérification ciblée de COMPANY-INFORMATION.md à la racine de 8 dépôts non-restaurants (EMPLOIDIRECT.CA, LOCACTIF.CA, qmaps, r2neet, mimt, BESOINAVOCAT.CA, ahmverdunca, Alkao.ca) via get_file_contents : aucun courriel de projet récupérable par cette route (fichier absent ou sans courriel). Les courriels non-restaurants connus viennent du fichier maître et des comptes connectés déjà au dossier.
- Croisement fait nom par nom entre les 81 dépôts et les 57 Pages (noms courants de la liste en direct, pas seulement l'audit — ex. 282744914913682 s'affiche aujourd'hui « Pizza Algérie Montréal -Saint Léonard- », l'audit la nommait « Traiteur Cook Montréal-Nord »).
- Règle appliquée : aucune Page déclarée morte depuis un fetch — les cas non prouvés sont marqués « à revérifier en session ».

## Tableau — 81 dépôts

| # | Projet (dépôt GitHub) | Nom de Page proposé | Site | Courriel (source) | Page Facebook actuelle | État | Page recyclable proposée |
|---|---|---|---|---|---|---|---|
| 1 | takatakca/pppmtl (public) | PPP Pizzeria | pppmtl.com | pppmtl.com@gmail.com (COMPANY-INFORMATION maître) | PPP Pizzeria Montréal -Saint Léonard- — https://www.facebook.com/483767435295888 (+ 2 autres, grappe §1) | DOUBLONS | — |
| 2 | takatakca/POPOULET.CA (public) | Po Poulet | popoulet.ca | popoulet.ca@gmail.com (maître) | Po Poulet Montreal -Notre Dame De Grâce- — https://www.facebook.com/110497128431808 (+ 2 autres, grappe §1) | DOUBLONS | — |
| 3 | takatakca/OOEUF.CA (public) | O'oeuf déjeuner | ooeuf.ca | ooeuf.ca@gmail.com (maître) | OOEUF Montréal -Notre Dame de Grâce- — https://www.facebook.com/102770028041467 (+ 2 autres, grappe §1) | DOUBLONS | — |
| 4 | takatakca/PIPITA.CA (public) | Pi Pita | pipita.ca | www.pipita.ca@gmail.com (maître) | Pi Pita Montréal -Notre Dame De Grâce- — https://www.facebook.com/108421598707603 (+ 1 autre, grappe §1) | DOUBLONS | — |
| 5 | takatakca/VIENNOISE.CA (public) | Gâteaux Montréal / Viennoise | viennoise.ca | viennoise.ca@gmail.com (maître) | Gâteaux Montréal -Notre Dame de Grâce- — https://www.facebook.com/104383909121946 (+ 2 autres, grappe §1) | DOUBLONS | — |
| 6 | takatakca/BMBD.CA (public) | BMBD — Crémière Bin Molle Bin Dure | bmbd.ca | bmbd.ca@gmail.com (maître) | Bin Molle & Bin Dure Montréal — https://www.facebook.com/102910359249848 (+ 1 autre, grappe §1) | DOUBLONS | — |
| 7 | takatakca/TACOMONTREAL.CA (public) | Taco Montréal | tacomontreal.ca | tacomontreal.ca@gmail.com (maître) | Taco Mexican Montreal-Notre Dame De Grâce- — https://www.facebook.com/1087556577773720 | OK | — |
| 8 | takatakca/OCREPE.CA (public) | O'Crêpe | ocrepe.ca | ocrepe.ca@gmail.com (maître) | O'Crêpe Montreal -Notre Dame De Grâce- — https://www.facebook.com/1082549831602471 (+ Hochelaga 265063723356018, 2e emplacement même marque) | OK | — |
| 9 | takatakca/NUTRISHAKE.CA (public) | Nutrition Shake | nutrishake.ca | nutrishake.ca@gmail.com (maître ; + nutritionshake.ca@gmail.com) | Nutrition Shake Montréal NDG — https://www.facebook.com/1426349433894036 (+ 2 autres, grappe §1) | DOUBLONS | — |
| 10 | takatakca/BOLON.CA (public) | Café Bolon | bolon.ca | cafebolon.ca@gmail.com (maître — officiel, à créer/connecter ; compte connecté actuel boloncafe.ca@gmail.com) | Bolon Café Montreal -Notre Dame De Grâce- — https://www.facebook.com/115999504787601 (+ 1 autre, grappe §1) | DOUBLONS | — |
| 11 | takatakca/MYTHOS2GO.CA (public) | Mythos & Go | mythosgo.ca (à commander) | mythosgo.ca@gmail.com (maître) | Mythos & Go Montreal-Notre Dame De Grâce- — https://www.facebook.com/100872212790454 | OK | — |
| 12 | takatakca/deli-aden-online (public) | Délices d'Aden | deliaden.ca (expiré 2026-10-17) | deliaden.ca@gmail.com (maître) | Les Délices D'Aden — https://www.facebook.com/108746045169773 | OK | — |
| 13 | takatakca/INNTIME.CA (public) | Pizza Inntime (INN TIME) | inntime.ca | inntime.ca@gmail.com (maître — PRÉSUMÉ, non confirmé) | INN TIME Montréal — https://www.facebook.com/216755544865350 | OK | — |
| 14 | takatakca/pitalibanais.ca (public) | Pita Libanais | pitalibanais.ca (à commander) | pitalibanais.ca@gmail.com (maître) | Pita Libanais Montréal NDG — https://www.facebook.com/1392282457302813 (+ Hochelaga 1436941379492537, 2e emplacement même marque) | OK | — |
| 15 | takatakca/POULETEXPRESS.CA (public) | Poulet Express | pouletexpress.ca (à commander) | pouletmtl@gmail.com (maître) | Poulet Express — https://www.facebook.com/1378509388684827 (grappe de confusion §1 avec Po Poulet / Poulet Poulet) | OK | — |
| 16 | takatakca/PIZZAALGERIE.CA (public) | Pizza Algérie | pizzaalgerie.ca (à commander) | pizzaalgerie.ca@gmail.com (maître) | Pizza Algérie Montréal -Saint Léonard- — https://www.facebook.com/282744914913682 (nom courant ; audit : « Traiteur Cook Montréal-Nord ») | OK | — |
| 17 | takatakca/PLACEDAFRIQUE.CA (public) | Place Afrique | placeafrique.ca (à commander) | placeafrique.ca@gmail.com (maître) | Place Afrique NDG — https://www.facebook.com/1832558563683426 (ex-Casa Lach ; il manque les Pages des autres emplacements — vague Casa 0/8, relance 2026-11-02) | OK | — |
| 18 | takatakca/DEJETDINNER.CA (public) | Déjeuner Montréal | dejeunermontreal.ca (à commander) | ooeufdejeuner@gmail.com (maître) | Déjeuner Montréal NDG — https://www.facebook.com/1372752575921168 | OK | — |
| 19 | takatakca/takatak-v1 (public) | TAKATAK (agence) | takatak.ca | takatak.ca@gmail.com (maître — courriel maître du groupe) | takatak.ca — https://www.facebook.com/257633186140512 (+ 1 autre, grappe §1) | DOUBLONS | — |
| 20 | takatakca/takatak (public) | TAKATAK (agence) — 2e dépôt du même projet que nº 19 | takatak.ca | takatak.ca@gmail.com (maître) | Takatak Marketing — https://www.facebook.com/109136031780822 (+ 1 autre, grappe §1) | DOUBLONS | — |
| 21 | takatakca/QUADROHOLDING (public) | Quadro Holdings / Groupe TAKATAK | — (holding, pas de site public propre) | takatak.ca@gmail.com (maître) | — (couverte par les Pages agence, grappe §1) | INTERNE — pas de Page propre attendue, à valider par Matt | — |
| 22 | takatakca/foodhubca (public) | Food Hub (plateforme du groupe) | — | takatak.ca@gmail.com (groupe — plateforme interne) | — | INTERNE — à valider par Matt | Fdeals.ca QC (si Matt veut une Page Food Hub) |
| 23 | takatakca/qmaps (public) | Qmaps.ca | qmaps.ca | À DONNER PAR MATT | Qmaps.ca — https://www.facebook.com/111850748533238 (658 abonnés, active) | OK | — |
| 24 | takatakca/mimt (public) | MIMT — Mobile Innovation Moderne Telecommunications | mimt.ca | À DONNER PAR MATT | Mobile Innovation Moderne Telecommunications — https://www.facebook.com/100728419421671 | OK | — |
| 25 | takatakca/mimtcaapp (public) | MIMT (app) — 2e dépôt du même projet que nº 24 | mimt.ca | À DONNER PAR MATT | Même Page que nº 24 | DOUBLONS (dépôt) | — |
| 26 | takatakca/r2neet (public) | Rapide 2 Nette | r2nette.ca | r2nette.ca@gmail.com (maître — adresses du groupe) | Rapide 2 Nette — https://www.facebook.com/1044118655779183 | OK | — |
| 27 | takatakca/on2goca (privé) | On2GO.ca | on2go.ca | on2go.ca@gmail.com (maître + compte connecté) | On2GO.ca — https://www.facebook.com/338588525994489 | OK | — |
| 28 | takatakca/EMPLOIDIRECT.CA (public) | Emploi Direct | emploiedirect.ca (à confirmer) | À DONNER PAR MATT | Emploi Direct — https://www.facebook.com/113484084668325 (200 abonnés, active) | OK | — |
| 29 | takatakca/LOCACTIF.CA (public) | LOC Actif | locactif.ca (à confirmer) | À DONNER PAR MATT | LOC Actif — https://www.facebook.com/101849556253698 (0 abonné ; invitation Casa en attente) | OK | — |
| 30 | takatakca/rentautoca (public) | Rent Auto Canada | rentautoca (domaine à confirmer) | À DONNER PAR MATT | Rent Auto Canada — https://www.facebook.com/106179458869094 (41 abonnés) | OK | — |
| 31 | takatakca/taxichambly (privé) | Taxi Chambly | — | À DONNER PAR MATT | Taxi Chambly — https://www.facebook.com/109232158603928 (749 abonnés, 234 avis, active) | OK | — |
| 32 | takatakca/ahmverdunca (public) | AhM Verdun | ahmverdun.ca (à confirmer) | À DONNER PAR MATT | AhM Verdun -Communauté — https://www.facebook.com/114816658382523 | OK | — |
| 33 | takatakca/GLOBESECURE.CA (public) | Globe Secure | globesecure.ca | À DONNER PAR MATT | Globe Secure -Sécurité- — https://www.facebook.com/108672858475187 | OK | — |
| 34 | takatakca/revers-canada-hope (public) | Revers Canada (MEV Québec) | reverscanada (à confirmer) | À DONNER PAR MATT | Revers Canada — https://www.facebook.com/114188131621111 | OK | — |
| 35 | takatakca/QCMEV.CA (public) | Revers Canada / MEV Québec — 2e dépôt du même projet que nº 34 | qcmev.ca | À DONNER PAR MATT | Même Page que nº 34 | DOUBLONS (dépôt) | — |
| 36 | takatakca/CUBARESORT.CA (public) | Cuba Resort Canada | cubaresort.ca (à confirmer) | À DONNER PAR MATT | Cuba Resort Canada — https://www.facebook.com/579261188604390 | OK | — |
| 37 | takatakca/promohavanaca (privé) | Complexe Havana / Havana Resort | promohavana.ca | promohavana.ca@gmail.com (courriel associé au compte Casa au dossier — à confirmer comme courriel du projet) | Halloween au Complexe Havana — https://www.facebook.com/1384551034735477 (Page saisonnière ; pas de Page principale « Complexe Havana » distincte relevée — à revérifier en session) | OK | — |
| 38 | takatakca/BESOINAVOCAT.CA (public) | Besoin Avocat | besoinavocat.ca | À DONNER PAR MATT | — | MANQUANTE | Poulet Poulet NDG (247671908438134) |
| 39 | takatakca/ACTIONAVOCAT.CA (public) | Action Avocat | actionavocat.ca | À DONNER PAR MATT | — | MANQUANTE | Restaurant Montréal-Nord (158024287401897) |
| 40 | takatakca/Alkao.ca (public) | Alkao.ca | alkao.ca | À DONNER PAR MATT | — | MANQUANTE | Café Bolon Montréal-Nord (263614826835067) |
| 41 | takatakca/CCC-CANADIEN-CONNEXION-CUBA (public) | Canadien Connexion Cuba | — | À DONNER PAR MATT | — | MANQUANTE | Taco Mexicano Montréal-Nord (278635711994147) |
| 42 | takatakca/cubafoodca (public) | Cuba Food | cubafood.ca (à confirmer) | À DONNER PAR MATT | — | MANQUANTE | Halloween au Complexe Havana (1384551034735477) — seulement si Matt détache Havana |
| 43 | takatakca/MIELAISSA.CA (public) | Miel Aissa | mielaissa.ca | À DONNER PAR MATT | — dans les 57 ; Page « Miel Aissa » vue DÉSACTIVÉE dans les captures de Matt (15:30) — à revérifier en session | MANQUANTE | Sa propre Page désactivée, à réactiver si Meta le permet (à revérifier en session) |
| 44 | takatakca/ocarinaspa (public) | Ocarina Spa | ocarinaspa.ca (à confirmer) | À DONNER PAR MATT | — | MANQUANTE | Fdeals.ca QC (101574182413130) |
| 45 | takatakca/DOMINICFINANCE (public) | Dominic Finance | — | À DONNER PAR MATT | — | MANQUANTE | Sédition MUSIC (1208836188985578) — à revérifier en session |
| 46 | takatakca/isexy (public) | iSexy | — | À DONNER PAR MATT | — | MANQUANTE | Surplus grappe Viennoise (§2) |
| 47 | takatakca/flexsca (public) | Flexs | flexs.ca (à confirmer) | À DONNER PAR MATT | — | MANQUANTE | Surplus grappe Nutrition Shake (§2) |
| 48 | takatakca/RAMASSEDEBRIS.CA (public) | Ramasse Débris | ramassedebris.ca | À DONNER PAR MATT | — | MANQUANTE | Surplus grappe Po Poulet (§2) |
| 49 | takatakca/festiiceca (public) | Festiice | festiice.ca (à confirmer) | À DONNER PAR MATT | — | MANQUANTE | Surplus grappe OOEUF (§2) |
| 50 | takatakca/droneair (public) | Drone Air | — | À DONNER PAR MATT | — | MANQUANTE | Surplus grappe BMBD (§2) |
| 51 | takatakca/co-work.ca-montreal-launch (privé) | Co-work Montréal | co-work.ca | À DONNER PAR MATT | — | MANQUANTE | Surplus grappe PPP (§2) |
| 52 | takatakca/cuban-coin-cad (privé) | Cuban Coin CAD | — | À DONNER PAR MATT | — | MANQUANTE | Surplus grappe Bolon (§2) |
| 53 | takatakca/CH4T (public) | — | — | À DONNER PAR MATT | — | INTERNE (outil) — à valider | — |
| 54 | takatakca/R2NETTEEMAIL (public) | — | — | À DONNER PAR MATT | — | INTERNE (outil courriel R2NETTE) — à valider | — |
| 55 | takatakca/takatak-automate (public) | — | — | À DONNER PAR MATT | — | INTERNE (automatisation) — à valider | — |
| 56 | takatakca/knowledgeAI (public) | Knowledge AI | — | À DONNER PAR MATT | — | INTERNE (base de connaissances ; dépôt public signalé au dossier sécurité) — à valider | — |
| 57 | takatakca/compassion-connect (privé) | Compassion Connect | — | À DONNER PAR MATT | — | INTERNE / projet tiers — à valider par Matt (client externe ?) | Surplus grappe Pi Pita (§2) si Matt le classe client |
| 58 | takatakca/SEOTAKATAK (public) | Tac Attack (SEO) | — | À DONNER PAR MATT | — | INTERNE (produit SEO de l'agence ; profil « Tac Attack » non ouvert — P17 en attente de Matt) — à valider | — |
| 59 | takatakca/TAKATAK-APP (public) | TAKATAK App | — | À DONNER PAR MATT | — | INTERNE (app) — à valider | — |
| 60 | takatakca/C4ISSE (public) | — | — | À DONNER PAR MATT | — | INTERNE (caisse) — à valider | — |
| 61 | takatakca/cake-concierge (privé) | Cake Concierge | — | À DONNER PAR MATT | — | INTERNE / projet — à valider par Matt (client externe ?) | Surplus grappe agence (§2) si Matt le classe client |
| 62 | takatakca/1lv-marketplace-hub (public) | 1LV Marketplace | — | À DONNER PAR MATT | — | INTERNE (marketplace ; lié à Takatak MUSIC 1LV ?) — à valider | — |
| 63 | takatakca/haste-mart (privé) | Haste Mart | — | À DONNER PAR MATT | — | INTERNE / projet — à valider | — |
| 64 | takatakca/Facturations (public) | — | — | À DONNER PAR MATT | — | INTERNE (facturation Groupe TAKATAK, selon description du dépôt) — aucune Page attendue | — |
| 65 | takatakca/ST4FF (public) | — | — | À DONNER PAR MATT | — | INTERNE (personnel) — à valider | — |
| 66 | takatakca/ACADEMYTAKATAK (public) | Academy TAKATAK | — | À DONNER PAR MATT | — | INTERNE (formation agence) — à valider | — |
| 67 | takatakca/TAKATAKREVIEW (public) | TAKATAK Review | — | À DONNER PAR MATT | — | INTERNE (produit avis, successeur Birdeye — P16 en attente) — à valider | — |
| 68 | takatakca/TR4CKER (public) | — | — | À DONNER PAR MATT | — | INTERNE (suivi) — à valider | — |
| 69 | takatakca/takatakbackend (public) | — | — | À DONNER PAR MATT | — | INTERNE (backend) — aucune Page attendue | — |
| 70 | takatakca/takatak-platform-reference (privé) | — | — | À DONNER PAR MATT | — | INTERNE (référence portails DoorDash/Uber, selon description) — aucune Page attendue | — |
| 71 | takatakca/skip-platform-reference (privé) | — | — | À DONNER PAR MATT | — | INTERNE (référence portail Skip) — aucune Page attendue | — |
| 72 | takatakca/T4CTILE (public) | Tactile | — | À DONNER PAR MATT | — | INTERNE / produit — à valider | — |
| 73 | takatakca/LOY4LTY (public) | Loy4lty | — | À DONNER PAR MATT | — | INTERNE (app fidélité Clover) — à valider | — |
| 74 | takatakca/LIVEID-TAKATAK (public) | LiveID TAKATAK | — | À DONNER PAR MATT | — | INTERNE / produit — à valider | — |
| 75 | takatakca/REW4RD (public) | Reward | — | À DONNER PAR MATT | — | INTERNE / produit — à valider | — |
| 76 | takatakca/ON2GO-CLOVER (public) | On2GO Clover | — | À DONNER PAR MATT | — | INTERNE (intégration Clover d'On2GO) — à valider | — |
| 77 | takatakca/4CCOUNTING (public) | — | — | À DONNER PAR MATT | — | INTERNE (comptabilité) — aucune Page attendue | — |
| 78 | takatakca/assurance-6241 (privé) | — | — | À DONNER PAR MATT | — | INTERNE (dossier d'assurance collaboratif, selon description — NEQ/dossier sensible) — aucune Page attendue | — |
| 79 | takatakca/takatak-doordash-operations (public) | — | — | À DONNER PAR MATT | — | INTERNE (workflows DoorDash, selon description) — aucune Page attendue | — |
| 80 | takatakca/r2fca (privé) | R2F | — | À DONNER PAR MATT | — | INTERNE / inconnu — à valider par Matt | — |
| 81 | takatakca/M4RKETING (public) | Marketing (outil agence) | — | À DONNER PAR MATT | — | INTERNE (outil agence) — à valider | — |

**Totaux du tableau : 81 dépôts — 23 OK · 12 DOUBLONS (dont 2 doublons de dépôts : mimtcaapp, QCMEV.CA) · 15 MANQUANTES · 31 INTERNE/à valider (dont QUADROHOLDING et foodhubca).** Projets clients comptés : 50 (23 + 12 + 15).

## §1 — Grappes de doublons (plusieurs Pages pour un même projet)

- **G1 PPP Pizzeria** (dépôt pppmtl) : PPP Pizzeria Montréal -Saint Léonard- https://www.facebook.com/483767435295888 · PPP Pizzeria Montréal -Notre Dame De Grâce- https://www.facebook.com/110018231878255 · PPP Montreal -Notre Dame De Grâce- https://www.facebook.com/1399633279898611. Deux Pages NDG pour un seul emplacement NDG = 1 vrai doublon ; SL est légitime (2e emplacement).
- **G2 Po Poulet** (dépôt POPOULET.CA) : Po Poulet Montreal -Notre Dame De Grâce- https://www.facebook.com/110497128431808 · Po Poulet https://www.facebook.com/108797431982867 · Po Poulet Montréal Hochelaga https://www.facebook.com/1324616364079000. À trancher par Matt : NDG officielle + Hochelaga (emplacement) + 1 sans suffixe (doublon probable). Grappe de confusion voisine : Poulet Express https://www.facebook.com/1378509388684827 (marque distincte, dépôt nº 15) et Poulet Poulet NDG https://www.facebook.com/247671908438134 (ex-Leopard Lake Gold Corp., aucun dépôt propre).
- **G3 O'oeuf** (dépôt OOEUF.CA) : OOEUF Montréal -Notre Dame de Grâce- https://www.facebook.com/102770028041467 · OOEUF Supreme Montréal NDG https://www.facebook.com/1453232214536227 · OOEUF Montréal -Hochelaga- https://www.facebook.com/113117403865850. Hochelaga = emplacement ; NDG × 2 = 1 doublon probable (« Supreme »).
- **G4 Pi Pita** (dépôt PIPITA.CA) : Pi Pita Montréal -Notre Dame De Grâce- https://www.facebook.com/108421598707603 · Pita Pita Montréal -Notre Dame de Grâce- https://www.facebook.com/247111815154972. Même emplacement, noms quasi identiques = doublon franc.
- **G5 Viennoise / Gâteaux Montréal** (dépôt VIENNOISE.CA) : Gâteaux Montréal -Notre Dame de Grâce- https://www.facebook.com/104383909121946 · Gâteau Montréal -Notre Dame de Grâce- https://www.facebook.com/107063592447528 · Gateau et viennoise Montréal -Notre Dame de Grâce- https://www.facebook.com/1065695216624618. Trois Pages, un emplacement = 2 doublons.
- **G6 BMBD** (dépôt BMBD.CA) : Bin Molle & Bin Dure Montréal https://www.facebook.com/102910359249848 · Bin Molle & Bin Dure Montréal Hochelaga https://www.facebook.com/1377415952121819 · (+ Crèmerie Bin Molle Bin Dure -Notre Dame de Grâce- https://www.facebook.com/1077344642127876, nom de marque long — même marque ; si les 3 visent NDG/Hochelaga, surplus = 1 à 2, à trancher par Matt).
- **G7 Nutrition Shake** (dépôt NUTRISHAKE.CA) : Nutrition Shake -Notre Dame De Grâce- https://www.facebook.com/111488005079940 · Nutrition Shake Montréal NDG https://www.facebook.com/1426349433894036 · Nutrition Shake Montreal Nord https://www.facebook.com/242913875561613. NDG × 2 = 1 doublon ; Montréal-Nord = adresse historique fermée (6241 boul. Léger) — son statut de Page d'emplacement est à trancher par Matt.
- **G8 Café Bolon** (dépôt BOLON.CA) : Bolon Café Montreal -Notre Dame De Grâce- https://www.facebook.com/115999504787601 · Café Bolon Montréal-Nord https://www.facebook.com/263614826835067. Montréal-Nord = adresse fermée → la 2e est recyclable si Matt confirme.
- **G9 Agence TAKATAK** (dépôts takatak + takatak-v1) : takatak.ca https://www.facebook.com/257633186140512 · Takatak Marketing https://www.facebook.com/109136031780822. Deux Pages pour l'agence = 1 doublon, à trancher par Matt.
- **G10 Dépôts jumeaux sans Page en double** : mimt / mimtcaapp (1 Page MIMT) · revers-canada-hope / QCMEV.CA (1 Page Revers Canada). Doublons de dépôts, pas de Pages — décision GitHub pour Matt, hors vague Facebook.

## §2 — Bassin de recyclage (Pages disponibles pour les projets MANQUANTES)

Surplus des grappes (après choix de la Page officielle par Matt) :
1. Une des deux Pages PPP NDG (110018231878255 ou 1399633279898611) — grappe G1.
2. Po Poulet (sans suffixe) 108797431982867 — grappe G2 (si Matt garde NDG + Hochelaga).
3. Une Page NDG de la grappe OOEUF (102770028041467 ou 1453232214536227 « Supreme ») — grappe G3.
4. Une des deux Pages Pi Pita NDG (108421598707603 ou 247111815154972) — grappe G4.
5. Deux des trois Pages Viennoise/Gâteaux NDG (104383909121946, 107063592447528, 1065695216624618 — en garder une) — grappe G5.
6. Une Page BMBD surplus (selon tranche de Matt) — grappe G6.
7. Une des deux Pages Nutrition Shake NDG (111488005079940 ou 1426349433894036) — grappe G7.
8. Une Page agence (257633186140512 ou 109136031780822 — en garder une) — grappe G9.

Pages dormantes, génériques ou hors projet :
9. Fdeals.ca QC — https://www.facebook.com/101574182413130 (15 abonnés ; aucun dépôt GitHub ; invitation Casa en attente).
10. Poulet Poulet NDG (ex-Leopard Lake Gold Corp.) — https://www.facebook.com/247671908438134 (9 abonnés ; contenu minier, pas un restaurant ; renommage possiblement encore en révision Meta — à revérifier en session).
11. Restaurant Montréal-Nord — https://www.facebook.com/158024287401897 (emplacement fermé 6241 Léger).
12. Café Bolon Montréal-Nord — https://www.facebook.com/263614826835067 (emplacement fermé ; aussi comptée en G8).
13. Taco Mexicano Montréal-Nord — https://www.facebook.com/278635711994147 (emplacement fermé ; marque Taco couverte par la Page NDG).
14. Nutrition Shake Montreal Nord — https://www.facebook.com/242913875561613 (emplacement fermé ; aussi comptée en G7 — seulement si Matt la détache de Nutrition Shake).
15. Halloween au Complexe Havana — https://www.facebook.com/1384551034735477 (saisonnière ; seulement si Matt la détache de Havana).
16. Sédition MUSIC — https://www.facebook.com/1208836188985578 (aucun dépôt ; statut à revérifier en session).
17. Miel Aissa — Page DÉSACTIVÉE vue dans les captures de Matt (« Not visible to the public », bouton Activate) ; pas dans les 57, pas de lien confirmé — à revérifier en session ; réactivation avant tout recyclage.
18. BP Taekwondo — https://www.facebook.com/1395058667296542 (hors 57 ; 0 personne assignée ; portefeuille barré par la vérification Meta — recyclage bloqué tant que la vérification n'est pas faite).

**Taille du bassin : 18 candidates** (dont 8 surplus de grappes et 10 dormantes/génériques/hors projet ; Miel Aissa et BP Taekwondo non confirmées en session). Besoin : 15 projets MANQUANTES (+ 2 conditionnels si Matt classe compassion-connect et cake-concierge comme clients). Le bassin couvre le besoin si Matt tranche les grappes.

**À NE PAS recycler (actives, déjà proposées à tort dans l'inventaire Casa 13:12 — correction)** : LOC Actif (Page du projet LOCACTIF.CA, nº 29), Rent Auto Canada (Page du projet rentautoca, nº 30), MIMT (398 abonnés), Qmaps.ca (658), Emploi Direct (200), Taxi Chambly (749, 234 avis).

## §3 — Courriels manquants — à demander à Matt

Pour chaque ligne ci-dessous : le courriel du projet (ou confirmation que le courriel maître takatak.ca@gmail.com s'applique). Liste générée depuis la colonne Courriel du tableau (mention « À DONNER PAR MATT ») :

qmaps · mimt · mimtcaapp (même projet que mimt) · EMPLOIDIRECT.CA · LOCACTIF.CA · rentautoca · taxichambly · ahmverdunca · GLOBESECURE.CA · revers-canada-hope · QCMEV.CA (même projet que revers) · CUBARESORT.CA · BESOINAVOCAT.CA · ACTIONAVOCAT.CA · Alkao.ca · CCC-CANADIEN-CONNEXION-CUBA · cubafoodca · MIELAISSA.CA · ocarinaspa · DOMINICFINANCE · isexy · flexsca · RAMASSEDEBRIS.CA · festiiceca · droneair · co-work.ca-montreal-launch · cuban-coin-cad · CH4T · R2NETTEEMAIL · takatak-automate · knowledgeAI · compassion-connect · SEOTAKATAK · TAKATAK-APP · C4ISSE · cake-concierge · 1lv-marketplace-hub · haste-mart · Facturations · ST4FF · ACADEMYTAKATAK · TAKATAKREVIEW · TR4CKER · takatakbackend · takatak-platform-reference · skip-platform-reference · T4CTILE · LOY4LTY · LIVEID-TAKATAK · REW4RD · ON2GO-CLOVER · 4CCOUNTING · assurance-6241 · takatak-doordash-operations · r2fca · M4RKETING.

Questions précises pour Matt (au-delà des courriels) : (1) promohavanaca — confirmer promohavana.ca@gmail.com comme courriel du projet Havana ; (2) INNTIME — confirmer inntime.ca@gmail.com (présumé) ; (3) compassion-connect et cake-concierge — clients externes (Page requise) ou internes ? (4) r2fca — c'est quoi ce projet ? (5) Pages officielles à garder dans chaque grappe §1 ; (6) Miel Aissa — réactiver ou abandonner ?

— Taktak

## Note d'après (résultat vérifié)

- Livrable terminé le 2026-11-01 (~15:52 EST) : 81 dépôts cartographiés — 23 OK · 12 DOUBLONS · 15 MANQUANTES · 31 INTERNE/à valider ; bassin de recyclage = 18 candidates ; 56 courriels à demander à Matt (§3).
- Dépôts : Drive Opérations **1qXx92a2RMW_F2EzvDbni9AbM2B4R5Lfa** ; GitHub QUADROHOLDING `docs/CARTOGRAPHIE-PROJETS-PAGES.md` (relu après push, contenu vérifié).
- Fil Gmail du jour (1a1954f63654da5c) : la réponse directe (+reply-all) a échoué — « could not prepare send », **rien n'a été envoyé**. La route brouillon a créé un brouillon HORS fil (threadId différent du fil du jour) : **non envoyé, mis à la corbeille**, conformément à l'interdit de créer un nouveau fil. Le corps du résumé est déposé en fichier : `~/workspace/your_files/2026-11-01 — Cartographie — corps courriel fil du jour — signé Taktak.txt` — à renvoyer dans le fil par la session principale à sa prochaine passe de supervision.
- Registre (en tête) et journal du jour mis à jour dans la même passe.
- Aucune action Meta (aucune création, aucun renommage, aucun recyclage). En attente : validation de Matt (bons / pas bons + courriels), puis vague 2 seulement après son OK.

— Taktak
