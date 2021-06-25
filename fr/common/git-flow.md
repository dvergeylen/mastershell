---
layout: default
title: "git flow"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-flow">
  <a href="/fr/common/git-flow.html">git flow</a> <a href="#git-flow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Une collection d'extensions Git pour procurer des opérations supplémentaires sur les dépôts.
> Plus d'informations : <https://github.com/nvie/gitflow>.

#### Initialiser dans un registre Git existant :
```shell
git flow init
```
#### Commencer le travail sur une fonctionnalité basé sur la branche `develop` :
```shell
git flow feature start {{feature}}
```
#### Terminer le travail sur une branche de fonctionnalité, la fusionner dans la branche `develop` puis la supprimer :
```shell
git flow feature finish {{feature}}
```
#### Publier une fonctionnalité sur le serveur distant :
```shell
git flow feature publish {{feature}}
```
#### Récupérer une fonctionnalité publiée par un autre utilisateur :
```shell
git flow feature pull origin {{feature}}
```
{% endraw %}