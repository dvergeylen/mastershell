---
layout: default
title: "apt-file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-file">
  <a href="/fr/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Recherche de fichiers dans les paquets apt, y compris ceux qui ne sont pas encore installés.
> Plus d'informations : <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### Mise à jour la base de données des métadonnées :
```shell
sudo apt update
```
#### Recherche des paquets qui contiennent le fichier ou le chemin d'accès spécifié :
```shell
apt-file search {{part/of/filename}}
```
#### Énumère le contenu d'un paquet spécifique :
```shell
apt-file list {{package_name}}
```
{% endraw %}