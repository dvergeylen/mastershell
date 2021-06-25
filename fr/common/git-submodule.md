---
layout: default
title: "git submodule"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-submodule">
  <a href="/fr/common/git-submodule.html">git submodule</a> <a href="#git-submodule"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inspecter, mettre à jour et manager des sous-modules.
> Plus d'informations : <https://git-scm.com/docs/git-submodule>.

#### Installer un sous-module depuis le dépôt courant :
```shell
git submodule update --init --recursive
```
#### Ajout d'un dépôt Git en tant que sous-module :
```shell
git submodule add {{repository_url}}
```
#### Ajout d'un dépôt Git en tant que sous-module à un répertoire donné :
```shell
git submodule add {{repository_url}} {{chemin/vers/repertoire}}
```
#### Mettre à jour tout les sous-modules à leur dernier commit :
```shell
git submodule foreach git pull
```
{% endraw %}