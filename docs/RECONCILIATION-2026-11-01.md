# Réconciliation complète — ordres de Matt, 2026-10-23 → 2026-11-01

**Mission :** terminer le fichier maître / la réconciliation (relance de Matt, 2026-11-01 10:15 EST : « t'as pas fini ta master file de tout relire, de tout réinscrire dans le GitHub pis de pousser tout qu'est-ce qu'on a oublié de finir »).
**Agent :** Taktak · **Date :** 2026-11-01 · **Statuts possibles :** FAIT (preuve nommée) · EN COURS · BLOQUÉ (geste de Matt ou blocage externe nommé) · OUBLIÉ (ordonné, jamais fait — ou jamais fini — au moment de la réconciliation).

---

## NOTE D'AVANT — état lu + plan (signé Taktak)

**Ce qui existait avant cette passe :**
- Corpus d'extraction complet : `~/workspace/extraction-rattrapage/` — digest-7jours.md (24 585 lignes, ~6 200 tours relus page par page), notes-7jours.md (4 126 lignes : 15 sections par département + section « NON FAIT » de 22 items + 1 098 paroles de Matt mot pour mot), progression-7jours.md (160 lignes), matt-verbatim-7jours.txt. Fenêtre couverte : 2026-10-23 → 2026-11-01 01:22.
- « Livre maître » déposé le 2026-11-01 02:16 : GitHub QUADROHOLDING commit 8aecb3ac, Drive 1na3DRhT9EJlT_6GChwk5gunO4B8_vbId, issue nº 6 ; 22 NON FAITS y étaient signalés aux agents (annonce envoyée 02:23, msg 1a195fde683b36ee).
- Fichier maître local (703 286 octets, tableau des missions M-01 → M-36) + copie Drive 16d0HAHtKXnqhckLPCodFHLiBl_VSf7QU ; registre `registre-travail-fait.md` (plus récent en tête) ; MEMORY.md.
- Le « Livre maître de mise à jour » (fichier local de 415 397 octets reprenant les notes-7jours avec en-tête) existait, mais **son dépôt avait été ARRÊTÉ à l'étape 0 (sécurité)**.

**Blocage sécurité — identifié et tranché dans cette passe :**
- Le déclencheur de l'arrêt : un grep de sécurité sur `notes-7jours.md` a frappé les motifs de noms de clés `*SECRET*`, `*KEY*`, `*TOKEN*`, `*PASSWORD*` (80 lignes touchées par le motif combiné) — arrêt de précaution à l'étape 0, avant de distinguer noms et valeurs.
- Vérification faite ligne par ligne dans cette passe (valeurs jamais reproduites) : dans **notes-7jours.md, il n'y a AUCUNE valeur de secret** — seulement (a) des **noms de variables d'environnement en prose** : CLOVER_CLIENT_SECRET (×2), CLOVER_WEBHOOK_SECRET (×3), CLOVER_WEBHOOK_AUTH (×1), toujours cités comme « jamais posé / introuvable / à poser via le coffre » ; (b) des mentions en prose (« mot de passe », « session », « token ») qui racontent des événements, sans valeur ; (c) des faux positifs (« IBAN » = l'intérieur de « Libanais »/« pitalibanais »). Aucune affectation NOM=valeur, aucun préfixe de jeton réel (familles Stripe/GitHub/Google/Slack/webhook/bloc PEM vérifiées une à une), aucune forme de carte, aucun code numérique, aucun hex long dans notes-7jours.md ni progression-7jours.md (0 partout).
- Le fichier « Livre maître de mise à jour » lui-même : balayage propre — 44 marqueurs « [valeur non consignée — vit au coffre] », 0 date de naissance, 0 forme de carte, 0 hex long, 0 code, 0 préfixe de secret. La passe de rédaction avait donc été efficace ; seuls les **mots-clés** subsistent (38 lignes « mot de passe » en prose, 5 noms CLOVER_*_SECRET).
- Le **digest brut** (digest-7jours.md), lui, contient encore des formes sensibles dans les citations brutes (dates de naissance en contexte ×9, une forme de numéro en 4×4 chiffres ×1, hex longs ×2 — vraisemblablement des hachages de commits —, contextes de codes numériques ×9) : **le digest reste un document source LOCAL, jamais déposé**. Règle appliquée à tous les dépôts de cette passe : construire depuis la couche notes (rédigée), jamais depuis les citations brutes, et re-grepper chaque livrable avant poussée.
- ⚠️ Rappel consigné (pas une valeur) : des jetons API ont été collés en clair dans le chat le 2026-10-26 (constat déjà présent dans les notes) ; ils vivent dans l'historique source — traitement = rotation par Matt/dev (voir M-15, item R-97).

**Ce qui manquait (le cœur de la relance de Matt) :** la réconciliation n'avait jamais été (1) mise à jour avec l'état postérieur au 2026-11-01 01:22 (fermeture Uber 06:39, ordre Jean-Talon 02:42 + portée confirmée 09:03 + retrait approuvé 10:04, vague DoorDash en cours, PR takatak-v1 nº 238 fermée sans fusion 09:09), (2) réinscrite dans le fichier maître avec propriétaires, (3) poussée en document de réconciliation sur GitHub. Et deux chantiers ordonnés n'avaient jamais été faits du tout : les visuels Uber appliqués aux Pages Facebook et les posts quotidiens Canva par brand (relancés le 2026-11-01 10:15 = P20/P21/P22 ; la présente mission = le chantier fichier maître).

**Plan :** (1) relire corpus + maître + registre + MEMORY.md ; (2) tableau complet des ordres avec statut et preuve ; (3) liste des OUBLIÉS ; (4) RESTE À FINIR par propriétaire, inscrit dans le fichier maître ; (5) dépôts : maître → Drive en place, ce document → GitHub QUADROHOLDING docs/ + Drive Opérations ; (6) registre mis à jour.

— Taktak

---

## SOMMAIRE DES COMPTES

**128 items réconciliés** (comptés sur le tableau ci-dessous, un item = un ordre ou un chantier de Matt) :

| Statut | Nombre |
|---|---|
| FAIT (preuve nommée) | 27 |
| EN COURS | 25 |
| BLOQUÉ (geste de Matt ou blocage externe nommé) | 37 |
| OUBLIÉ (jamais fait / jamais fini) | 39 |
| **Total** | **128** |

Lecture honnête : le FAIT est minoritaire. Le BLOQUÉ est dominé par des gestes que seul Matt peut faire (connexions, paiements, décisions, envois « send »). L'OUBLIÉ est le vrai problème que Matt a relancé le 2026-11-01 : 39 items, dont plusieurs ne demandaient AUCUN geste de Matt (visuels Facebook, confrontations portail DoorDash, réponses dues à DoorDash, menus Skip, réponses d'agents jamais revenues).

---

## TABLEAU COMPLET — tous les ordres de Matt depuis le 2026-10-23

### A. Meta / Facebook — Pages, accès, monétisation

| Nº | Item | Statut | Preuve / blocage | Propriétaire |
|---|---|---|---|---|
| R-01 | Redondance admins : les 3 comptes de Matt en contrôle complet sur toutes les Pages (règle du 2026-10-31 23:11) | FAIT | Vague terminée et auditée le 2026-11-01 00:34 (57 Pages) ; note signée Drive Opérations 1rmpsTSXGLPA3GSlMimkvsjFutz46ss9c ; Casa : 41 invitations envoyées, LesGroupes : 29 en place | Taktak / LesGroupes |
| R-02 | Acceptation des invitations côté Casa + relances des 3 Pages bloquées par la limite d'invitations Meta (AhM Verdun, Les Délices D'Aden, Cuba Resort Canada) | EN COURS | Invitations en attente côté Casa ; limite Meta à laisser se libérer | LesGroupes |
| R-03 | Portefeuilles Meta à vérification de compte (Estephanie Molina, Rapide 2 Nette, Takatak INC, irqc.ca) | BLOQUÉ | « Verify account » jamais cliqué — geste de Matt | Matt (geste) |
| R-04 | Création des ~8–10 Pages restantes (Place Afrique Hochelaga, Poulet Poulet SL, Déjeuner & Dinner Hochelaga, Café Bolon Hochelaga, Mythos & Go Hochelaga, Gâteaux Montréal SL, Bin Molle & Bin Dure SL, INN TIME Hochelaga…) | OUBLIÉ | Création refusée par Meta le 2026-10-31 sur les 2 comptes essayés ; la route Casa Lachine (compte sain, connecté 22:18) n'a jamais été relancée pour créer | LesGroupes |
| R-05 | 3 renommages de Pages (Pizza Algérie SL, Place Afrique NDG, Poulet Poulet NDG) | EN COURS | Statut CONTESTÉ : rapport 00:34 = « soumis, en révision » vs rapport 22:01 = « arrêtés au mur du mot de passe » — à trancher par relecture Meta directe avant toute affirmation | Taktak / LesGroupes |
| R-06 | Recyclage BP Taekwondo → Pi Pita SL | BLOQUÉ | Tenté en dernier, bloqué derrière la vérification Meta | LesGroupes |
| R-07 | Post épinglé/en vedette « 6241 » sur les Pages PPP (ancien numéro/adresse + 24/7) | OUBLIÉ | Toujours présent aux contrôles SOCIO répétés (dernier : 2026-11-01 08:52, inchangé) ; jamais dépinglé ni remplacé par le post canonique | SOCIO |
| R-08 | Page PPP NDG affichée « Always open » alors que l'horaire réel est 16 h–3 h | OUBLIÉ | Incohérence signalée dès le 2026-10-28, toujours ouverte aux contrôles SOCIO | SOCIO |
| R-09 | Monétisation Facebook 100 % par Page + publicité maison dans nos reels (M-30) | OUBLIÉ | Mandat déposé le 2026-10-31 04:20 (Drive Opérations) ; aucune activation vérifiée Page par Page ; PPP SL : « Not yet eligible / Invite only », abonnements 1/3 | SOCIO |
| R-10 | Ménage du mur PERSONNEL de Matt + tri de ses photos personnelles en albums (noms protégés intouchables) | OUBLIÉ | Ordonné le 2026-10-25 ; fenêtre morte en Phase 1 (inventaire partiel), jamais repris | Taktak |
| R-11 | Visuels Uber Eats (bannière, header, logo du nouveau set) appliqués à l'identique sur les Pages Facebook et les réseaux (IG, X) | OUBLIÉ | Ordre « VISUELS UBER → PARTOUT » du 2026-11-01 ; relance de Matt le 2026-11-01 10:15 : « t'as jamais appliqué les logos qui sont directement dans le Uber ou dans le DoorDash, directement sur leur page Facebook » — aucune application faite | SOCIO / Lévesque |
| R-12 | Posts automatiques quotidiens pour chaque brand, photos Canva, publiés DEPUIS Canva (loi du 2026-10-27) | EN COURS | Oublié jusqu'à la relance de Matt du 2026-11-01 10:15 ; étape 1 (inventaire + montage) lancée le 2026-11-01 — note signée « Posts quotidiens Canva par brand » ; blocage précis trouvé : le connecteur Canva n'a ni outil de publication/programmation ni edit-design (publication à faire depuis l'interface Canva/Facebook) ; aucun post n'est encore parti | SOCIO / Taktak |
| R-13 | Format publicitaire carrousel Meta par défaut (M-35) | FAIT | Dépôts vérifiés : GitHub QUADROHOLDING docs/FORMAT-PUBLICITAIRE-CARROUSEL-META.md (commit 67c62d55) + issue nº 4 ; Drive Opérations 1NMuHXhGdoraeP5HN1ntRfQO5ADmf9P6Q ; maître M-35 | SOCIO |
| R-14 | Modèle courriel de marque des 18 marques (en-tête blanc + pied professionnel, ajout seulement) (M-23) | OUBLIÉ | Consigne déposée le 2026-10-30 (note Drive + maître + GitHub) ; SOCIO n'a jamais étampé ni livré | SOCIO |
| R-15 | TripAdvisor : créer les fiches manquantes des 18 marques × emplacements et tout lier (M-26) | OUBLIÉ | Mandat envoyé le 2026-10-31 (msg 1a1904f88eea9e22) + ordre d'exécution sur issue QUADROHOLDING nº 1 ; aucun rapport par marque jamais revenu | SOCIO |
| R-16 | Contrôles Facebook SOCIO (cadence ~3 h) | EN COURS | Dernier contrôle déposé : 2026-11-01 08:52, vérifié inchangé (supervision 09:40) | SOCIO |

### B. Uber Eats

| Nº | Item | Statut | Preuve / blocage | Propriétaire |
|---|---|---|---|---|
| R-17 | Magasins modèle terminés à 18 catégories / 193/193 (nº 1 BMBD SL, nº 2 Gâteaux SL, nº 3 Nutri SL, nº 7 Gâteaux NDG, nº 8 Nutri NDG, nº 9 O'Oeufs NDG, nº 14 Pizza Algérie = le modèle, nº 15 Mythos & Go) | FAIT | Vérifiés un par un entre le 2026-10-25 et le 2026-10-31 ; nº 14 terminé le 2026-10-29 21:14 | Lévesque (fenêtre Uber) |
| R-18 | Nº 16 PPP Pizzeria Saint-Léonard — construction complète | FAIT | Vérification finale le 2026-11-01 07:16–07:19 UTC : 18 catégories, 193 livraison / 193 ramassage, ancres chiffre par chiffre ; magasin 627d09f0-8fb4-57f2-8ec1-6a71984ad267 | Taktak (fenêtre Uber) |
| R-19 | Nº 11 O'OEUF SL — nettoyage (le « terminé » du 2026-10-29 ne tenait pas) | FAIT | Nettoyage terminé et revérifié le 2026-11-01 10:50–10:52 UTC : 18 catégories, 193/193 ; 12 trios en double et 3 breuvages en double supprimés, ~25 prix corrigés | Taktak (fenêtre Uber) |
| R-20 | Inscriptions des marques absentes : 22 magasins créés au portail (40 au total) | FAIT | Créés le 2026-11-01, arrêtés au launchpad à 14 % (Continue jamais cliqué, aucune étape bancaire/ID) ; note signée Drive Opérations 1L88iBIU-za7kQIWn-B78tyJ2kzrZXG3I | Taktak (fenêtre Uber) |
| R-21 | Onboarding des 22 magasins créés (finir la configuration, poser le courriel de chaque marque) + suivi des 6 paires Hochelaga détournées vers le contact Uber (1–3 jours ouvrables) | EN COURS | Rien n'est lancé ; les courriels de marque sont consignés « à poser aux réglages / à l'onboarding » dans la note d'inscription | Lévesque |
| R-22 | 2 demandes Jean-Talon E soumises AVANT l'ordre d'arrêt (Po Poulet SL 028dd6c9-f92e-46c2-915e-567519d44355 ; Taco Mexican SL 137014b7-940b-450d-a777-947a395b990a) | BLOQUÉ | Gelées en préparation (14 %), non supprimables au portail ; retrait approuvé par Matt le 2026-11-01 10:04 — message au support Uber préparé et montré au chat, en attente de son « send » (procédure edit/send) | Matt (send) |
| R-23 | Architecture des prix pizzas du nº 16 (item à 0,00 $ + prix pleins par grandeur, façon PPP, vs prix de base + incréments du modèle) | BLOQUÉ | Décision de Matt demandée le 2026-11-01 ~06:43, toujours pendante | Matt (décision) |
| R-24 | Nº 4 Bin Molle & Bin Dure NDG — « Paused by Uber Eats », éditeur Menu Maker non autorisé | BLOQUÉ | Reconfirmé le 2026-11-01 07:31 UTC ; seule route = support Uber ou le gestionnaire de compte de Matt — commence par Matt | Matt (geste) |
| R-25 | 3 renommages bloqués par le filtre Uber (« Coca-Cola », « Cheesecake Amande », « Gâteau Amande » gardés aux bons prix) | EN COURS | Prix et comptes intacts ; seul recours = appel au support Uber (envoi externe = procédure edit/send, jamais préparé) | Taktak |
| R-26 | Magasins à 90–95 % : PPP NDG pilote 95 % · Bolon NDG 90 % (page publique « fermé depuis le 8 oct. » à confirmer) · Bolon SL 95 % · O'Oeufs 6280 95 % (décision breuvages DELUXE ouverte) · Pi Pita NDG 90 % · Pi Pita SL 95 % (page publique vide) | EN COURS | Programme de déploiement, états vérifiés au registre | Lévesque |
| R-27 | Pizza Algérie : le magasin vivant nº 14 est déployé sous 6280 Somerled alors que son adresse canonique est 5839 Jean-Talon E — correction d'adresse due | OUBLIÉ | Signalé à répétition depuis le déploiement ; jamais corrigé au portail | Lévesque |
| R-28 | Audit des frais Uber : 127 relevés + 2 CSV consolidés (2026-05 → 2026-10, plafond portail 184 jours) | FAIT | Extraits le 2026-11-01 ; fichiers f01–f18 dans ~/workspace/uber-fees-extraction/ ; note signée Drive Opérations 10tKHuZuDDF-hLstTS2xKVEVH8U2I0mtg + Drive Comptabilité 14m1RBCQagyDgGcSsFE2F33KM5umztQ2H ; ZIP Drive 111XCpMmKKqmwtMZOPzi7Yw3pxMDWkNJW | Taktak |
| R-29 | Lettre L3 Uber — versements suspendus 1 688,72 $ | FAIT | Envoyée le 2026-10-31 à merchants@uber.com (msg 1a1948c2f1373be1, fil 1a15a4909fb552d1), autorisée séparément par Matt | Taktak |
| R-30 | Approbation Uber demandée pour Baba Hamdi | FAIT | Vérifié le 2026-10-27 : magasin absent du compte (18 magasins passés au complet, aucune invitation) — rien à approuver ; dossier clos sur preuve | Taktak |

### C. DoorDash

| Nº | Item | Statut | Preuve / blocage | Propriétaire |
|---|---|---|---|---|
| R-31 | Clonage des menus au portail (groupe 10626494, menus v3) | FAIT | Terminé le 2026-10-30 ; clones laissés inactifs à ce moment | Taktak (fenêtre DoorDash) |
| R-32 | Corrections des magasins ACTIFS au catalogue v3 (OOEUF SL → Gâteau NDG → PPP Hochelaga reconstruction complète → Po Poulet NDG en dernier, un changement à la fois) | EN COURS | Vague en cours (fenêtre 91ebd08d, mandat du 2026-10-31 20:33) ; audit de référence : 10 items manquants par magasin bâti, TRIO/COMBO erronés, DUO absent, règles breuvages à refaire | Taktak (fenêtre DoorDash) |
| R-33 | Nouvelles demandes pour chaque magasin désactivé/inactif (même entreprise, ancien laissé tel quel) | EN COURS | Ordre de Matt du 2026-10-31 20:37, dans la même vague ; **pause Jean-Talon E définitive** (ordre 02:42, portée confirmée toutes marques le 2026-11-01 09:03, transmise à la fenêtre) | Taktak (fenêtre DoorDash) |
| R-34 | Confrontations PORTAIL Po Poulet 41946420 (copies texte tronquées après Pita ; assiettes absentes du corps depuis la copie de 12:19 UTC) et Gâteau 28114454 (écart texte vitrine vs portail) | OUBLIÉ | Des dizaines de relectures texte faites ; la confrontation au portail elle-même n'a jamais eu lieu — elle bloque toute correction d'items sur ces 2 magasins | Taktak (fenêtre DoorDash) |
| R-35 | Activations : OOEUF SL 33597929 en ligne ; PPP Hochelaga 33598081 réactivé | FAIT | Vérifiés ouverts le 2026-10-31 (OOEUF SL en ligne ; PPP Hochelaga réactivé 17:00, Open sur les 2 canaux) | Taktak |
| R-36 | Activations BMBD NDG 28108457 et Pizza INNTIME 28519423 (contrôles passés, erreur portail à l'activation) | EN COURS | Erreur portail au moment d'activer ; jamais réessayé depuis | Taktak (fenêtre DoorDash) |
| R-37 | Vérification d'entreprise Stripe : Po Poulet NDG 41946420 + Mythos 2 Go NDG 41946413 | FAIT | Soumise le 2026-10-31 19:11 — « Pending verification » ; ville, TVQ, détails publics posés ; bancaire intouché ; « Confirm your directors » jamais pressé | Taktak |
| R-38 | Lettre v6 DoorDash — réclamation 10 492,07 $ | FAIT | Envoyée le 2026-10-31 ~16:24 (msg 1a1939f74bbac3c8, fil 1a18d3689f869d3d) ; réponse DoorDash : conciliation ligne par ligne exigée ; décision écrite toujours attendue | Taktak |
| R-39 | Lettre L1 DoorDash — ajustements injustifiés 2 988,01 $ (98 lignes, 13 magasins) | FAIT | Envoyée le 2026-10-31 ~20:39 à mxpsupport@doordash.com (msg 1a1948b542b9f8d3), approuvée par Matt | Taktak |
| R-40 | Relance de suivi sur la réclamation de 10 492,07 $ (brouillon D1 §8 prêt) | BLOQUÉ | En attente du choix de pièces de Matt (2 PDF REQ/fiscaux OU 2 CSV de frais OU aucune) + procédure chat edit/send | Matt (choix + send) |
| R-41 | Réponse due à Hailin — cas 774709330 (IDs de magasins + courriel de réception des commandes par magasin) | OUBLIÉ | Dette consignée à l'extraction D1 du 2026-10-31 ; jamais préparée ni envoyée | Codex / Taktak |
| R-42 | Réponse due à l'équipe Photos — cas 773996517 (IDs entreprise/magasin pour le magasin 27982486) | OUBLIÉ | Dette consignée à l'extraction D1 du 2026-10-31 ; jamais préparée ni envoyée | Codex / Taktak |
| R-43 | Retransmission de L1 à l'avocat Yan Romanowski | BLOQUÉ | Son adresse courriel est introuvable dans nos fichiers, contacts et 4 boîtes vérifiées | Matt (adresse) |
| R-44 | Lettre L2 (frais bancaires) | BLOQUÉ | Avis du 2026-10-30 : paiement de 2,90 $ échoué pour Po Poulet NDG sur un compte finissant 0619 — source inexpliquée ; brouillon Drive 1Ntt6CGwGYPFLsY2ZXEaj98rsbyoA4F5q ; jamais envoyer la version Desjardins (compte fermé, consigne corrigée par Matt le 2026-10-31 : BMO courant) | Taktak |
| R-45 | Réactivation Gâteaux Montréal NDG — documents exigés par Hailin (cas 774713534 : propriété, Tax ID, pièce d'identité, chèque annulé, routing, infos bancaires) | BLOQUÉ | Courriel à Hailin envoyé le 2026-10-29 10:31 ; les documents eux-mêmes n'ont jamais été fournis | Matt (documents) |
| R-46 | Recalcul complet des frais par marque depuis octobre 2025 (ordre de Matt du 2026-10-27, après sa déception sur les frais de tablette) | EN COURS | Extraction D1 terminée (7 923 messages, 150 PDF → 101 uniques) et fichier maître des frais déposé ; le recalcul par marque livré en entier reste à produire dans le classeur BMO (R-103) | Taktak |
| R-47 | Retrait des 4 breuvages hors catalogue du groupe OOEUF SL (RED BULL, COURONNE, MAKAYA, LAIT AU CHOCOLAT — ruling catalogue du 2026-10-31 21:52 : retirés, pas re-tarifés) | EN COURS | Ruling transmis à la vague de corrections ; retrait non attesté à ce jour — à vérifier au prochain passage de la fenêtre | Taktak (fenêtre DoorDash) |
| R-48 | Confirmation d'utilisation des 152 photos par Gerlin Rivera (M-17) | EN COURS | Paquet livré le 2026-10-29 ; vérifié le 2026-10-31 : aucune réponse ; aucune relance envoyée | Taktak (attente externe) |
| R-49 | Rapports DoorDash téléchargés par Matt le 2026-10-28 (3 rapports restés dans le navigateur) | OUBLIÉ | Jamais récupérés au Drive malgré l'ordre « Mettre dans google drive » (pont navigateur→fichiers brisé) ; job quotidien de téléchargement créé, passe du 2026-10-31 en échec | Taktak |
| R-50 | Régénération des rapports mensuels DoorDash expirés | BLOQUÉ | Décision de Matt requise | Matt (décision) |

### D. SkipTheDishes

| Nº | Item | Statut | Preuve / blocage | Propriétaire |
|---|---|---|---|---|
| R-51 | Inventaire du portail (11 magasins, compte « masteraccount ») | FAIT | Note signée du 2026-10-31 déposée ; 1 seul magasin en ligne (PPP NDG) | Taktak (fenêtre Skip) |
| R-52 | 41/41 inscriptions soumises et confirmées (7 NDG, 17 Saint-Léonard, 17 Hochelaga) | FAIT | Confirmations /success du portail partenaires le 2026-11-01 00:46 ; aucun numéro de référence émis ; les 17 Saint-Léonard PRÉDATENT l'ordre Jean-Talon du 2026-11-01 02:42 | Taktak (fenêtre Skip) |
| R-53 | Poser le courriel propre de chaque marque sur les 41 inscriptions (30/41 parties sous takatak.ca@gmail.com) | OUBLIÉ | Loi de Matt du 2026-10-26 : chaque marque vit sous SON courriel ; correction jamais faite — à poser aux appels d'onboarding Skip (1–2 jours ouvrables promis) | Taktak |
| R-54 | Menus Skip alignés au catalogue v3 + heures canoniques (menus actuels = ancien menu partagé 175 items ; heures portail fausses) | OUBLIÉ | « Earliest stage » déclaré à Matt le 2026-11-01 00:36 ; jamais clonés ni vérifiés depuis | Lévesque |
| R-55 | Vérification du compte Skip (code de vérification en 2 étapes au téléphone finissant 587) | BLOQUÉ | Code délibérément jamais demandé — geste de Matt | Matt (code) |
| R-56 | Réclamation des frais hebdomadaires inexpliqués : 584,64 $/semaine sur 7 magasins (zéro commande, aucune ligne de conciliation) | OUBLIÉ | Documenté au fichier maître des frais (déposé) ; la lettre de réclamation elle-même n'a jamais été préparée | Taktak |
| R-57 | Écart des numéros de taxes imprimés sur les relevés Skip (TVQ 1225732198TQ0001 / TPS 833276447 ≠ paire canonique) | EN COURS | Écart consigné, non résolu ; à soulever avec Skip à l'onboarding | Taktak |
| R-58 | Spec du clone Skip (référence pour le dashboard Food Hub unifié) | FAIT | Dépôt takatakca/skip-platform-reference, commit 9ab37c7f879215ce09c9e2ce1b4320c08e89e690 | Taktak |

### E. Clover — marchand et Marketplace

| Nº | Item | Statut | Preuve / blocage | Propriétaire |
|---|---|---|---|---|
| R-59 | Clover marchand On2GO.CA : audit complet + corrections (descriptions catalogue, prix, groupes, photos officielles jaunes) | FAIT | Annoncé terminé et vérifié le 2026-10-28 14:33 ; photos Trios 18/18 vérifiées le 2026-10-25 ; en-tête (450) 999-4999 relu chiffre par chiffre le 2026-10-29 | Taktak |
| R-60 | Adresse d'en-tête Clover toujours à 6284 au lieu de 6280 | OUBLIÉ | Écart distinct ouvert depuis le 2026-10-28 ; jamais corrigé | Lévesque |
| R-61 | 12/18 descriptions de Trios disent encore « boisson » au lieu de « breuvage » | OUBLIÉ | Constaté le 2026-10-28 10:33 ; correction annoncée à la fenêtre suivante, jamais revérifiée | Lévesque |
| R-62 | 5 images d'items Clover manquantes à produire (M-10) | OUBLIÉ | Demandées à Lévesque le 2026-10-29 ; aucun retour au 2026-11-01 (M-08/M-09/M-10 tous sans retour) | Lévesque |
| R-63 | Fiches des 11 apps Clover — dossiers complets en DRAFT (plans 50/100/150 $ décidés par Taktak) | FAIT | Vague fiches 11/11 terminée le 2026-10-30 04:03 ; script maître M-01 et guidelines M-03 déposés (Drive 1AWFm3ZSzJjvn38Ixy-1VfJSF8C0SxcTi) | Taktak |
| R-64 | Soumission des 11 apps (« Submit App ») | EN COURS | Jamais cliqué — par règle : apprendre les guidelines et ne soumettre que des fonctions testables ; dépend de la production vidéo (R-65) et des fonctions branchées | Taktak |
| R-65 | Production vidéo des 11 apps (M-04 : captures réelles + Runway, 2 vidéos/app) | EN COURS | Scripts 11/11 écrits et déposés (Drive 19f5kTVKf6952Sah_-NqAovBWbWB1HPZG) ; la production elle-même n'a jamais été lancée | Taktak / SOCIO |
| R-66 | LOY4LTY : ticket DNS Mochahost MOCHA-JHB-404-25821, CLOVER_CLIENT_SECRET à poser (session fraîche), authentification webhook, test marchand | BLOQUÉ | App déployée sur Coolify (2026-10-29) ; restes bloqués par l'incident Contabo (R-84) et la session développeur fraîche à faire | Taktak / dev |
| R-67 | Statut services/facturation du marchand Clover désactivé (« .ca » minuscule, bannière « vos services ont pris fin ») | BLOQUÉ | Jamais vérifié par Matt depuis le constat du 2026-10-25 | Matt (vérification) |

### F. Google — Business, Merchant Center, agence

| Nº | Item | Statut | Preuve / blocage | Propriétaire |
|---|---|---|---|---|
| R-68 | Créations Google Business en bulk sous le compte agence (31 fiches) | BLOQUÉ | **GARÉ par Matt le 2026-10-29** (« il fera sa partie plus tard ») — ne pas relancer, ne pas rapporter ; import jamais soumis (clic « Select file » de Matt jamais reçu) ; créations faites sous on2go contre l'ordre initial | Matt (garé) |
| R-69 | Suggestion d'heures erronée 11 h–23 h soumise à Google sur PPP NDG (réel : 16 h–3 h) | EN COURS | En révision chez Google depuis le 2026-10-31 ; consigne de Matt : surveiller le résultat ; si appliquée, corriger immédiatement (la fiche affiche toujours 16 h–3 h) | Taktak |
| R-70 | Merchant Center : chaîne des 10 comptes terminée | FAIT | Terminée le 2026-10-28 (dernier : Taco MC 5890482821) | Taktak |
| R-71 | Merchant Center : 0 produit approuvé sur 6 comptes × 198 produits ; vérifications de sites reportées | OUBLIÉ | Constaté le 2026-10-26 ; jamais repris depuis | Taktak |
| R-72 | Suspension de l'accès Google Business Profile de ooeuf.ca@gmail.com (M-28) | BLOQUÉ | Découverte le 2026-10-31 00:41 lors de la liaison au MC 5881528797 ; appel jamais soumis — décision de Matt | Matt (décision) |
| R-73 | Identifier le compte qui détient les fiches O'oeuf 6280 Somerled et 5839 Jean-Talon E et les lier au Merchant Center | OUBLIÉ | Les fiches n'étaient pas sous ooeuf.ca@gmail.com (liste du 2026-10-31) ; seul le 6241 Léger a été lié ; recherche du compte détenteur jamais faite | Taktak |

### G. Citations / Annuaires

| Nº | Item | Statut | Preuve / blocage | Propriétaire |
|---|---|---|---|---|
| R-74 | Yelp PPP Saint-Léonard + PPP NDG à 91 % (galerie menu complète, 169 images) | EN COURS | Restes = gestes de Matt seulement : installer/ouvrir l'app Yelp for Business + photo du compte utilisateur derrière le mur de vérification | Matt (gestes) |
| R-75 | Yelp — toutes les autres marques | OUBLIÉ | Seul PPP a été traité ; aucune autre marque jamais faite sur Yelp | Lévesque |
| R-76 | Yelp O'oeuf — fenêtre garée à l'étape du mot de passe Google (pré-remplissage fautif attrapé, rien soumis) | BLOQUÉ | Choix de Matt demandé le 2026-10-31 07:05, sans réponse | Matt (geste) |
| R-77 | Wikidata — entité TAKATAK Marketing supprimée le 2026-10-27 (notoriété) | BLOQUÉ | Contestation déposée ; restauration = décision de Matt, sans décision d'admin à ce jour | Matt (décision) |
| R-78 | Cylex — 13 fiches prêtes sous un seul compte (contre la loi « 1 courriel = 1 entité »), porte fermée | BLOQUÉ | Matt : attendre (gratuit) ; correction de la fiche O'oeuf Cylex (toujours au 6241 avec l'ancien téléphone 450-600-6383) jamais faite | Taktak |
| R-79 | Foursquare — O'oeuf et Bolon toujours au 6241 avec de mauvais téléphones | OUBLIÉ | Constaté le 2026-10-26 ; jamais corrigé | Taktak |
| R-80 | Balayage 411.ca | FAIT | Fait le 2026-10-26 : aucune fiche de marque (seul l'ancien occupant au 6241) | Taktak |
| R-81 | Pages Jaunes — corrections des fiches | FAIT | Courriel du 2026-10-27 rebondi puis resoumission accusée le 2026-10-28 (suivi 26193506) ; courriel à Dane Bettridge envoyé le 2026-10-31 (inscription gratuite réglée, aucun produit payant sans approbation écrite) | Taktak |
| R-82 | RestoMontréal | BLOQUÉ | Bloqué Cloudflare, constaté par Matt lui-même ; garé | — |
| R-83 | Birdeye → décision : soumettre le courriel au formulaire de démo ou bâtir depuis les pages publiques | BLOQUÉ | Demandé à Matt le 2026-10-31 05:57 ; jamais tranché (lien avec le système d'avis maison, R-95) | Matt (décision) |

### H. Sites / GitHub / Dev / Produits

| Nº | Item | Statut | Preuve / blocage | Propriétaire |
|---|---|---|---|---|
| R-84 | Contabo — VPS vmi3621936 en « Error » depuis le 2026-10-30 (ticket 16240531435 : restaurer sans réinstaller ni effacer) | BLOQUÉ | Contabo a répondu le 2026-11-01 03:56 : Rescue actif, connexion impossible sans les identifiants Rescue définis à l'activation — question portée à Matt (identifiants via carte sécurisée, ou demander la marche à suivre) ; Coolify revenu le 2026-10-31 22:56 mais 7/14 sites toujours en panne au contrôle TWILO de 07:45 | Matt (réponse) |
| R-85 | PPP — preuve d'un paiement réel (checkout atteint la page Clover, aucune preuve complétée) ; NO-GO paiements maintenu | BLOQUÉ | Stripe Link non connecté + réautorisation Stripe du marchand = clic de Matt ; connecteur Stripe toujours « reauthorization_required » au 2026-11-01 06:17 | Matt (clics) |
| R-86 | PPP — SMS Twilio (bouton « Envoyer un code » mort, issue pppmtl nº 20) | BLOQUÉ | Activation AUTORISÉE par Matt le 2026-10-29 ; reste : créer/recharger le compte Twilio et poser les identifiants dans Coolify via le coffre — geste de Matt, bloqué aussi par Contabo | Matt (compte) |
| R-87 | Interac — deux copies existent (pppmtl, désactivée dans le code, commits 47f8c944/098fd63b ; Food Hub, PR DRAFT nº 141 bloquée à l'approbation BMO) | BLOQUÉ | Choix du propriétaire jamais fait par Matt : quelle copie est l'officielle | Matt (décision) |
| R-88 | pppmtl — PR ouvertes 19/21/22/23/25 non fusionnées ; main = 098fd63b (veille du 2026-11-01 10:14) | EN COURS | Rebase + CI = travail du dev ; veilles aux 15 min actives, aucun nouveau commit depuis 03:28 EST | Dev PPP |
| R-89 | Garde /dev de pppmtl jamais déployée — page d'audit interne pppmtl.com/dev/menu-audit exposée publiquement sans connexion | OUBLIÉ | Signalée le 2026-10-28 01:40 ; jamais fermée ni déployée | Dev PPP |
| R-90 | Alerte fraude (appel) — paquet de 28 snippets prêt pour les 18 restaurants | OUBLIÉ | Bâti le 2026-10-30 (ZIP Drive 1CJJbQtG2Vgi5cYjKo9ixXF85J00ThTQa) ; jamais déployé — attend la restauration Contabo puis le déploiement site par site | Taktak |
| R-91 | Food Hub — écrans de commande, étapes 3–6 (serveur relais, 18 écrans, connexions) (M-13) | BLOQUÉ | Code et déploiement Coolify faits (PR 102/107/109 fusionnées) ; serveur relais jamais provisionné = décision de dépense de Matt + restauration Contabo ; puis une connexion par écran par Matt | Matt (décision dépense) |
| R-92 | Construire les 6 sites vides (popoulet.ca, bmbd.ca, tacomontreal.ca, ocrepe.ca, nutrishake.ca, inntime.ca) + corriger ooeuf.ca (M-14) | OUBLIÉ | Briefs déposés en issues nº 1 des dépôts le 2026-10-31 ; constructions jamais commencées | Taktak / dev |
| R-93 | 7 domaines en attente : deliaden.ca expiré le 2026-10-17 + 6 jamais commandés (mythosgo.ca, pitalibanais.ca, pouletexpress.ca, pizzaalgerie.ca, placeafrique.ca, dejeunermontreal.ca) | BLOQUÉ | Paiement = geste de Matt seulement | Matt (paiement) |
| R-94 | M-36 — Dashboard SEO « Tac Attack » (clone Jumper, dans takatak-v1, issue nº 236) | BLOQUÉ | Spec déposée (Drive 1yWclmaDiVDWu7m0V9P93z-2SP-MfrMgN) ; compte DataForSEO activé par Matt (solde 1 $) ; restes chez Matt : accès API Google Business Profile, plafond budget données, liste de lancement ; appel Jumper confirmé lun. 2026-11-02 08:40 EST (événement kcsjpashp8mq0csm5k35d2d938) | Matt (inputs) |
| R-95 | TAKATAK Review — système d'avis maison (spec interface Yelp Reviews déposée) | OUBLIÉ | Spec : GitHub TAKATAKREVIEW docs (commit 65e2f1f1) + Drive 1En3qy6JyelYWzJ0bWyaq7AHL0klARbh7 ; issue nº 2 ; le système lui-même n'a jamais été bâti. (La demande de fausses reviews croisées a été REFUSÉE en permanence — non-fait assumé, pas un oubli.) | Taktak / dev |
| R-96 | M-32 — Dashboard social maison (clone Brandwatch, SOCIO propriétaire produit) | OUBLIÉ | Spec déposée (Drive 1htX8f6tnZyP4L8Jnep1MX5ziD42U3T24 + annexe 1neNOK2kV8vOytL-o4ZHmUD9MtZdV-1jB ; ordre d'exécution sur issue QUADROHOLDING nº 3) ; réponse signée de SOCIO et exécution dev jamais arrivées | SOCIO |
| R-97 | Sécurité M-15 : .env toujours à la racine du dépôt PUBLIC deli-aden-online ; knowledgeAI toujours public ; rotation des secrets Alkao (issue nº 84) non cochée | BLOQUÉ | Plan d'action déposé (Drive 1hUB5AZ4KZhHEM4vc1qwPRalgFSFSV8cKvC) ; exécution = décisions de visibilité + rotations de Matt/dev ; **jeton GitHub expire vers le 2026-11-04 — geste de Matt urgent** | Matt (décisions) |
| R-98 | M-33 — Vidéos choc TAKATAK.CA (production SOCIO ; logistique pixel/CAPI/GA4 avant toute pousse payante) | OUBLIÉ | Pack de scripts déposé (Drive 1hCc4uRzT-5K4cvXufN3I8jNGfot2EP3j) ; production jamais lancée ; nommer de vrais compétiteurs = décision de Matt seule | SOCIO |
| R-99 | M-34 — Widget panneau latéral MIMT.ca + besoinavocat.ca (TWILO) | EN COURS | Paquet d'intégration besoinavocat.ca livré et confirmé au Drive le 2026-10-31 22:46 ; déploiement bloqué par l'accès serveur ; intégration MIMT ensuite ; **capture d'écran règle nº 13 de TWILO toujours manquante** (route manuelle à faire) | TWILO |
| R-100 | M-29 — Notifications push marketing (board de consentement + campagnes à déclencheurs) | OUBLIÉ | Spec déposée (Drive 14saAtBXyt8SF6o85cH6jKx2EEdEgJFdF ; issue qmaps nº 9) ; implémentation jamais commencée | Dev / QMAPS |
| R-101 | QMAPS — cloner le tableau de bord marchand type Yelp for Business | OUBLIÉ | Spec déposée (GitHub qmaps, issue nº 8 ; Drive 16FZsfiaGoGOz0ubnipReOmqOnBWWcLhG) ; implémentation jamais commencée | Dev / QMAPS |
| R-102 | Support TAKATAK « IA en premier » + système maître unique + départements type DoorDash (ordres de Matt du 2026-10-27) | OUBLIÉ | Spécifié dans les paroles de Matt du 2026-10-27 ; jamais bâti, jamais transformé en mission étampée | Taktak / dev |
| R-103 | TR4CKER (application chauffeur maison, tiers 50/100/150 $) | OUBLIÉ | Ordonné le 2026-10-27 ; jamais bâti (hors la fiche Clover en draft, R-63) | Dev |
| R-104 | Google Wallet (carte cadeau + points) sur pppmtl.com et les sites resto | OUBLIÉ | Ordonné le 2026-10-27 ; jamais fait | Dev PPP |
| R-105 | Pop-up d'accueil PPP + vidéo checkout « Track my order » 3–5 s (issues pppmtl nº 16 et suivantes) | OUBLIÉ | Ordonnés le 2026-10-27 ; jamais faits | Dev PPP |
| R-106 | M-31 — App mobile R2NETTE (parité Housecall Pro, Happy APPY) | EN COURS | Spec A–Z déposée (issue r2neet nº 48 ; Drive 1Urj0cCdbnZpsEafM-fCHqEMO684UhzQA) ; Happy APPY n'a jamais répondu ; connexion bancaire Housecall Pro = geste de Matt seul | Happy APPY / Matt |
| R-107 | COMPANY-INFORMATION — redistribution GitHub : 12/20 dépôts non poussés | BLOQUÉ | Drive 19/19 fait ; GitHub 8/20 poussés ; 12 cartes d'approbation REFUSÉES — respectées, jamais réessayées ; relance = approbation de Matt (rapport A2 : Drive 1iH0ZVkqxTKVfAMNEEq8KSdOkiXj_5PLb) | Matt (approbations) |
| R-108 | M-20 — MIMT : AdSense refusé (site soumis à identifier + 5 correctifs), AdMob à finaliser | BLOQUÉ | Matt doit nommer le site soumis à AdSense ; resubmit = son clic après correctifs | Matt (information) |
| R-109 | M-21 / M-22 — analyses de spécialisation + relectures anti-refus de Claude et ChatGPT | OUBLIÉ | Assignées le 2026-10-29 dans le « 00 — TO-DO LIST — HUMAIN » ; jamais déposées | Claude / ChatGPT |
| R-110 | Send-as matt@takatak.ca | BLOQUÉ | 2FA désactivée sur takatak.agency = blocage structurel ; garé par Matt | Matt (garé) |

### I. Finances

| Nº | Item | Statut | Preuve / blocage | Propriétaire |
|---|---|---|---|---|
| R-111 | Fichier maître des frais plateformes (Uber + Skip + DoorDash) | FAIT | 15 753,44 $ documentés, 15 168,80 $ réclamés ; GitHub QUADROHOLDING docs/FRAIS-PLATEFORMES-FICHIER-MAITRE.md (commit 6666d7e295843d4791b4df0a3381e1b75f435dac) ; Drive Opérations 1F7FxFKiT9r76MiPXbeY60jRqhS8CD4Zo ; Drive Comptabilité 1J0gieaxVDnU-K5GSfReZdIuJGWTSVxz7 | Taktak |
| R-112 | Extractions de frais : DoorDash D1 (7 923 messages, 101 PDF uniques) ; Skip (35 CSV) ; Uber (R-28) | FAIT | D1 : rapport signé + ZIP Drive 10k48AkAPS58fjftwj5oL-FPWy_RnLFpN ; Skip : ~/workspace/skip-fees-extraction/ ; Uber : ~/workspace/uber-fees-extraction/ | Taktak |
| R-113 | Classeur maître BMO ↔ plateformes (apparier chaque transaction BMO aux relevés Uber/DoorDash/Skip) | BLOQUÉ | Ordonné le 2026-11-01 02:50 (accès BMO complet accordé, lecture seule) ; extraction bloquée à la page de connexion BMO Entreprises — déblocage = Matt se connecte DANS l'onglet Muse laissé ouvert ; matière Uber + Skip déjà extraite et prête | Matt (connexion) |
| R-114 | Déclarations TPS/TVQ — échéance 2026-11-02 | BLOQUÉ | « FINANCE GO » de Matt requis ; numéros au dossier (COMPANY-INFORMATION amendée le 2026-10-31) | Matt (go) |
| R-115 | Reformulation des promos plateformes (doctrine : petits spéciaux diversifiés par section, non cumulables, avec protections) | BLOQUÉ | Audits FAITS (Uber : 11 campagnes ; DoorDash : 35 campagnes) ; la reformulation attend les chiffres de Matt — aucun changement sans son approbation (promos = argent) | Matt (chiffres) |
| R-116 | Avis de paiement CNESST du 2026-10-30 (montant inconnu) ; entente Fiserv (Pierre) ; échec de paiement Superhuman 40 $ | EN COURS | Items ouverts consignés ; montants/gestes à confirmer | Taktak / Pierre |

### J. Juridique / REQ / Organisation / Divers

| Nº | Item | Statut | Preuve / blocage | Propriétaire |
|---|---|---|---|---|
| R-117 | REQ — saisir les 20 noms d'entreprise préparés par Claude (NOMS-A-SAISIR-REQ) | BLOQUÉ | Liste prête (Drive 1OEyppZ9MDlzq73ICXOnGnb0AqUoLTOEC, dossier 1g0ay1ugFg2DRLFHkU3gNOuwBrfXcT9DC) ; clicSÉQUR refusé code 21423 (Mon bureau non activé) — déblocage = appel de Matt au 418 659-2281 ; extrait public consolidé Drive 1w6cuQuZUNAwAwzWbicVbOwoHgHw-A5wA ; DMA 2026 due avant le 2027-01-01 | Matt (appel) |
| R-118 | Too Good To Go (P19) — extraction + réécritures des 16 magasins | EN COURS | Partiel fait le 2026-11-01 01:42 (chaîne, OOEUF NDG complet + réécritures, OOEUF Jean-Talon partiel ; note Drive 12sOqp2j6beO3NEzVzKeZodcwTxXYAGSb) ; reste : paniers Jean-Talon 27 $/33 $, 14 magasins, onglets Pricing/Permissions — reprise = nouvelle fenêtre MyStore ouverte par Matt ; aucun lien public n'existe au portail (constat vérifié) | Matt (fenêtre) |
| R-119 | Réponse à Shehroz Mehmood (WhatsApp du 2026-10-27 : domaines gardés sous reseller Mochahost) | OUBLIÉ | Signalé le 2026-10-27 ; réponse jamais confirmée | Taktak |
| R-120 | Rapport Phase 2 de LesGroupes | OUBLIÉ | Dû depuis le 2026-10-31 01:42 ; relancé aux supervisions 05:10/05:40/06:10/08:10 ; toujours rien ; aucun courriel de plevesquemtl@gmail.com depuis le 2026-10-27 | LesGroupes / Lévesque |
| R-121 | Retours de Lévesque sur M-08 (nettoyage Uber nº 13), M-09 (9 corrections Bolon SL), M-10 (images Clover) | OUBLIÉ | Transmis le 2026-10-29 ; aucun retour au 2026-11-01 | Lévesque |
| R-122 | PC de Matt à apparié à Muse (nettoyage de fichiers + miroir Drive local) | BLOQUÉ | Seul son téléphone est apparié ; installation + appairage sur le PC = geste de Matt | Matt (geste) |
| R-123 | Questions « propriétaire » du check-in Claude du 2026-11-01 07:45 (vente MIMT, abonnements Stripe, voix) | EN COURS | Rapportées par Claude, non vérifiées par Taktak ; portées aux agents dans le fil du jour | Matt (réponses) |
| R-124 | Identité des alertes de connexion Meta/Microsoft du 2026-10-29 et Facebook du 2026-10-30 | EN COURS | Question ouverte laissée en inbox exprès aux passes Gmail | Matt (confirmation) |
| R-125 | Nom de l'agent dev PPP (à confirmer par Matt) ; existence d'un 4e compte Facebook (message de Matt coupé le 2026-10-31 23:11) | BLOQUÉ | Deux confirmations jamais reçues | Matt (confirmation) |
| R-126 | Organisation multi-agents : thread unique quotidien, registre, journal, règles d'or nº 11/12/13, liste de tâches numérotée | FAIT | En vigueur et vérifiés en continu (supervisions aux 30 min, relectures aux 30 min, rapports horaires ; fil du jour 2026-11-01 = 1a1954f63654da5c) | Taktak |
| R-127 | Boîte Gmail takatak.ca@gmail.com — passes de tri M-12 | FAIT | Passe finale pour le réveil du 2026-11-02 terminée le 2026-11-01 02:44 : 1 497 → 1 207 messages, 292 étiquetés + archivés, 0 suppression, 0 envoi | Taktak |
| R-128 | Mission courriel « tout répondre » (167 fils balayés) | FAIT | Rapport signé du 2026-10-31 ; envois autorisés faits : Contabo, Too Good To Go, Adel Sani (msg 1a193cbade7cbe69), Dane Bettridge (msg 1a193cc862638648) | Taktak |

---

## LISTE COMPLÈTE DES OUBLIÉS (39) — le cœur de la relance de Matt

*Oublié = ordonné par Matt, jamais fait ou jamais fini, sans blocage qui l'explique entièrement. R- = renvoi au tableau.*

1. **R-04** — Création des ~8–10 Pages Facebook restantes (route Casa jamais relancée après les refus Meta du 2026-10-31) — LesGroupes.
2. **R-07** — Post épinglé « 6241 » des Pages PPP jamais dépinglé/remplacé — SOCIO.
3. **R-08** — Page PPP NDG « Always open » jamais corrigée à 16 h–3 h — SOCIO.
4. **R-09** — Monétisation Facebook 100 % (M-30) : aucune activation vérifiée par Page ; gabarits de pub maison dans les reels jamais proposés — SOCIO.
5. **R-10** — Ménage du mur personnel de Matt + tri de ses photos en albums — jamais repris après la fenêtre morte du 2026-10-25 — Taktak.
6. **R-11** — **Visuels Uber (bannière/header/logo) jamais appliqués aux Pages Facebook ni aux réseaux** — relance expresse de Matt le 2026-11-01 10:15 — SOCIO/Lévesque.
7. **R-14** — Modèle courriel des 18 marques (M-23) jamais produit par SOCIO (consigne du 2026-10-30).
8. **R-15** — TripAdvisor (M-26) : fiches des 18 marques jamais créées/lienées, aucun rapport revenu — SOCIO.
9. **R-27** — Adresse du magasin Uber nº 14 Pizza Algérie jamais corrigée (vivant au 6280, canonique 5839) — Lévesque.
10. **R-34** — **Confrontations portail DoorDash jamais faites** (Po Poulet : troncature/assiettes ; Gâteau : écart vitrine) — des relectures texte à la place, pendant des jours — Taktak.
11. **R-41** — Réponse due à Hailin (cas 774709330) jamais préparée — Codex/Taktak.
12. **R-42** — Réponse due à l'équipe Photos DoorDash (cas 773996517) jamais préparée — Codex/Taktak.
13. **R-49** — 3 rapports DoorDash téléchargés le 2026-10-28 jamais récupérés au Drive — Taktak.
14. **R-53** — Courriel propre de chaque marque jamais posé sur 30/41 inscriptions Skip — Taktak.
15. **R-54** — **Menus Skip jamais alignés au catalogue v3** (ancien menu de 175 items, heures fausses) — Lévesque.
16. **R-56** — Lettre de réclamation des frais Skip (584,64 $/semaine) jamais préparée — Taktak.
17. **R-60** — Adresse d'en-tête Clover 6284 jamais corrigée à 6280 — Lévesque.
18. **R-61** — « Boisson » → « breuvage » dans 12/18 descriptions de Trios Clover jamais corrigé/revérifié — Lévesque.
19. **R-62** — 5 images d'items Clover (M-10) jamais produites — Lévesque.
20. **R-71** — Merchant Center : approbation des 198 produits jamais reprise (0 approuvé) — Taktak.
21. **R-73** — Compte détenteur des fiches O'oeuf Somerled/Jean-Talon jamais identifié pour la liaison MC — Taktak.
22. **R-75** — Yelp des autres marques jamais fait (seul PPP traité) — Lévesque.
23. **R-79** — Foursquare O'oeuf/Bolon toujours au 6241 avec de mauvais téléphones — Taktak.
24. **R-89** — Garde /dev de pppmtl jamais déployée (page d'audit interne publique) — dev PPP.
25. **R-90** — Alerte fraude : paquet prêt depuis le 2026-10-30, jamais déployé — Taktak.
26. **R-92** — 6 sites de marques jamais construits (briefs seulement) — Taktak/dev.
27. **R-95** — TAKATAK Review : système d'avis maison jamais bâti (spec seulement) — Taktak/dev.
28. **R-96** — M-32 dashboard social : réponse SOCIO et exécution jamais arrivées — SOCIO.
29. **R-98** — M-33 vidéos choc : production jamais lancée — SOCIO.
30. **R-100** — M-29 notifications push : implémentation jamais commencée — dev/QMAPS.
31. **R-101** — QMAPS : clone du dashboard marchand jamais implémenté — dev/QMAPS.
32. **R-102** — Support TAKATAK « IA en premier » + système maître + départements (2026-10-27) jamais bâtis ni étampés — Taktak/dev.
33. **R-103** — TR4CKER jamais bâti — dev.
34. **R-104** — Google Wallet sur pppmtl.com et les sites jamais fait — dev PPP.
35. **R-105** — Pop-up PPP + vidéo checkout 3–5 s jamais faits — dev PPP.
36. **R-109** — Analyses M-21 (Claude) et M-22 (ChatGPT) jamais déposées depuis le 2026-10-29 — Claude/ChatGPT.
37. **R-119** — Réponse à Shehroz Mehmood (domaines Mochahost) jamais confirmée — Taktak.
38. **R-120** — Rapport Phase 2 de LesGroupes jamais livré (dû depuis le 2026-10-31) — LesGroupes.
39. **R-121** — Retours de Lévesque M-08/M-09/M-10 jamais reçus depuis le 2026-10-29 — Lévesque.

*Cas particulier — R-12 (posts quotidiens Canva) : oublié jusqu'à la relance du 2026-11-01 10:15, relancé le jour même (étape 1 en cours) ; il est donc compté EN COURS, pas OUBLIÉ, mais il appartient à la même famille de relances que R-11 et que la présente réconciliation (les 3 chantiers P20/P21/P22 de Matt).*

---

## RESTE À FINIR — par propriétaire

**Matt (gestes/décisions seulement) :** R-03 vérifications de portefeuilles Meta · R-22 « send » du retrait Jean-Talon · R-23 décision prix pizzas nº 16 · R-24 route support nº 4 Uber · R-40 choix de pièces + « send » relance DoorDash · R-43 adresse de Yan Romanowski · R-45 documents de réactivation Gâteaux NDG · R-50 régénération des rapports mensuels · R-55 code 2 étapes Skip · R-67 vérification du marchand Clover désactivé · R-68 Google Business (GARÉ, à rouvrir par lui) · R-72 appel de la suspension GBP O'oeuf · R-74 gestes Yelp (app + photo) · R-76 geste mot de passe Yelp O'oeuf · R-77 décision Wikidata · R-83 décision Birdeye · R-84 réponse Contabo Rescue · R-85 clics Stripe (Link + réautorisation) · R-86 compte Twilio · R-87 choix Interac · R-91 décision dépense serveur relais Food Hub · R-93 paiement des 7 domaines · R-94 inputs M-36 (API GBP, budget, liste) · R-97 décisions sécurité M-15 + **jeton GitHub avant le ~2026-11-04** · R-106 connexion bancaire Housecall Pro · R-107 approbations des 12 pushes COMPANY-INFORMATION · R-108 nommer le site AdSense · R-113 connexion BMO dans l'onglet Muse · R-114 « FINANCE GO » TPS/TVQ (échéance 2026-11-02) · R-115 chiffres des promos · R-117 appel clicSÉQUR 418 659-2281 (code 21423) · R-118 fenêtre MyStore TGTG · R-122 appairage du PC · R-123 réponses au check-in Claude · R-124 identité des alertes de connexion · R-125 nom du dev PPP + 4e compte Facebook.

**Taktak :** R-05 trancher le statut des renommages par relecture Meta · R-10 ménage du profil personnel · R-25 appel support Uber (renommages, via edit/send) · R-34 confrontations portail (avec la fenêtre DoorDash) · R-41/R-42 préparer les 2 réponses DoorDash dues (edit/send, une à la fois) · R-46/R-111/R-112 matière du classeur (prête, attend R-113) · R-49 rapports navigateur · R-53 courriels Skip à l'onboarding · R-56 préparer la lettre Skip · R-57 écart taxes Skip · R-71 produits Merchant Center · R-73 compte détenteur des fiches O'oeuf · R-78/R-79 citations Cylex/Foursquare · R-90 déployer l'alerte fraude dès Contabo restauré · R-119 réponse Shehroz · R-48 relance Gerlin si silence prolongé.

**Lévesque (restaurants) :** R-21 onboarding des 22 magasins Uber + leads détournés · R-26 finir les magasins 90–95 % · R-27 adresse Pizza Algérie · R-54 menus Skip v3 · R-60/R-61/R-62 restes Clover marchand · R-75 Yelp des autres marques · R-121 livrer M-08/M-09/M-10.

**LesGroupes (autres entreprises) :** R-02 acceptations Casa · R-04 créer les Pages restantes sur Casa · R-06 recyclage BP Taekwondo · R-120 rapport Phase 2.

**SOCIO (sociaux) :** R-07 post « 6241 » · R-08 heures PPP NDG · R-09 monétisation M-30 · R-11 visuels Uber → Pages/réseaux · R-12 posts quotidiens Canva (avec Taktak) · R-14 modèle courriel M-23 · R-15 TripAdvisor M-26 · R-16 contrôles Facebook · R-65 vidéos Clover (avec Taktak) · R-96 réponse M-32 · R-98 production M-33.

**Claude :** R-109 analyse M-21. **ChatGPT :** R-109 reformulations M-22. **Codex :** R-41/R-42 (avec Taktak). **TWILO :** R-99 déploiement widget + capture règle nº 13. **Dev PPP :** R-88 PR/rebase · R-89 garde /dev · R-104/R-105 Wallet, pop-up, vidéo checkout. **Happy APPY :** R-106 répondre et bâtir l'app R2NETTE. **Dev/QMAPS :** R-100/R-101 implémentations.

---

## NOTE D'APRÈS — dépôts de cette passe (signé Taktak)

- Le présent document est inscrit dans le **fichier maître** (section « RÉCONCILIATION 2026-11-01 » ajoutée en place, copie locale) et sa copie Drive est mise à jour **en place** (ID 16d0HAHtKXnqhckLPCodFHLiBl_VSf7QU).
- Poussé sur **GitHub takatakca/QUADROHOLDING** sous `docs/RECONCILIATION-2026-11-01.md` (poussée UTF-8 via l'intégration ; commit vérifié en direct après poussée — le hachage est consigné au registre et dans la note signée « 2026-11-01 — Réconciliation et fichier maître terminés — signé Taktak.md », déposée au Drive Opérations 11B5CeNU_lZgO2VFA_fzejoLJNkSZdnv- avec le présent document).
- Sécurité du livrable : ce document a été re-greppé avant poussée (mêmes motifs que la note d'avant) — aucune valeur de secret, aucun jeton, aucun code, aucune date de naissance ; seuls des noms de variables et des constats en prose y figurent.
- Aucun courriel envoyé, aucune plateforme modifiée, aucun paiement fait dans cette passe. takatak-v1 : lecture seule respectée (aucune écriture).

— Taktak, 2026-11-01
