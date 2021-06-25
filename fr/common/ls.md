---
layout: default
title: "ls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ls">
  <a href="/fr/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Liste le contenu d'un répertoire.
> Plus d'informations : <https://www.gnu.org/software/coreutils/ls>.

#### Liste les fichiers, un par ligne :
```shell
ls -1
```
#### Liste tous les fichiers, ainsi que les fichiers cachés :
```shell
ls -a
```
#### Liste tous les fichiers avec un format détaillé (permissions, propriétaire, taille et date de modification) :
```shell
ls -la
```
#### Liste les fichiers avec un format détaillé en utilisant des préfixes d'unités (KiB, MiB, GiB) :
```shell
ls -lh
```
#### Liste les fichiers avec un format détaillé en triant par taille décroissante :
```shell
ls -lS
```
#### Liste avec un format détaillé tous les fichiers en triant par date de modification (les plus anciennes en premier) :
```shell
ls -ltr
```
{% endraw %}