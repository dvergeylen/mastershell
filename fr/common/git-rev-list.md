---
layout: default
title: "git rev-list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rev-list">
  <a href="/fr/common/git-rev-list.html">git rev-list</a> <a href="#git-rev-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Liste les révisions (commits) dans l'ordre chronologique inverse.
> Plus d'informations : <https://git-scm.com/docs/git-rev-list>.

#### Lister tout les commits dans la branche courante :
```shell
git rev-list {{HEAD}}
```
#### Lister tout les commits plus récents qu'une date spécifique, sur une branche spécifique :
```shell
git rev-list --since={{'2019-12-01 00:00:00'}} {{master}}
```
#### Lister tout les commits de merge depuis un commit spécifique :
```shell
git rev-list --merges {{commit}}
```
{% endraw %}