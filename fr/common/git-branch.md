---
layout: default
title: "git branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-branch">
  <a href="/fr/common/git-branch.html">git branch</a> <a href="#git-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Commande Git principale pour travailler avec des branches.
> Plus d'informations : <https://git-scm.com/docs/git-branch>.

#### Liste les branches locale en préfixant la branche courante avec `*` :
```shell
git branch
```
#### Liste toutes les branches (locale et distantes) :
```shell
git branch -a
```
#### Affiche le nom de la branche courante :
```shell
git branch --show-current
```
#### Crée une nouvelle branche depuis le commit courant :
```shell
git branch {{nom_de_branche}}
```
#### Crée une nouvelle branche depuis un commit en particulier :
```shell
git branch {{nom_de_branche}} {{commit_hash}}
```
#### Renommer une branche (ne pas se trouver sur la branche pour le faire) :
```shell
git branch -m {{ancien_nom_de_branche}} {{nouveau_nom_de_branche}}
```
#### Supprimer un branche locale (ne pas se trouver sur la branche pour le faire) :
```shell
git branch -d {{nom_de_branche}}
```
#### Supprimer une branche distante :
```shell
git push {{nom_distant}} --delete {{nom_de_branche_distante}}
```
{% endraw %}