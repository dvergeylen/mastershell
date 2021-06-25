---
layout: default
title: "git status"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-status">
  <a href="/fr/common/git-status.html">git status</a> <a href="#git-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Affiche les changements sur les fichiers dans la branche courante.
> Affiche les fichiers édités, déplacés, renommés, ajoutés, supprimés par rapport à la référence de la branche courante.
> Plus d'informations : <https://git-scm.com/docs/git-status>.

#### Affiche les fichiers modifiés qui n'ont pas encore été ajoutés pour le commit :
```shell
git status
```
#### Affiche les fichiers modifiés (version courte) :
```shell
git status -s
```
#### Affiche les fichiers modifiés, sans tenir des comptes des fichiers non-suivis :
```shell
git status --untracked-files=no
```
#### Affiche les fichiers modifiés (version courte) avec les informations de branche :
```shell
git status -sb
```
{% endraw %}