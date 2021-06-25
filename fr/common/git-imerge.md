---
layout: default
title: "git-imerge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-imerge">
  <a href="/fr/common/git-imerge.html">git-imerge</a> <a href="#git-imerge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Générer un `git merge` ou un `git rebase` entre deux branches de manière incrémentale.
> Les conflits entre les branches sont suivis en paires de commits individuels, pour simplifier la résolution des conflits.
> Plus d'informations : <https://github.com/mhagger/git-imerge>.

#### Démarrer un imerge rebase (se placer dans la branche à rebaser d'abord) :
```shell
git imerge rebase {{branche_sur_laquelle_rebaser}}
```
#### Démarrer imerge merge (se placer dans la branche depuis laquelle merger d'abord) :
```shell
git imerge merge {{branche_a_merger}}
```
#### Afficher le diagramme ASCII du merge ou rebase en cours :
```shell
git imerge diagram
```
#### Continuer l'opération après une résolution de conflit (d'abord `git add` les fichiers en conflits) :
```shell
git imerge continue --no-edit
```
#### Terminer l'opération i-merge après la résolution de tous les conflits :
```shell
git imerge finish
```
#### Annuler l'opération et retourner à la branche précédente :
```shell
git-imerge remove && git checkout {{previous_branch}}
```
{% endraw %}