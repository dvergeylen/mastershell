---
layout: default
title: "git add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-add">
  <a href="/fr/common/git-add.html">git add</a> <a href="#git-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ajoute les fichiers modifiés à l'index.
> Plus d'informations : <https://git-scm.com/docs/git-add>.

#### Ajouter un fichier à l'index :
```shell
git add {{chemin/vers/fichier}}
```
#### Ajouter tous les fichiers (suivis et non-suivis) :
```shell
git add -A
```
#### Ajoute les modifications des fichiers déjà suivis :
```shell
git add -u
```
#### Ajoute aussi les fichiers ignorés :
```shell
git add -f
```
#### Ajoute des parties de fichiers interactivement :
```shell
git add -p
```
#### Ajoute interactivement les parties d'un fichier spécifié :
```shell
git add -p {{chemin/vers/fichier}}
```
#### Ajouter un fichier interactivement :
```shell
git add -i
```
{% endraw %}