# 8. Données et calculs

## Les formules

Pour un service donné :

- **Frais** = frais fixes + frais en % × montant envoyé
- **Taux appliqué** = taux réel × (1 − marge)
- **Montant reçu** = (montant envoyé − frais) × taux appliqué
- **Marge cachée** = (montant envoyé − frais) × marge, exprimée dans la devise d'envoi
- **Coût total** = frais + marge cachée

**Calcul inverse** (montant à recevoir X connu) :
montant à envoyer = (X ÷ taux appliqué + frais fixes) ÷ (1 − frais en %)

**Exemple vérifié à la main** : 1 000 € vers le Maroc, taux réel 10,85, frais de 4,15 €, sans marge.
(1 000 − 4,15) × 10,85 = 995,85 × 10,85 = **10 804,97 MAD**, comme dans le comparatif publié (10 805 MAD).

## D'où viennent les données

| Donnée | Source | Mise à jour |
|---|---|---|
| Taux de change réel | [ExchangeRate-API](https://www.exchangerate-api.com) (secours : base de devises publique de fawazahmed0 sur jsDelivr) | Chaque jour |
| Tarifs de chaque service | Comparateur public de Wise : frais, marge, taux et montant reçu relevés auprès de chaque banque et service de transfert | En continu, avec la date de chaque relevé |
| Relevés manuels EUR → MAD et EUR → TND | Wafir.ma, LesMRE.com, DémarchesÉtrangers.fr, LesAfriques.com, Wise, JeChange.fr d'après la Banque mondiale | Utilisés seulement en secours |
| Coûts moyens par type de service | Banque mondiale, *Remittance Prices Worldwide* n° 53 (mars 2025) | Utilisés seulement en secours |

## Ce que fait le site selon les cas

1. **Des tarifs existent pour la paire** → comparaison service par service, avec la date de chaque relevé.
2. **Aucun tarif publié** (par exemple TND → EUR, à cause du contrôle des changes) → un encadré l'explique, puis :
   - nos relevés manuels si la paire est EUR → MAD ou EUR → TND ;
   - sinon, les coûts moyens de la Banque mondiale par type de service, appliqués au taux réel du jour.
3. **Le service de tarifs ne répond pas** → même solution de secours.

## Limites assumées

- Les tarifs varient selon le pays d'envoi, le mode de paiement et les promotions : le site affiche le pays du relevé quand ce n'est pas la France, et renvoie toujours vers le site officiel du service.
- Les tarifs viennent du comparateur de Wise, qui est aussi un service comparé. Le site le dit clairement.
- Les moyennes de la Banque mondiale portent sur des envois de 200 $ : pour de plus gros montants, le coût en % est en général plus bas.
- EnvoiMalin ne transfère pas d'argent et ne touche aucune commission.
