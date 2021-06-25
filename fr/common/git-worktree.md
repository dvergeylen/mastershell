---
layout: default
title: "git worktree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-worktree">
  <a href="/fr/common/git-worktree.html">git worktree</a> <a href="#git-worktree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gérer plusieurs arbres de travail attachés au même dépôt.
> Plus d'informations : <https://git-scm.com/docs/git-worktree>.

#### Créer un nouvel arbre de travail avec une branche spécifiée :
```shell
git worktree add {{chemin/vers/répertoire}} {{branche}}
```
#### Créer un nouvel arbre de travail avec une nouvelle branche :
```shell
git worktree add {{chemin/vers/répertoire}} -b {{nouvelle_branche}}
```
#### Répertorier tous les arbres de travail attachés à ce dépôt :
```shell
git worktree list
```
#### Supprimer les arbres de travail (après avoir supprimé les répertoires de travail) :
```shell
git worktree prune
```
{% endraw %}