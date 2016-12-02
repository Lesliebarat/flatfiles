---
---

# GIT #

Un outil de dévellopement collaboratif

## Présentation ##

GitHub est un service web d'hébergement et de gestion de développement de logiciels, utilisant le logiciel de gestion de versions Git. Ce site est développé en Ruby on Rails et Erlang par Chris Wanstrath, PJ Hyett et Tom Preston-Werner. 

## Fonctions ##

GitHub est centré vers l'aspect social du développement. Il offre l'hébergement de projets avec Git. GitHub offre aussi la possibilité de créer un wiki et une page web pour chaque dépôt. Le site offre aussi un logiciel de suivi de problèmes. GitHub propose l'intégration d'un grand nombre de services externes, tels que l'intégration continue, la gestion de versions, badges, chat basés sur les projets, etc.

Les documentations des projets sont écrites en langage Markdown (fichiers .md).

## Commandes Git ##

### Status des fichiers ###

$ git status

### Lister les branchs ###

$ git branch

### Créer une branch ###

$ git branch nom_de_ma_branch

### Changer de branch ###

$ git checkout nom_de_ma_branch

### Premier commit ###

$ git add .
$ git commit - m "initial commit"

### Commit suivant ###

$ git add chemin_vers_mon_fichier
$ git commit -m "message du commit"

### Annuler le dernier commit et modifs ###

$ git reset --hard md5_commit
$ git push --force

### Mettre à jour le dépôt local ###

$ git pull

### Envoyer ses commits vers le dépôt distant ###

$ git push

### Supprimer un fichier du répertoire de travail et de l'index ###

$ git rm nom_du_fichier

