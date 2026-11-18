# 6. Brainstorming et PESTEL (TD 7)

## Brainstorming

Règles respectées : 3 minutes d'idées libres, puis 3 minutes pour rebondir ; aucune critique ; la quantité et le « pillage » des idées des autres sont encouragés.

### Tour 1 · Idées libres

1. Comparateur des frais d'envoi d'argent à l'étranger
2. Chasseur d'abonnements oubliés (Netflix, salle de sport…)
3. Simulateur de prêt étudiant
4. Objectifs d'épargne étudiants (permis, voyage, ordinateur)
5. Factures et cotisations pour étudiants auto-entrepreneurs
6. Cagnotte de groupe pour un cadeau ou un voyage
7. Budget étudiant avec la règle 50/30/20
8. Carte de fidélité regroupant tous les commerces du campus
9. Jeu pour apprendre la bourse sans risque
10. Alerte quand une facture augmente

### Tour 2 · Rebonds

- Sur l'idée 1 : **montrer la marge cachée sur le taux de change**, pas seulement les frais.
- Sur l'idée 1 : **calcul inverse** : « ma mère doit recevoir 200 000 francs CFA ».
- Sur l'idée 1 : **alerte quand le taux devient intéressant**.
- Sur l'idée 2 : prévenir **avant** le prélèvement, pas après.
- Sur l'idée 4 : comparer **Livret A et compte courant** pour l'épargne.
- Sur l'idée 9 : utiliser les **vrais cours du jour**.

### Sujet retenu

**Le comparateur des frais d'envoi d'argent (idée 1 et ses rebonds).**

Pourquoi :
- c'est un vrai problème financier, chiffré par la Banque mondiale ;
- deux membres de l'équipe le vivent personnellement (envois entre la France et la Tunisie, et depuis la Côte d'Ivoire) ;
- c'est clairement de la fintech : transparence des coûts et données en temps réel ;
- il se démontre en quelques secondes ;
- il est réalisable dans le temps du semestre.

## Grille PESTEL

| | Ce qui touche notre sujet | Conséquence pour EnvoiMalin |
|---|---|---|
| **Politique** | Les pays du G20 visent un coût moyen des envois d'argent de 3 % maximum d'ici 2030. La Tunisie applique un contrôle des changes : le dinar ne s'envoie pas librement vers l'étranger. Le franc CFA de Côte d'Ivoire a un taux fixe avec l'euro (1 € = 655,957 XOF) : tout écart de taux est donc une marge du service. | Notre outil va dans le sens de cet objectif. Pour les paires soumises au contrôle des changes, le site explique pourquoi aucun tarif n'existe. |
| **Économique** | Envoyer de l'argent coûte en moyenne 6,49 % dans le monde et 14,55 % par une banque (Banque mondiale, mars 2025). Les taux de change bougent tous les jours. Pour beaucoup de familles, l'argent reçu est un revenu essentiel. | Il faut le taux du jour et des tarifs récents, sinon la comparaison est fausse. Montrer l'économie sur un an rend l'enjeu concret. |
| **Social** | Forte diaspora en France (près de 700 000 Tunisiens selon LesAfriques.com, et une importante communauté ivoirienne) et nombreux étudiants internationaux. Habitudes différentes : agence en espèces, application, virement bancaire. | Le site doit être très simple, en français, utilisable sur téléphone et sans compte. |
| **Technologique** | Développement des fintechs et des services 100 % en ligne. Des données publiques existent : taux de change du jour, tarifs relevés par des comparateurs. | Un site léger qui interroge ces données en direct, sans serveur à maintenir. |
| **Écologique** | Le numérique consomme de l'énergie. Un envoi en ligne évite un déplacement en agence. | Site en une seule page, sans bibliothèque lourde ni serveur ; hébergement statique sur GitHub Pages. |
| **Légal** | Transférer de l'argent exige un agrément d'établissement de paiement (ACPR). Les règles européennes imposent la transparence des frais. Le RGPD encadre les données personnelles. Les services appliquent des contrôles d'identité (lutte contre le blanchiment). | EnvoiMalin compare sans transférer, ne crée pas de compte et ne collecte aucune donnée personnelle. |

## Programmer son travail (TD 7 · point 4)

Le Kanban CryptPad reprend toutes les tâches du [backlog](03-backlog.md), avec pour chacune sa **valeur** et sa **difficulté**. Un exemple de Daily Scrum est dans le [déroulé des sprints](04-sprints.md).
