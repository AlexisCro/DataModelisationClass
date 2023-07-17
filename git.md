# GIT <img src="./img/logo_git.png">

## Introduction 

Git un est logiciel de versionning permettant de tracer les versions des projets et d'avoir des dépôts dit locals et distants afin de faciliter le travail en équipe. 

# Les commandes de bases
## Instanciation d'un projet GIT
### Init
```sh
git init
```
Cette commande permet d'instancier un dépôt GIT lorsqu'on est dans notre répertoire de notre projet. 
Cela va générer un répertoire <b>.git</b>

Si on ne veut plus que notre répertoire soit un projet git, alors il suffit de supprimer le répertoire <b>.git</b>

### Remote
```sh
git remote add <name> <url>
```
Cette commande permet de lier un dépôt distant à un dépôt local.

Exemple ici nous avons instancié un projet donc un dépôt git.
Au sein de github (ça peut être gitlab ou autre serveur de partage distant du même type), nous instancions un nouveau repertoire et nous lui donnons donc un nom :

Dans notre cas <b>DataModelisationClass</b>

Pour lier donc pour dépôt local à mon distant se situant sur Github j'entre la commande suivante : 
```sh
git remote add ModelisationData https://github.com/AlexisCro/DataModelisationClass.git
```

### Clone

Il se peut que l'on veuille récupérer un dépôt distant d'une équipe ou que nous ayons créé en premier le dépôt distant. Dans ce cas nous utiliserons 
```sh
git clone <url>
```
Pour cela on se place dans un répertoire qui sera celui de notre projet et on entre la commande cité ci-dessus. 

Le répertoire distant et tout les fichiers contenu dedans seront importés en local. 

## Status/Add/Commit/Push
### Status
Afin de connaitre le status de nos fichiers, donc si on a des modifications qui ont été effectuées et que nous n'avons pas enregistrer nous pouvons savoir quels fichiser cela concerne grâce à 
```sh
git status
```

En <em style="color:red;">rouge</em> les fichies non indexer seront affichés. 

En <em style="color:green;">vert</em> les fichiers indexés. 

Si un fichier n'est pas affiché c'est qu'il n'a pas eu de modification depuis le dernier commit (enregistrement).

### Indexer

Il y a trois étapes à connaître afin de pouvoir enregistrer les modifications apportés à nos fichiers. 

La première consiste à indexer (stage) et pour cela on utilise la commande 
```sh
git add
```

Cette commande prend différentes options.

```sh
git add . # index tout les fichiers ayant eu des modifications
git add <file_name> # index le fichier spécifier
git add -p # permet d'indexer de façon intéractive tout en affichant les aperçus avant/après
```

### Commit

Après avoir indexer nos fichiers il faut les sauvegarder on dit alors qu'on commit nos fichiers. 

Cela crée un point de sauvegarde dans notre branche (notre ligne temporelle de notre projet).

La commande est la suivante :
```sh
git commit
```

Cela ouvrira un éditeur de texte de type vim pour donner un titre à notre commit. 

Pour ne pas passer par l'éditeur vim utiliser l'option <b>-m</b>.

```sh
git commit -m "titre de mon commit"
```

### Push

Enfin pour mettre à jour notre dépôt distant il faut alors push (pousser) nos données. 

```sh
git push
```

Notre dépôt distant est alors à jour avec notre dépôt local :v: :+1:

