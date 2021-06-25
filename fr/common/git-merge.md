---
layout: default
title: "git merge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-merge">
  <a href="/fr/common/git-merge.html">git merge</a> <a href="#git-merge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pour fusionner des branches `git`.
> Plus d'informations : <https://Pour fusionner des docs `git`/git-merge>.

#### Fusionne une branche dans votre branche courante :
```shell
git merge {{nom_de_branche}}
```
#### Editer le message de fusion (`merge commit`) :
```shell
git merge -e {{nom_de_branche}}
```
#### Fusionner une branche et créer un commit de fusion (`merge commit`) :
```shell
git merge --no-ff {{nom_de_branche}}
```
#### Annuler une fusion en cas de conflit :
```shell
git merge --abort
```
#### Continuer une fusion après une résolution de conflit :
```shell
git merge --continue
```
{% endraw %}