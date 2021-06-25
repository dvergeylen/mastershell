---
layout: default
title: "git switch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-switch">
  <a href="/fr/common/git-switch.html">git switch</a> <a href="#git-switch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Basculez entre les branches Git. Nécessite la version 2.23+ de Git.
> Voir également `git checkout`.
> Plus d'informations : <https://git-scm.com/docs/git-switch>.

#### Baculer sur une branche existante :
```shell
git switch {{nom_de_branche}}
```
#### Créer une nouvelle branche et basculer dessus :
```shell
git switch --create {{nom_de_branche}}
```
#### Créer une nouvelle branche en partant d'un commit donné et basculer dessus :
```shell
git switch --create {{nom_de_branche}} {{commit}}
```
#### Basculer sur la branche précédente :
```shell
git switch -
```
#### Basculer vers une branche et mettre à jour tous les sous-modules pour qu'ils correspondent :
```shell
git switch --recurse-submodules {{nom_de_branche}}
```
#### Basculer vers une branche et fusionner automatiquement la branche actuelle et toutes les modifications non validées dedans :
```shell
git switch --merge {{nom_de_branche}}
```
{% endraw %}