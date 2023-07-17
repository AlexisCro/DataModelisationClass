# Modelisation de donnée (Merise, MLD, MCD, MPD)

## Merise
### Introduction

C'est une méthode de modélisation de données.

Merise est un acronyme : Méthode d'Etude et de Réalisation Informatique pour les Systèmes d'Entreprise. 

Elle se caractérise par trois points clés:
  - une approche dite systémique :

    transformation des processus de l'entreprise en système d'information 

  - une séparation des données et des traitements
  - une approche nivelée

### L'approche systémique

![schéma systémique](./img/modelisation/syst%C3%A9mique.png)

#### Définitions
 - Système de pilotage :

    Les preneurs de décisions (patrons, cadres, managers, ...)

 - Système d'information :

    Les employers de l'entreprise.

 - Le système opérant :
    
    Il est composé de l'ensemble des acteurs produisant les données du système d'information


### La séparation des donnees et des traitements

La séparation des données et des traitements permet de séparer les données du système d'information et les traitements effectuées sur les données. 

Cette démarche de fait en 3 étapes :
- L'analyse des flux : on analyse les flux d'informations entre les acteurs du système d'information et les acteurs du système opérant
- L'étude des documents interne (factures, bon de livraison, ...)
- L'étude des documents externes (fournisseurs, clients, ...)

Les différents types d'informations :
- les infos de bases ou élémentaires : ce sont les données de base du système d'information. 
- les infos calculées : ce sont les données calculées à partir des données de base
- les traitements ou les fonctions (actions) : ce sont les traitements effectuées sur les données de base pour obtenir les données calculées. 

### Niveau conceptuel
Permet de modéliser les données de l'entreprise. 
On utilisera le modèle conceptuel de données **(MCD)** pour modéliser les données de l'entreprise et le MCT pour modéliser les traitements de ces données.

### Niveau organisationnel
Il va permettre d'intégrer à l'analyse précédente toutes les notions de temporalités, chronologie des opérations, de contraintes. 

On va utiliser le modèle organisationnel des traitememnts **(MOT)** et le modèle organisationnel des données **(MOD)** pour modéliser les traitements.

A partir des données recueillis au niveau conceptuel on se pose ces questions : 
- **Quand** les traitements sont-ils effectués ? 
- **Où** les traitements sont-ils effectués ? 
- **Qui** effectue les traitements ?

### Le niveau logique

Le niveau logique va permettre de modéliser les data de l'entreprise en utilisant le **MLD** et les traitements de l'entreprise en utilisant le **MLT**

Le **MLD** est indépendant des languages de prog et **SGBD**

On répond à la question **Avec quoi** les traitements sont effectués ?

### Le niveau physique

Il s'agit dde l'organisation réelle des data. 

On va utiliser le modèle physique de data **MPD** et le modèle physique des traitements **MPT**

On répond à la question **Commment** on effectue les traitements ?

### **Resumé**
Nous avons donc 4 niveaux
- Conceptuel
- Organisationnel
- Logique
- Physique

### Des données aux dépendances fonctionnelles

Pour être intégrées dans un système d'information, les données doivent être triées et organisées. On va souvenat tenter de les classer par type de données :
- string
- alphanum
- integer, float
- date
- boolean

### Création d'un dictionnaire de data
![dico data](./img/modelisation/dico_data.png)

[Exercice modelisation donnée facture](./Exercice/dictionnaire_data.md)

### Les dépendances fonctionnelles

Une dépendence est une relation entre deux attributs d'une table. Elle permet de définir une relation de dépendance entre deux attriibuts d'une table. 

#### Exercice
Elaborer un MCD à partir d'un dictionnaire de données.
 
[Enoncer exercice](./Exercice/image-14.png)
![modélisation exercice](./img/modelisation/Exercice/restaurant.jpg)

#### Quelques définitions 
Propriétés : sont les info de base d'un SI

Entité : c'est une table

Relation : définis par des verbes d'actions  

Cardinalité : 1.N, N.N, 0.N, 0.1, 1.1