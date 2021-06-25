---
layout: default
title: "git show"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-show">
  <a href="/fr/common/git-show.html">git show</a> <a href="#git-show"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Affiche différents types d'objets Git (commits, tags, etc.).
> Plus d'informations : <https://git-scm.com/docs/git-show>.

#### Afficher des informations sur le dernier commit (hachage, message, modifications et autres métadonnées) :
```shell
git show
```
#### Affiche les informations du dernier commit :
```shell
git show {{commit}}
```
#### Affiche les informations associés au tag spécifié :
```shell
git show {{etiquette}}
```
#### Affiche les informations à propos du 3ème commit en partant du sommet de la branche :
```shell
git show {{branche}}~{{3}}
```
#### Afficher le message d'un commit sur une seule ligne, en supprimant la sortie diff :
```shell
git show --oneline -s {{commit}}
```
#### Affiche uniquement la liste des fichiers changés dans un commit :
```shell
git show --stat {{commit}}
```
#### Afficher le contenu d'un fichier tel qu'il était à une révision donnée (par exemple, branche, tag ou commit) :
```shell
git show {{revision}}:{{chemin/vers/fichier}}
```
{% endraw %}