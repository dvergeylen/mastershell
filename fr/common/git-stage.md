---
layout: default
title: "git stage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-stage">
  <a href="/fr/common/git-stage.html">git stage</a> <a href="#git-stage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ajouter le contenu du fichier à la zone de préparation.
> Synonyme de `git add`.
> Plus d'informations : <https://git-scm.com/docs/git-stage>.

#### Ajouter un fichier à l'index :
```shell
git stage {{chemin/vers/fichier}}
```
#### Ajoute tous les fichiers à l'index (suivis et non-suivis) :
```shell
git stage -A
```
#### Ajout uniquement des fichiers déjà suivis :
```shell
git stage -u
```
#### Ajout également des fichiers ignorés :
```shell
git stage -f
```
#### Ajout des fichiers par parties, interactivement :
```shell
git stage -p
```
#### Ajout d'un fichier par parties, interactivement :
```shell
git stage -p {{chemin/vers/fichier}}
```
#### Ajout d'un fichier, interactivement :
```shell
git stage -i
```
{% endraw %}