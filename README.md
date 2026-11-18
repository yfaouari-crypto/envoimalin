# EnvoiMalin

**Combien vos proches reçoivent vraiment ?**

EnvoiMalin compare les frais d'envoi d'argent à l'étranger. Pour chaque service (banques et services de transfert), il affiche le montant réellement reçu, **marge cachée sur le taux de change comprise**, et classe les services du moins cher au plus cher.

**Site en ligne :** https://yfaouari-crypto.github.io/envoimalin/

**Kanban du projet (lecture seule) :** [tableau Scrum sur CryptPad](https://cryptpad.fr/kanban/#/2/kanban/view/SQKf5+G0nboPRSnDIh6vCJ5spxdjhNDs3P7iaa6pfS4/)

Projet de semestre : Licence 3 MIAGE, Université de Bordeaux, méthode agile Scrum (Prof. R. Berty), 2026-2027.

---

## Le problème

Beaucoup de services affichent « 0 € de frais » mais appliquent un taux de change moins bon que le taux réel. Cette marge ne se voit pas. Selon la Banque mondiale, envoyer de l'argent coûte en moyenne **6,49 %** du montant, et **14,55 %** par une banque (mars 2025).

## Ce que fait le site

- **Toutes les devises** (153), au départ comme à l'arrivée, avec une barre de recherche (code, nom ou pays).
- **Taux réel du jour**, mis à jour automatiquement.
- **Comparaison service par service** avec des tarifs relevés en direct : frais, taux appliqué, marge cachée, coût total, montant reçu, date du relevé.
- **Calcul dans les deux sens** : « j'envoie 500 € » ou « ils doivent recevoir 200 000 francs CFA (XOF) ».
- **Flèche d'échange** des deux devises en un clic.
- **Filtre** banques / services de transfert.
- **Économie** sur l'envoi et sur un an, et **graphique** du coût total.
- **Solution de secours** quand aucun service ne publie de tarif pour une paire (par exemple TND → EUR, à cause du contrôle des changes).

EnvoiMalin **ne transfère pas d'argent** et ne collecte **aucune donnée personnelle**.

## Documentation du projet (TD 6, 7 et 8)

| Document | Contenu |
|---|---|
| [1. Sujet et vision](docs/01-sujet-et-vision.md) | Problème, personas, vision produit, pourquoi c'est de la fintech |
| [2. Équipe, rôles et rythmes](docs/02-equipe-roles-rythmes.md) | Rôles Scrum, cérémonies, Definition of Done, règles du Kanban |
| [3. Backlog](docs/03-backlog.md) | User stories, MoSCoW, valeur et difficulté, critères d'acceptation |
| [4. Sprints](docs/04-sprints.md) | Sprint 0 à 4 : tâches, reviews, rétrospectives, Daily Scrum, démo |
| [5. SWOT](docs/05-swot.md) | SWOT individuels, d'équipe et du produit |
| [6. Brainstorming et PESTEL](docs/06-brainstorming-pestel.md) | Idées, choix du sujet, grille PESTEL |
| [7. SCAMPER, Bono et IAG](docs/07-scamper-bono-iag.md) | Questionner et améliorer le sujet |
| [8. Données et calculs](docs/08-donnees-et-calculs.md) | Formules, sources, cas de secours, limites |

## Équipe

| Membre | Rôle |
|---|---|
| Youssef Hmidi | Product Owner + développeur : a développé et mis en ligne le site |
| Ariel | Scrum Master |
| Imhotep | Lead technique : relecture du code, tests, fiabilité des données |

Sprints de 2 semaines · Daily Scrum le lundi, le mercredi et le vendredi · [Kanban sur CryptPad](https://cryptpad.fr/kanban/#/2/kanban/view/SQKf5+G0nboPRSnDIh6vCJ5spxdjhNDs3P7iaa6pfS4/).

## Choix techniques

| Élément | Choix | Pourquoi |
|---|---|---|
| Site | Une page HTML, CSS et JavaScript | Simple, rapide, rien à installer |
| Taux de change | ExchangeRate-API, avec une source de secours | Taux du jour gratuit, sans clé |
| Tarifs des services | Comparateur public de Wise | Tarifs relevés auprès de chaque service, avec leur date |
| Hébergement | GitHub Pages | Gratuit, lien public, aucun serveur à maintenir |
| Données personnelles | Aucune | Pas de compte ; seuls les derniers choix sont gardés dans le navigateur |

## Limites et version 2

- Les tarifs viennent du comparateur de Wise, qui figure lui-même dans la comparaison. Le site le dit clairement et renvoie vers le site officiel de chaque service.
- Certaines paires de devises n'ont aucun tarif publié : le site affiche alors une estimation et l'explique.
- **V2** : historique du taux sur 30 jours, alerte de taux, installation sur téléphone, filtre par mode de réception (compte, espèces, mobile).
