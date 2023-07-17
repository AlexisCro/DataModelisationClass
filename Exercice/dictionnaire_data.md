#### Exercice

| Name data | Format | Longueur | Type (élémentaire ou calculé) | Règle de calcul | Règle de gestion | Document |
| --- | --- | --- | --- | --- | --- | --- |
|nom_société| string | 255 | élémentaire | | | |
Adresse sociétée |string | 255 | élémentaire | | | | 
| tel_entreprise | alphanumérique | 20 | élémentaire | | | |
email_entreprise | alphanumérique | 255 | élémentaire | | | |
| nom client | string | 255 |élémentaire | | | |
adresse_client | alphanumérique | 255 | élémentaire | | | | 
| email_client | alphanumérique | 255 | élémentaire | | | |
| N° client | alphanumérique | 255 | calculé | concaténation | "client n°" + id du client | table client pour trouver id |
|numéro_fature | alphanumérique | 255 | calculé | concaténation | "facture n°" + id_facture | table facture pour l'id |
| date_facture | date |  | élémentaire | | | |
| échéance en jour | integer | | élémentaire | | | |
|date fin échéance | date | | calculé | somme | date_facture + échéance en jour |
| nom_article | string | 255 | élémentaire | | | |
| taille_article | string | 255 | élémentaire | | | |
| quantité_article | integer | | élémentaire | | | |
| article_prix_unitaire | float | | élémentaire | | | |
| article_prix_unitaire_HT | float | | élémentaire | | | |
| article_montant | float | |calculé | multiplication | quantité_article * article_prix_unitaire | |
| total_HT | float | | calculé | somme | somme des prix articles HT | |
| accompte | float | | élémentaire | | | |
| net à payer | float | | calculé | soustraction | total - accompte | |

