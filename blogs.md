# LES BLOGS #

## Oragnisation du blog ##

Suite à la génération du blog, Jekyll a créé le minimum pour le générer. 


### Le fichier _config ###

contient la configuration générale du blog.

### le dossier _layout ###

contient les templates qui serviront à générer les pages. 

### Le dossier _post ###

contient les articles.

### le dossier _site ###
contient le blog généré. C’est ce dossier qu’il faudra placer sur le serveur pour publier le blog.

## Créer des articles ##  

Les post peuvent être écris en Markdown ou en Textile.
Pour ajouter un article, il faut créer un fichier :
ANNEE-MOIS-JOUR-titre.md ou ANNEE-MOIS-JOUR-titre.textile (par exemple 2013-03-10-Titre-de-mon-article.md). 
Les pages commence par quelques lignes de YAML pour la configuration. Les formats Markdown et Textile sont simples, il n’y a pas de code HTML à écrire, le code est généré lors de la génération de la page.

### Exemple ###

---
published: true
layout: post
title: "Tutoriel : Créer un blog statique avec Jekyll"
category: jekyll
---
#### Mon titre en H4 ####
Bonjour, je suis un article, 
je peux avoir des mots en _italique_, 
d'autres en **gras** et des [liens](http://www.jekyllrb.com).


## Création de pages ##

Pour créer une page, il faut placer un fichier HTML à la racine du projet. Lors de la génération du blog, ce fichier sera placé dans le dossier _site.

## Template ##

Le principe est d’avoir des fichiers html dans le dossier _layouts. Le fichier default.html contient par exemple la structure des pages (balise head, …). Le contenu des pages sera copier à l’emplacement de la variable content :

{{ content }}

Il y a un système d’héritage très simple entre les templates. Par exemple le fichier post.html hérite du fichier default.html