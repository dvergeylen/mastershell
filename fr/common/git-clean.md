---
layout: default
title: "git clean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-clean">
  <a href="/fr/common/git-clean.html">git clean</a> <a href="#git-clean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Supprimer les fichiers non-suivis d'un dépôt Git.
> Plus d'informations : <https://git-scm.com/docs/git-clean>.

#### Supprimer les fichiers non-suivis :
```shell
git clean
```
#### Supprimer les fichiers non-suivis de manière interactive :
```shell
git clean -i
```
#### Affiche les fichiers non-suivis qui peuvent être supprimés :
```shell
git clean --dry-run
```
#### Nettoyage forcé des fichiers non-suivis :
```shell
git clean -f
```
#### Nettoyage forcé des répertoires non-suivis :
```shell
git clean -fd
```
#### Supprime tous les fichiers suivis, incluant ceux répertoriés par `.gitignore` et `.git/info/exclude` :
```shell
git clean -x
```
{% endraw %}