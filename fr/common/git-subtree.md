---
layout: default
title: "git subtree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-subtree">
  <a href="/fr/common/git-subtree.html">git subtree</a> <a href="#git-subtree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil pour gérer les dépendances de projet en tant que sous-projets.
> Plus d'informations : <https://manpages.debian.org/testing/git-man/git-subtree.1.en.html>.

#### Ajout d'un dépôt Git en tant que sous-arbre :
```shell
git subtree add --prefix={{chemin/vers/repertoire/}} --squash {{repository_url}} {{master}}
```
#### Mettre à jour le sous-arbre avec son dernier commit :
```shell
git subtree pull --prefix={{chemin/vers/repertoire/}} {{repository_url}} {{master}}
```
#### Merge le dépot d'un sous arbre dans la branche master :
```shell
git subtree merge --prefix={{chemin/vers/repertoire/}} --squash {{repository_url}} {{master}}
```
#### Pousser les commits vers le dépôt d'un sous-arbre :
```shell
git subtree push --prefix={{chemin/vers/repertoire/}} {{repository_url}} {{master}}
```
#### Extraire un nouvel historique de projet de l'historique d'un sous-arbre :
```shell
git subtree split --prefix={{chemin/vers/repertoire/}} {{repository_url}} -b {{nom_de_branche}}
```
{% endraw %}