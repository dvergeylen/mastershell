---
layout: default
title: "git remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-remote">
  <a href="/fr/common/git-remote.html">git remote</a> <a href="#git-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Organisation des dépôts suivis ("remotes").
> Plus d'informations : <https://git-scm.com/docs/git-remote>.

#### Affiche les dépôts existants, leur nom et URL :
```shell
git remote -v
```
#### Affiche les informations à propos d'un dépôt :
```shell
git remote show {{nom_distant}}
```
#### Ajoute un dépôt :
```shell
git remote add {{nom_distant}} {{url_distant}}
```
#### Change l'URL d'un dépôt (ajouter `--add` pour conserver l'URL existante) :
```shell
git remote set-url {{nom_distant}} {{new_url}}
```
#### Supprime un dépôt :
```shell
git remote remove {{nom_distant}}
```
#### Renomme un dépôt :
```shell
git remote rename {{old_name}} {{new_name}}
```
{% endraw %}