---
layout: default
title: "z"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="z">
  <a href="/fr/common/z.html">z</a> <a href="#z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Recherche les répertoires les plus utilisés et permet une navigation rapide à l'aide de chaînes de caractères ou d'expressions régulières.
> Plus d'informations : <https://github.com/rupa/z>.

#### Aller dans un répertoire qui contient "foo" dans son nom :
```shell
z {{foo}}
```
#### Aller dans un répertoire qui contient "foo" et "bar' dans son nom :
```shell
z {{foo}} {{bar}}
```
#### Aller dans le répertoire le mieux classé parmi ceux qui contiennent "foo" dans leurs noms :
```shell
z -r {{foo}}
```
#### Aller dans le répertoire accédé le plus récemment parmi ceux qui contiennent "foo" dans leurs noms :
```shell
z -t {{foo}}
```
#### Lis l'ensemble des répertoires dans la base de données `z` qui contiennent "foo" dans leurs noms :
```shell
z -l {{foo}}
```
#### Supprime le répertoire courant de la base de données de `z` :
```shell
z -x .
```
{% endraw %}