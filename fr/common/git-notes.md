---
layout: default
title: "git notes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-notes">
  <a href="/fr/common/git-notes.html">git notes</a> <a href="#git-notes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ajoute ou inspecte des notes d'objets.
> Plus d'informations : <https://git-scm.com/docs/git-notes>.

#### Lister toutes les notes et leurs objets rattachés :
```shell
git notes list
```
#### Lister toutes les notes attachées à un objet donné :
```shell
git notes list [{{objet}}]
```
#### Afficher les notes attachées à un objet donné :
```shell
git notes show [{{objet}}]
```
#### Ajoute une note à un objet donné :
```shell
git notes append {{objet}}
```
#### Ajoute une note à un objet donné, en spécifiant le message :
```shell
git notes append --message="{{texte_du_message}}"
```
#### Édite une note existante :
```shell
git notes edit [{{objet}}]
```
#### Copie la note d'un objet vers un autre :
```shell
git notes copy {{objet_source}} {{objet_cible}}
```
#### Supprime toutes les notes d'un objet donné :
```shell
git notes remove {{objet}}
```
{% endraw %}