---
layout: default
title: "git tag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-tag">
  <a href="/fr/common/git-tag.html">git tag</a> <a href="#git-tag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Créer, lister, vérifier et supprimer des tags.
> Un tag est une référence statique vers un commit.
> Plus d'informations : <https://git-scm.com/docs/git-tag>.

#### Lister tout les tags :
```shell
git tag
```
#### Créer un tag avec le nom donné pointant vers le commit actuel :
```shell
git tag {{nom_d_etiquette}}
```
#### Créer un tag avec le nom donné pointant vers un commit spécifié :
```shell
git tag {{nom_d_etiquette}} {{commit}}
```
#### Créer un tag annoté avec le message spécifié :
```shell
git tag {{nom_d_etiquette}} -m {{message_d_etiquette}}
```
#### Supprimer le tag avec le nom spécifié :
```shell
git tag -d {{nom_d_etiquette}}
```
#### Mettre à jour les tags depuis l'origine :
```shell
git fetch --tags
```
#### Liste toutes les tags dont les ancêtres incluent un commit donné :
```shell
git tag --contains {{commit}}
```
{% endraw %}