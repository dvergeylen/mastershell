---
layout: default
title: "git help"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-help">
  <a href="/fr/common/git-help.html">git help</a> <a href="#git-help"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Afficher le manuel de Git.
> Plus d'informations : <https://git-scm.com/docs/git-help>.

#### Afficher le manuel d'une sous-commande :
```shell
git help {{subcommand}}
```
#### Même chose dans un navigateur :
```shell
git help --web {{subcommand}}
```
#### Afficher la liste des sous-commandes disponibles :
```shell
git help --all
```
#### Lister les manuels disponibles :
```shell
git help --guide
```
#### Lister toutes les variables de configuration disponibles :
```shell
git help --config
```
{% endraw %}