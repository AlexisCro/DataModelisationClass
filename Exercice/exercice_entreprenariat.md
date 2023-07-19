# Exercice entreprenariat

## Enoncé

[Enoncé exercise](./Exercice_3.docx)

## Dictionnaire de données

| Nom data | format | longueur | type (élémentaire/calculé) | règle de calcul | règle de gestion | source |
| --- | --- | --- | --- | --- | --- | --- |
| coordonnée client | varchar | 255 | élémentaire | | | table client |
| prénom client | varchar | 255 | élémentaire | | | table client |
| nom client | varchar | 255 | élémentaire | | | table client |
| DDN client | date |  | élémentaire | | | table client |
| tel client | varchar | 255 | élémentaire | | | table client |
| mail client | varchar | 255 | élémentaire | | | table client |
| nom matériel | varchar | 255 | élémentaire | | | table materiel |
| type d'intervention | varchar | 255 | élémentaire | | | table intervention |
| taux horaire | float | | élémentaire | | | table taux_horaire |
| description intervention | varchar | 255 | élémentaire | | | table intervention |
| début intervention | datetime | 255 | élémentaire | | | table intervention |
| fin intervention | datetime | 255 | élémentaire | | | table intervention |
| durée intervention | datetime | 255 | calculé | différence entre début et fin d'intervention | fin intervention - début intervention | table intervention |
| RefComposant | alphanuméric | 255 | élémentaire |  |  | table composant |
| Prix Composant HT | float | | élémentaire |  |  | table composant |
| Prix Composant TTC | float | | calculé | Prix HT soumis à la TVA | Prix HT * TVA | table composant |
| Taux TVA | float | | élémentaire | |  | table TVA |

## MCD

![MCD](image-1.png)

## MLD

![Alt text](image-2.png)
