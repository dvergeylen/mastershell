---
layout: default
title: "git diff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-diff">
  <a href="/fr/common/git-diff.html">git diff</a> <a href="#git-diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Afficher les changements sur les fichiers suivis.
> Plus d'informations : <https://git-scm.com/docs/git-diff>.

#### Afficher les changements sur les fichiers suivis :
```shell
git diff
```
#### Afficher tous les changements sur les fichiers par rapport à la tête de branche :
```shell
git diff HEAD
```
#### Afficher tous les changements sur les fichiers ajoutés mais pas encore commités :
```shell
git diff --staged
```
#### Afficher les changements de tous les commits à partir d'une date / heure donnée (expression de dates, ex : "1 week 2 days" pour 1 semaine et 2 jours ou une date ISO) :
```shell
git diff 'HEAD@{3 months|weeks|days|hours|seconds ago}'
```
#### Afficher seulement les noms des fichiers modifiés depuis un commit donné :
```shell
git diff --name-only {{commit}}
```
#### Afficher un résumé des créations de fichiers, renommages ou changements de droits depuis un commit :
```shell
git diff --summary {{commit}}
```
#### Comparer un fichier entre deux branches ou commits :
```shell
git diff {{branche_1}}..{{branche_2}} [--] {{chemin/vers/fichier}}
```
#### Comparer plusieurs fichiers de la branche courante avec une autre branche :
```shell
git diff {{branche}}:{{chemin/vers/fichier2}} {{chemin/vers/fichier}}
```
{% endraw %}