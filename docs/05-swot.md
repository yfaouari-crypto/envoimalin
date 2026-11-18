# 5. SWOT (TD 7 · « Faire équipe »)

Le TD demande un SWOT **individuel** puis un SWOT **d'équipe** pour ce projet. Nous ajoutons un SWOT du **produit** pour préparer la soutenance.

*Forces et faiblesses = interne (nous). Opportunités et menaces = externe (l'environnement).*

## SWOT individuels

### Youssef · Product Owner + développeur

| Forces | Faiblesses |
|---|---|
| Parcours économie-gestion : à l'aise avec les notions de finance (taux de change, frais, marges) | Arrivé en MIAGE en L3 : moins de pratique en développement |
| Connaît le problème de l'intérieur (envois d'argent entre la France et la Tunisie) | Porte à la fois le rôle de PO et une grande partie du développement : risque de surcharge |
| Expérience en développement commercial et lancement de produit| |
| Sens du produit et de la présentation | |

| Opportunités | Menaces |
|---|---|
| Projet directement lié à son projet professionnel en finance | Plusieurs projets et examens en même temps sur le semestre |
| Montrer un site réellement utilisable, pas une simple maquette | Dépendance à des sources de données externes |

### Ariel · Scrum Master

| Forces | Faiblesses |
|---|---|
| Parcours économie-gestion : à l'aise avec les notions de finance | Arrivé en MIAGE en L3 : moins de pratique en développement |
| Organisation et suivi : tient le Kanban et le rythme des cérémonies | Rôle de Scrum Master découvert pendant ce projet |
| Regard extérieur au code : repère ce qui n'est pas clair pour un utilisateur | Moins impliqué dans la partie technique |
| Connaît les envois d'argent depuis la Côte d'Ivoire | |

| Opportunités | Menaces |
|---|---|
| Développer des compétences de gestion de projet agile, très demandées | Si les cérémonies sont sautées, perte de visibilité sur l'avancement |

### Imhotep · Lead technique

| Forces | Faiblesses |
|---|---|
| Parcours économie-gestion : à l'aise avec les notions de finance | Arrivé en MIAGE en L3 : moins de pratique en développement |
| Rigueur : relecture du code et vérification des calculs | N'a pas écrit la majorité du code : doit le relire en profondeur pour le maîtriser |
| Attention à la fiabilité des données | |

| Opportunités | Menaces |
|---|---|
| Expérience concrète des tests et de la qualité logicielle | Peu de temps pour relire si les développements arrivent en fin de sprint |

> Ces SWOT individuels ont été rédigés à partir de nos rôles. Chacun peut les compléter avec ses propres points.

## SWOT de l'équipe

| Forces | Faiblesses |
|---|---|
| Toute l'équipe vient d'économie-gestion : à l'aise avec la finance (taux, frais, marges) | Tous arrivés en MIAGE en L3 : peu de pratique du développement |
| Rôles complémentaires : produit (Youssef), organisation (Ariel), qualité (Imhotep) | Équipe de 3, alors que le TD conseille 4 à 6 personnes : chacun porte plusieurs casquettes |
| Deux membres connaissent personnellement les envois d'argent à l'étranger (Tunisie pour Youssef, Côte d'Ivoire pour Ariel) | Le code dépend beaucoup d'une seule personne |
| Site en ligne, qui fonctionne avec des données réelles | Peu d'expérience préalable de Scrum |
| Règles claires : Definition of Done, relecture croisée | |

| Opportunités | Menaces |
|---|---|
| Sujet concret et original, qui se démontre en quelques secondes | Délai court avant la soutenance |
| Données publiques disponibles : taux du jour, tarifs des services, études de la Banque mondiale | Les sources de données peuvent changer ou s'arrêter |
| Outils gratuits : GitHub, GitHub Pages, CryptPad | Absence ou indisponibilité d'un membre |

**Actions décidées à partir de ce SWOT**
- Contre la dépendance à une seule personne : relecture systématique du code par Imhotep, et documentation dans le dépôt.
- Contre la fragilité des sources : une seconde source de taux et une solution de secours pour les tarifs.
- Contre le délai court : un MVP clair (Sprint 2) avant les fonctionnalités de confort.

## SWOT du produit EnvoiMalin

| Forces | Faiblesses |
|---|---|
| Montre le coût total, marge cachée comprise, et pas seulement les frais affichés | Ne transfère pas l'argent : l'utilisateur doit ensuite aller sur le site du service |
| Tarifs relevés en direct, service par service, avec leur date | Les tarifs viennent du comparateur d'un acteur (Wise) qui figure lui-même dans la liste |
| Toutes les devises, calcul dans les deux sens | Pas de tarif publié pour certaines paires (devises soumises au contrôle des changes) |
| Gratuit, sans compte, aucune donnée personnelle collectée | |

| Opportunités | Menaces |
|---|---|
| Forte demande de transparence : le coût moyen d'un envoi reste de 6,49 % dans le monde (Banque mondiale, 2025) | Comparateurs déjà installés sur le marché |
| Objectif international de ramener ce coût à 3 % d'ici 2030 | Évolution de la réglementation des comparateurs |
| Diaspora importante en France (près de 700 000 Tunisiens, selon LesAfriques.com) | Changement ou fermeture des sources de données |
