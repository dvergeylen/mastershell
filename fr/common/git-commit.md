---
layout: default
title: "git commit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-commit">
  <a href="/fr/common/git-commit.html">git commit</a> <a href="#git-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enregistrer (`commit`) les fichiers dans le dépôt.
> Plus d'informations : <https://git-scm.com/docs/git-commit>.

#### Commit les fichiers en stage dans le dépôt avec un message :
```shell
git commit -m "{{message}}"
```
#### Commit tous les fichiers modifiés avec un message :
```shell
git commit -am "{{message}}"
```
#### Met à jour le dernier commit avec les modifications en stage :
```shell
git commit --amend
```
#### Commit seulement les fichiers spécifiés (qui sont déjà en stage) :
```shell
git commit {{chemin/vers/mon/fichier1}} {{chemin/vers/mon/fichier2}}
```
{% endraw %}