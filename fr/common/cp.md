---
layout: default
title: "cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cp">
  <a href="/fr/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copie des fichiers et des répertoires.
> Plus d'informations : <https://www.gnu.org/software/coreutils/cp>.

#### Copier un fichier vers un autre emplacement :
```shell
cp {{chemin/vers/fichier_source.ext}} {{chemin/vers/fichier_cible.ext}}
```
#### Copier un fichier vers un autre répertoire en conservant le nom du fichier :
```shell
cp {{chemin/vers/fichier_source.ext}} {{chemin/vers/répertoire_parent_cible}}
```
#### Copier récursivement le contenu d'un répertoire vers un autre emplacement (si la destination existe, le répertoire est copié à l'intérieur) :
```shell
cp -R {{chemin/vers/répertoire_source}} {{chemin/vers/répertoire_cible}}
```
#### Copier un répertoire récursivement, en mode verbeux (affiche les fichiers au fur et à mesure de leur copie) :
```shell
cp -vR {{chemin/vers/répertoire_source}} {{chemin/vers/répertoire_cible}}
```
#### Copier les fichiers texte vers un autre emplacement, en mode interactif (demande confirmation avant d'écraser) :
```shell
cp -i {{*.txt}} {{chemin/vers/répertoire_cible}}
```
#### Déréférencer les liens symboliques avant de copier :
```shell
cp -L {{link}} {{chemin/vers/répertoire_cible}}
```
{% endraw %}