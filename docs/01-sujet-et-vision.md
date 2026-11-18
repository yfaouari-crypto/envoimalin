# 1. Sujet et vision produit (TD 6 · atelier 2)

## Le sujet

Le projet du semestre demande une solution informatique qui relève de la **fintech** : utiliser la technologie pour rendre un service financier plus simple, plus transparent ou plus accessible.

Notre sujet : **EnvoiMalin, un comparateur des frais d'envoi d'argent à l'étranger.**

## Le problème

Quand on envoie de l'argent à sa famille à l'étranger, on paie deux choses :

1. **les frais affichés** (par exemple 4,99 €) ;
2. **une marge cachée sur le taux de change** : le service applique un taux moins bon que le taux réel, et garde la différence.

La deuxième partie ne se voit presque jamais. Beaucoup de services annoncent « 0 € de frais » et se rémunèrent uniquement sur le taux. Résultat :

- selon la Banque mondiale, envoyer de l'argent coûte en moyenne **6,49 %** du montant dans le monde, et **14,55 %** en passant par une banque (rapport *Remittance Prices Worldwide* n° 53, mars 2025) ;
- vers le Maroc, sur un envoi de 1 000 €, l'écart entre le service le moins cher et le plus cher peut atteindre **environ 80 €** (comparatif Wafir.ma, mai 2026).

## La cible

| Persona | Situation | Ce qu'il veut savoir |
|---|---|---|
| **Karim, 21 ans, étudiant tunisien à Bordeaux** | Reçoit de l'argent de ses parents chaque mois | Quel service fait perdre le moins d'argent à sa famille |
| **Nadia, 45 ans, salariée, diaspora marocaine** | Envoie 300 à 500 € par mois à sa mère | Combien sa mère reçoit vraiment, et où |
| **Lucas, 23 ans, en échange au Canada** | Envoie ponctuellement des euros vers le dollar canadien | Si sa banque ou un service en ligne est moins cher |

## La solution

Un site web, simple et gratuit :

1. on indique le montant et les deux devises (toutes les devises du monde sont disponibles) ;
2. le site affiche, **service par service**, ce que le bénéficiaire reçoit vraiment : frais, marge cachée, taux appliqué, coût total ;
3. il classe les services du moins cher au plus cher et montre l'économie possible sur un an.

Le calcul inverse est aussi possible : « mes proches doivent recevoir 5 000 dirhams, combien dois-je envoyer ? ».

## Vision produit (en une phrase)

> **Pour** les personnes qui envoient de l'argent à leurs proches à l'étranger,
> **qui** perdent de l'argent sans le savoir à cause des marges cachées sur le taux de change,
> **EnvoiMalin est** un comparateur en ligne
> **qui** montre le montant réellement reçu, frais et marge compris, pour chaque service.
> **Contrairement aux** sites des services eux-mêmes, qui mettent en avant leurs propres frais,
> **notre produit** rend visible le coût total et l'affiche de façon neutre.

## Pourquoi c'est de la fintech

- **Transparence financière** : rendre visible un coût caché (la marge de change).
- **Données financières en temps réel** : taux de change du jour et tarifs des services relevés automatiquement.
- **Inclusion financière** : aider des personnes qui envoient de petits montants, pour qui chaque euro compte.

## Ce que le site ne fait pas (choix assumé)

EnvoiMalin **ne transfère pas d'argent**. Transférer de l'argent exige un agrément d'établissement de paiement délivré par l'ACPR. Le site compare, puis renvoie vers le service choisi.
