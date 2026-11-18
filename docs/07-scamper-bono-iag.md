# 7. SCAMPER, 6 chapeaux de Bono et IAG (TD 8)

## Objectif de la réflexion

**Le sujet** : un comparateur des frais d'envoi d'argent à l'étranger.

**Le but** :
- Comment améliorer l'idée ? Rendre visible le coût **réel** d'un envoi, marge cachée comprise.
- Comment résoudre le problème ? Donner, en quelques secondes, le service qui fait perdre le moins d'argent.
- Comment améliorer une fonctionnalité ? Rendre la comparaison fiable pour **toutes** les devises, pas seulement l'euro vers le dirham.

## SCAMPER

| Lettre | Question | Notre réponse | Décision |
|---|---|---|---|
| **S** · Substituer | Qu'est-ce qui pourrait être remplacé ? | Remplacer les frais relevés à la main, vite périmés, par des **tarifs relevés automatiquement** pour chaque service. | ✅ Fait (Sprint 2) |
| **C** · Combiner | Que combiner pour multiplier les usages ? | Combiner le **taux réel du jour**, les **tarifs des services** et les **moyennes de la Banque mondiale** dans un seul écran. | ✅ Fait |
| **A** · Adapter | Quels changements pour un autre contexte ? | Adapter l'outil aux **étudiants en échange** (euro vers dollar canadien, livre…), pas seulement à la diaspora : d'où toutes les devises. | ✅ Fait (Sprint 3) |
| **M** · Modifier | Que modifier pour l'améliorer ? | Afficher le **coût total** au lieu des seuls frais, et l'**économie sur un an** pour rendre l'enjeu concret. | ✅ Fait |
| **P** · Proposer | Quels autres usages ? | Calculer **l'inverse** (« ils doivent recevoir 5 000 MAD ») ; à terme, une **alerte de taux**. | ✅ Calcul inverse · Alerte en V2 |
| **E** · Éliminer | Que retirer pour simplifier ? | Supprimer la **création de compte** et le champ « fréquence » : moins de saisie, aucune donnée personnelle. | ✅ Fait |
| **R** · Réorganiser | Comment réorganiser pour être plus efficace ? | Placer « Vous envoyez » et « Ils reçoivent » **côte à côte** avec une flèche d'échange, et classer du moins cher au plus cher. | ✅ Fait (Sprint 3) |

## Les 6 chapeaux de Bono

Chacun a porté un ou deux chapeaux pendant la séance.

| Chapeau | Rôle | Ce qui a été dit |
|---|---|---|
| ⚪ **Blanc** · les faits | Données objectives | Coût moyen d'un envoi : 6,49 % dans le monde, 14,55 % par une banque (Banque mondiale, 2025). Des comparateurs de tarifs existent déjà. Certaines devises ne s'envoient pas librement (contrôle des changes). |
| 🔴 **Rouge** · les émotions | Ressenti | Frustration de découvrir qu'on a perdu 30 € sur un envoi « sans frais ». Méfiance envers les petits caractères. Besoin d'être rassuré : « est-ce que ma mère va bien recevoir la somme ? » |
| ⚫ **Noir** · la prudence | Risques | Les tarifs changent vite. Les données viennent d'un acteur du marché (Wise), pas d'un organisme neutre. Certaines paires n'ont aucun tarif. On ne doit pas laisser croire que le site transfère l'argent. |
| 🟡 **Jaune** · l'optimisme | Avantages | Gratuit, rapide, sans compte. Économie concrète : plusieurs centaines d'euros par an pour un envoi mensuel. Un argument fort à l'oral. |
| 🟢 **Vert** · la créativité | Idées nouvelles | Calcul inverse, flèche d'échange, recherche de devise par pays, alerte de taux, installation sur téléphone. |
| 🔵 **Bleu** · l'organisation | Synthèse | On garde le MVP centré sur le coût total. On traite le chapeau noir : date de chaque relevé, source affichée, solution de secours, mention claire « EnvoiMalin ne transfère pas d'argent ». Le reste va en V2. |

**Ce que la séance a changé** : le chapeau noir nous a poussés à afficher partout la **source et la date** des tarifs, et à prévoir un **affichage de secours** quand aucun tarif n'existe.

## IAG et créativité

Nous avons utilisé une IA générative (Claude) en appliquant les conseils du TD : beaucoup d'idées, des exemples, un score de créativité (CSCORE) et des contraintes inhabituelles.

**Prompt 1 · brainstorming avec exemples**
> « Nous faisons un site fintech qui compare les frais d'envoi d'argent à l'étranger. Exemples d'idées déjà trouvées : afficher la marge cachée, calculer l'économie sur un an. Propose 15 fonctionnalités nouvelles. Prends en compte le CSCORE dans ta réponse : de 1 (réponses basiques) à 10 (réponses très créatives). Vise un CSCORE de 8. »

Meilleurs résultats retenus :
- calcul inverse « combien envoyer pour qu'ils reçoivent X » → **US08, fait** ;
- recherche d'une devise par le nom du pays → **US10, fait** ;
- alerte quand le taux dépasse un seuil choisi → **US16, V2** ;
- historique du taux sur 30 jours pour choisir le bon moment → **US15, V2**.

**Prompt 2 · contrainte inhabituelle**
> « Imagine que notre site doit être utilisable par une grand-mère qui n'a jamais utilisé d'application bancaire, en moins de 10 secondes. Qu'est-ce que tu enlèves ? CSCORE 7. »

Résultats retenus : un seul écran, deux champs côte à côte, aucune inscription, le meilleur choix mis en évidence → appliqué dans la **réorganisation de l'écran** (Sprint 3).

**Prompt 3 · jeu de rôle**
> « Tu es un professeur de finance très exigeant. Critique notre projet en 5 points. »

Critiques retenues :
1. « D'où viennent vos chiffres ? » → source et date affichées pour chaque tarif.
2. « Votre source est un concurrent » → nous le disons clairement sur le site.
3. « Que se passe-t-il pour le dinar vers l'euro ? » → encadré explicatif et affichage de secours.

**Notre regard critique sur l'IAG** : elle aide à produire beaucoup d'idées vite, mais elle peut inventer des chiffres. Nous n'avons gardé que des données vérifiées dans une source citée.
