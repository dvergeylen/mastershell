---
layout: default
title: "tar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tar">
  <a href="/fr/common/tar.html">tar</a> <a href="#tar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitaire d'archivage.
> Souvent combiné avec une méthode de compression, telle que gzip ou bzip2.
> Plus d'informations : <https://www.gnu.org/software/tar>.

#### Créer une archive à partir de fichiers :
```shell
tar cf {{cible.tar}} {{fichier1 fichier2 fichier3}}
```
#### Créer une archive gzip :
```shell
tar czf {{cible.tar.gz}} {{fichier1 fichier2 fichier3}}
```
#### Extraie une archive (compressée) dans le dossier courant :
```shell
tar xf {{source.tar[.gz|.bz2|.xz]}}
```
#### Extraie une archive dans un dossier cible :
```shell
tar xf {{source.tar}} -C {{dossier}}
```
#### Créer une archive compressée, en utilisant le suffixe de l'archive pour déterminer le programme de compression :
```shell
tar caf {{cible.tar.xz}} {{fichier1 fichier2 fichier3}}
```
#### Lister le contenu d'une archive tar :
```shell
tar tvf {{source.tar}}
```
#### Extraire les fichiers correspondant au motif :
```shell
tar xf {{source.tar}} --wildcards "{{*.html}}"
```
{% endraw %}