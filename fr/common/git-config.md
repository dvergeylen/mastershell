---
layout: default
title: "git config"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-config">
  <a href="/fr/common/git-config.html">git config</a> <a href="#git-config"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gérer les options de configuration personnalisées pour les référentiels Git.
> Ces configurations peuvent être locales (pour le référentiel courant) ou globales (pour l'utilisateur).
> Plus d'informations : <https://git-scm.com/docs/git-config>.

#### Liste les entrées de configurations locales (stockées dans `.git/config` du répertoire courant) :
```shell
git config --list --local
```
#### Liste les entrées de configuration globales (stockées dans `~/.gitconfig`) :
```shell
git config --list --global
```
#### Liste toutes les entrées de configuration, globales et locales :
```shell
git config --list
```
#### Récupère la valeur d'une entrée de configuration :
```shell
git config alias.unstage
```
#### Attribue la valeur d'une entrée de configuration :
```shell
git config --global alias.unstage "reset HEAD --"
```
#### Restaure la valeur d'une entrée de configuration globale à sa valeur par défaut :
```shell
git config --global --unset alias.unstage
```
#### Édite le fichier de configuration du référentiel courant dans l'éditeur par défaut :
```shell
git config --edit
```
#### Édite le fichier de configuration globale dans l'éditeur par défaut :
```shell
git config --global --edit
```
{% endraw %}