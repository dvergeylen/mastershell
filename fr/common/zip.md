---
layout: default
title: "zip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zip">
  <a href="/fr/common/zip.html">zip</a> <a href="#zip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Empaquette et compresse (archive) les fichiers en un fichier zip.

#### Empaquette et compresse [r]écursivement un répertoire et son contenu :
```shell
zip -r {{archive.zip}} {{chemin/du/répertoire}}
```
#### E[x]clure des fichiers de l'archive :
```shell
zip -r {{archive.zip}} {{chemin/vers/le/répertoire}} -x {{chemin/des/fichiers/exclus}}
```
#### Archive un répertoire et son contenu avec le plus haut niveau [9] de compression :
```shell
zip -r -{{9}} {{archive.zip}} {{chemin/du/répertoire}}
```
#### Empaquette et compresse plusieurs répertoires et fichiers :
```shell
zip -r {{archive.zip}} {{chemin/du/répertoire1 chemin/du/répertoire2 chemin/du/fichier}}
```
#### Crée une archive chiffrée (l'utilisateur sera sollicité pour saisir le mot de passe) :
```shell
zip -e -r {{archive.zip}} {{chemin/du/répertoire}}
```
#### Ajoute des fichiers à une archive existante :
```shell
zip {{archive.zip}} {{chemin/du/fichier}}
```
#### Supprime des fichiers d'une archive existante :
```shell
zip -d {{archive.zip}} "{{foo/*.tmp}}"
```
#### Archive un répertoire et son contenu en plusieurs fichiers zip [s]cindés (ex : des fichiers de 3 Go) :
```shell
zip -r -s {{3g}} {{archive.zip}} {{chemin/du/répertoire}}
```
{% endraw %}