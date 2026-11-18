# 3. Backlog produit

Priorités en **MoSCoW** (Must, Should, Could, Won't). **Valeur** : intérêt pour l'utilisateur, de 1 à 5. **Difficulté** : points de complexité (suite de Fibonacci), estimés en planning poker.

## User stories

| US | En tant qu'utilisateur, je veux… | Priorité | Valeur | Difficulté | Sprint | État |
|---|---|---|---|---|---|---|
| US01 | saisir un montant et choisir la devise d'envoi et la devise de réception | Must | 5 | 3 | 1 | ✅ |
| US02 | voir le taux de change réel du jour | Must | 5 | 3 | 1 | ✅ |
| US03 | comparer les services : frais, taux appliqué, montant reçu | Must | 5 | 8 | 1 | ✅ |
| US04 | voir les services classés du moins cher au plus cher, avec un badge « Meilleur choix » | Must | 4 | 2 | 2 | ✅ |
| US05 | voir la marge cachée sur le taux de change, en montant et en % | Must | 5 | 3 | 2 | ✅ |
| US06 | voir la date du relevé de chaque tarif et un lien vers le site officiel du service | Should | 4 | 2 | 2 | ✅ |
| US07 | filtrer entre banques et services de transfert | Should | 3 | 2 | 2 | ✅ |
| US08 | calculer l'inverse : « mes proches doivent recevoir X, combien j'envoie ? » | Should | 4 | 5 | 3 | ✅ |
| US09 | échanger les deux devises en un clic | Should | 3 | 1 | 3 | ✅ |
| US10 | rechercher une devise par son code, son nom ou son pays | Should | 4 | 3 | 3 | ✅ |
| US11 | voir combien j'économise sur cet envoi et sur un an | Should | 4 | 2 | 3 | ✅ |
| US12 | voir un graphique du coût total de chaque service | Could | 3 | 3 | 3 | ✅ |
| US13 | avoir quand même une estimation quand aucun service ne publie de tarif pour ma paire de devises | Should | 3 | 5 | 4 | ✅ |
| US14 | utiliser le site confortablement sur mon téléphone | Must | 4 | 3 | 4 | ✅ |
| US15 | voir l'évolution du taux de change sur 30 jours | Could | 3 | 5 | V2 | — |
| US16 | recevoir une alerte quand le taux devient intéressant | Could | 3 | 8 | V2 | — |
| US17 | installer le site sur mon téléphone comme une appli | Could | 2 | 3 | V2 | — |
| US18 | filtrer selon le mode de réception (compte, espèces, mobile) | Could | 3 | 8 | V2 | — |
| US19 | envoyer l'argent directement depuis le site | Won't | — | — | — | Exclu |
| US20 | créer un compte pour garder mes envois habituels | Won't | — | — | — | Exclu |

**Pourquoi US19 et US20 sont exclues**
- **US19** : transférer de l'argent demande un agrément d'établissement de paiement (ACPR). Le site reste un comparateur neutre.
- **US20** : un compte imposerait de stocker des données personnelles (RGPD). Sans compte, le site n'en collecte aucune.

**Pourquoi US18 est en V2** : la source de données utilisée ne précise pas le mode de réception de chaque tarif.

## Critères d'acceptation des stories principales

**US01 · Montant et devises**
- Le montant accepte la virgule ou le point, avec au plus 2 décimales.
- Un montant vide, nul ou invalide affiche un message d'erreur clair.
- Toutes les devises en circulation sont proposées (153), l'euro et le dollar en premier.
- Choisir deux fois la même devise affiche un message.

**US02 · Taux réel**
- Le taux affiché est celui du jour, avec sa date de mise à jour.
- Si le service de taux ne répond pas, une source de secours prend le relais.

**US03 · Comparaison**
- Pour chaque service : frais, taux appliqué, marge cachée, coût total, montant reçu.
- Montant reçu = (montant envoyé − frais) × taux appliqué.
- Les tarifs sont relevés en direct pour la paire de devises choisie.

**US05 · Marge cachée**
- Marge cachée = (montant envoyé − frais) × marge en %.
- Elle est affichée en montant et en pourcentage, en rouge quand elle n'est pas nulle.

**US08 · Calcul inverse**
- Si l'utilisateur tape dans « Ils reçoivent », le site calcule le montant à envoyer pour chaque service.
- Le classement se fait alors du plus petit au plus grand montant à envoyer.

**US13 · Estimation de secours**
- Si aucun service ne publie de tarif pour la paire, un encadré l'explique.
- Le site affiche alors nos relevés manuels (EUR → MAD et EUR → TND) ou, à défaut, les coûts moyens de la Banque mondiale par type de service.

## Tâches transverses (toujours au backlog)

- Relire le code avant chaque mise en ligne (Imhotep).
- Vérifier un calcul à la main à chaque sprint (Imhotep).
- Tenir le Kanban et animer les cérémonies (Ariel).
- Mettre à jour le README et la documentation (Youssef).
