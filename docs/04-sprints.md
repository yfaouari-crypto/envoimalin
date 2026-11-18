# 4. Déroulé des sprints

Sprints de 2 semaines. Pour chaque sprint : l'objectif, ce qui a été livré, ce qu'on montre en review et ce qu'on retient en rétrospective.

| Sprint | Objectif | User stories | Points |
|---|---|---|---|
| Sprint 0 | Préparer le projet | — | — |
| Sprint 1 | La base : un premier comparateur qui marche | US01, US02, US03 | 14 |
| Sprint 2 | Le MVP : comparer et comprendre le coût réel | US04, US05, US06, US07 | 9 |
| Sprint 3 | Rendre l'outil pratique au quotidien | US08, US09, US10, US11, US12 | 14 |
| Sprint 4 | Fiabiliser et finaliser | US13, US14 + tests, README, présentation | 8 |

## Sprint 0 · Préparation

| Tâche | Qui |
|---|---|
| Lire l'énoncé et résumer les objectifs | Tous |
| Brainstorming et choix du sujet ([TD 7](06-brainstorming-pestel.md)) | Tous |
| SWOT individuel et d'équipe ([TD 7](05-swot.md)) | Tous |
| Analyse PESTEL du sujet ([TD 7](06-brainstorming-pestel.md)) | Tous |
| Rédiger la vision produit ([sujet](01-sujet-et-vision.md)) | Youssef |
| Écrire et estimer les user stories (planning poker) | Tous |
| Prioriser le backlog en MoSCoW | Youssef |
| Fixer le calendrier des cérémonies | Ariel |
| Créer le Kanban CryptPad | Ariel |
| Relever les frais réels des services et choisir les sources de données | Imhotep + Youssef |
| Rédiger la Definition of Done | Tous |
| Créer le dépôt GitHub et mettre le site en ligne | Youssef |

**Rétrospective** : on garde le planning poker, qui a fait émerger les vraies difficultés (la récupération des tarifs). À améliorer : décider plus tôt des sources de données.

## Sprint 1 · La base

**Tâches** : formulaire montant + devises ; appel au service de taux du jour ; premier tableau de comparaison ; formule du montant reçu.

**Review** : on saisit 500 €, on choisit le dinar tunisien, et le site affiche le taux du jour et le montant reçu pour chaque service.

**Rétrospective** : on garde la vérification des calculs sur un exemple fait à la main. À améliorer : les frais saisis à la main deviennent vite faux. Action : chercher une source de tarifs mise à jour automatiquement.

## Sprint 2 · Le MVP

**Tâches** : tri du moins cher au plus cher ; badge « Meilleur choix » ; calcul et affichage de la marge cachée ; date du relevé et lien officiel ; filtre banques / services de transfert ; branchement des tarifs en direct.

**Review** : sur 1 000 € envoyés en Côte d'Ivoire, le site montre l'écart entre le service le moins cher et le plus cher, et combien chacun prend en marge cachée.

**Rétrospective** : objectif tenu. À améliorer : penser aux paires de devises sans tarif publié (par exemple du dinar tunisien vers l'euro).

## Sprint 3 · Pratique au quotidien

**Tâches** : calcul inverse ; flèche d'échange des devises ; recherche de devise ; carte d'économie (envoi et année) ; graphique du coût total.

**Review** : « Ma mère doit recevoir 200 000 francs CFA » : le site donne le montant à envoyer pour chaque service. La flèche inverse EUR et TND en un clic.

**Rétrospective** : on garde la relecture croisée. À améliorer : tester plus tôt sur téléphone.

## Sprint 4 · Fiabiliser et finaliser

**Tâches** : solution de secours quand aucun tarif n'existe (relevés manuels puis moyennes Banque mondiale) ; seconde source de taux ; tests sur téléphone ; README ; documentation ; préparation de la soutenance.

**Review** : démonstration complète, y compris un cas sans tarif publié (TND → EUR), expliqué à l'écran.

**Rétrospective** : US15 à US18 restent au backlog pour une V2.

## Exemple de Daily Scrum (TD 7 · point 4)

| Membre | Hier | Aujourd'hui | Blocage |
|---|---|---|---|
| Youssef | Branché les tarifs en direct (US03) | Calcul inverse (US08) | Aucun |
| Ariel | Mis à jour le Kanban, préparé la review | Tester le site sur téléphone (US14) | Aucun |
| Imhotep | Relu le code de la marge cachée (US05) | Vérifier 3 calculs à la main | Paires sans tarif : à traiter (US13) |

## Scénario de démonstration (3 minutes)

1. Ouvrir le site : 500 € vers le dinar tunisien. Le classement s'affiche avec les tarifs du jour.
2. Ouvrir la fiche du premier et du dernier service : frais, marge cachée, date du relevé.
3. Montrer la carte « Économie sur un an ».
4. Choisir le franc CFA (XOF) et taper dans « Ils reçoivent » : 200 000. Le site calcule ce qu'il faut envoyer.
5. Chercher « roupie » dans la liste des devises, puis échanger les devises avec la flèche.
6. Choisir TND → EUR : montrer l'encadré qui explique pourquoi aucun service ne publie de tarif.
