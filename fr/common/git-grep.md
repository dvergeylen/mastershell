---
layout: default
title: "git-grep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-grep">
  <a href="/fr/common/git-grep.html">git-grep</a> <a href="#git-grep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rechercher une occurrence de texte n'importe où dans l'historique d'un dépôt git.
> Comprend la plupart des arguments du `grep` classique.
> Plus d'informations : <https://git-scm.com/docs/git-grep>.

#### Rechercher une occurrence dans les fichiers suivis :
```shell
git grep {{chaine_recherché}}
```
#### Rechercher une occurrence dans les fichiers suivis d'après un pattern de fichiers :
```shell
git grep {{chaine_recherché}} -- {{file_glob_pattern}}
```
#### Rechercher une occurrence dans les fichiers suivis et les sous-modules :
```shell
git grep --recurse-submodules {{chaine_recherché}}
```
#### Rechercher une occurrence à partir d'un point spécifique dans l'historique :
```shell
git grep {{chaine_recherché}} {{HEAD~2}}
```
#### Rechercher une occurrence dans toutes les branches :
```shell
git grep {{chaine_recherché}} $(git rev-list --all)
```
{% endraw %}