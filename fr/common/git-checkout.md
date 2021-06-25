---
layout: default
title: "git checkout"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-checkout">
  <a href="/fr/common/git-checkout.html">git checkout</a> <a href="#git-checkout"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extraire une branche ou des chemins vers l'arborescence de travail.
> Plus d'informations : <https://git-scm.com/docs/git-checkout>.

#### Créer une branche et basculer dessus :
```shell
git checkout -b {{nom_de_branche}}
```
#### Créer une branche depuis une référence spécifique et basculer dessus (par exemple, branche locale/distante, tag, commit) :
```shell
git checkout -b {{nom_de_branche}} {{référence}}
```
#### Basculer sur une branche locale existante :
```shell
git checkout {{nom_de_branche}}
```
#### Basculer sur la branche précédente :
```shell
git checkout -
```
#### Basculer sur une branche distante existante :
```shell
git checkout --track {{nom_distant}}/{{nom_de_branche}}
```
#### Annule tout les changements dans le répertoire courant (voir `git reset` pour plus de commandes d'annulation) :
```shell
git checkout .
```
#### Annule tout les changements dans le fichier spécifié :
```shell
git checkout {{filename}}
```
#### Remplace un fichier par sa version d'une autre branche :
```shell
git checkout {{nom_de_branche}} -- {{filename}}
```
{% endraw %}