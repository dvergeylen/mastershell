---
layout: default
title: "zoxide"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zoxide">
  <a href="/fr/common/zoxide.html">zoxide</a> <a href="#zoxide"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Garde une trace des répertoires les plus utilisés.
> Utilise un algorithme de classement pour identifier le meilleur résultat.
> Plus d'informations : <https://github.com/ajeetdsouza/zoxide>.

#### Aller au répertoire avec le meilleur classement qui contient "foo" dans son nom :
```shell
zoxide query {{foo}}
```
#### Aller au répertoire avec le meilleur classement qui contient "foo" et "bar" dans son nom :
```shell
zoxide query {{foo}} {{bar}}
```
#### Démarre une recherche de répertoire interactive (nécessite `fzf`) :
```shell
zoxide query --interactive
```
#### Ajoute un répertoire ou incrémente son classement :
```shell
zoxide add {{chemin/du/répertoire}}
```
#### Supprime un répertoire de la base de données de `zoxide` :
```shell
zoxide remove {{chemin/du/répertoire}}
```
#### Génère la configuration du shell pour la mise en place des alias de commandes (`z`, `za`, `zi`, `zq`, `zr`) :
```shell
zoxide init {{bash|fish|zsh}}
```
{% endraw %}