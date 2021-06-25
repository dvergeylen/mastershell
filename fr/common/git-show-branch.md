---
layout: default
title: "git show-branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-show-branch">
  <a href="/fr/common/git-show-branch.html">git show-branch</a> <a href="#git-show-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Affiche les branches et leurs commits.
> Plus d'informations : <https://git-scm.com/docs/git-show-branch>.

#### Affiche un résumé du dernier commit dans la branche :
```shell
git show-branch {{nom_de_branche}}|ref|commit}}
```
#### Comparer des commits avec plusieurs commits ou branches :
```shell
git show-branch {{nom_de_branche}}|ref|commit}}
```
#### Comparer toutes les branches distantes :
```shell
git show-branch --remotes
```
#### Comparer la branche locale avec la branche distante :
```shell
git show-branch --all
```
#### Lister les derniers commits sur toutes les branches :
```shell
git show-branch --all --list
```
#### Comparer une branche spécifique à la branche courante :
```shell
git show-branch --current {{commit|branch_name|ref}}
```
#### Afficher le nom du commit au lieu du nom relatif :
```shell
git show-branch --sha1-name --current {{current|branch_name|ref}}
```
#### Continuez l'affichage d'un certain nombre de commits au-delà de l'ancêtre commun :
```shell
git show-branch --more {{5}} {{commit|branch_name|ref}} {{commit|branch_name|ref}} {{...}}
```
{% endraw %}