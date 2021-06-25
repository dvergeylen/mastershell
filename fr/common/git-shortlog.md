---
layout: default
title: "git shortlog"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-shortlog">
  <a href="/fr/common/git-shortlog.html">git shortlog</a> <a href="#git-shortlog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Récapitule la sortie de `git log`.
> Plus d'informations : <https://git-scm.com/docs/git-shortlog>.

#### Afficher un résumé de tous les commits effectués, regroupés par ordre alphabétique par nom d'auteur :
```shell
git shortlog
```
#### Afficher un résumé de tous les commits effectués, regroupés par le nombre de commits effectués :
```shell
git shortlog -n
```
#### Afficher un résumé de tous les commits effectués, regroupés par le nom et l'email de l'utilisateur :
```shell
git shortlog -c
```
#### fficher un résumé des 5 derniers commits effectués :
```shell
git shortlog HEAD~{{5}}..HEAD
```
#### Afficher tout les utilisateurs, emails et le nombre de commits dans la branche :
```shell
git shortlog -sne
```
#### Afficher tout les utilisateurs, emails et le nombre de commits dans toutes les branches :
```shell
git shortlog -sne --all
```
{% endraw %}