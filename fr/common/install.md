---
layout: default
title: "install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="install">
  <a href="/fr/common/install.html">install</a> <a href="#install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copie des fichiers et met à jour leurs attributs.
> Copie des fichiers (souvent des exécutables) dans un répertoire système comme `/usr/local/bin` et leur donne les permissions et propriétaires appropriés.
> Plus d'informations : <https://www.gnu.org/software/coreutils/install>.

#### Copie des fichiers vers une destination :
```shell
install {{chemin/fichier/source}} {{chemin/repertoire/destination}}
```
#### Copie des fichiers vers une destination en mettant à jour leur propriétaire :
```shell
install -o {{utilisateur}} {{chemin/fichier/source}} {{chemin/repertoire/destination}}
```
#### Copie des fichiers vers une destination en mettant à jour leur groupe d'appartenance :
```shell
install -g {{utilisateur}} {{chemin/fichier/source}} {{chemin/repertoire/destination}}
```
#### Copie des fichiers vers une destination en mettant à jour leur mode :
```shell
install -m {{+x}} {{chemin/fichier/source}} {{chemin/repertoire/destination}}
```
#### Copie des fichiers en mettant à jour leur dates d'accès et de modification à partir de leurs sources respectives :
```shell
install -p {{chemin/fichier/source}} {{chemin/repertoire/destination}}
```
{% endraw %}