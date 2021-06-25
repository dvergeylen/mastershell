---
layout: default
title: "git stash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-stash">
  <a href="/fr/common/git-stash.html">git stash</a> <a href="#git-stash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stocker les modifications Git locales dans une zone temporaire.
> Plus d'informations : <https://git-scm.com/docs/git-stash>.

#### Stocker les changements courants, sauf les fichiers non-suivis :
```shell
git stash [push -m {{nom_de_stash_optionel}}]
```
#### Stocker les changements courants, incluant les fichiers non-suivis :
```shell
git stash -u
```
#### Stocker les parties d'un fichier interactivement :
```shell
git stash -p
```
#### Lister tous les stashs (affiche leurs noms, les branches relatives et messages) :
```shell
git stash list
```
#### Applique un stash (par défaut, le dernier, nommé stash@{0}) :
```shell
git stash apply {{nom_de_stash_ou_de_commit_optionel}}
```
#### Applique un stash (par défaut le dernier, stash@{0}), et le supprimer de la liste des stashs s'il n'y a pas de conflit :
```shell
git stash pop {{nom_de_stash_optionel}}
```
#### Supprime un stash (par défaut le dernier, stash@{0}) :
```shell
git stash drop {{nom_de_stash_optionel}}
```
#### Supprime tous les stashs :
```shell
git stash clear
```
{% endraw %}