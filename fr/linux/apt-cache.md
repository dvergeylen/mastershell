---
layout: default
title: "apt-cache"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-cache">
  <a href="/fr/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil de recherche de paquets Debian et Ubuntu.
> Plus d'informations : <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### Recherche un paquet dans vos sources actuelles :
```shell
apt-cache search {{query}}
```
#### Affiche des informations sur un paquet :
```shell
apt-cache show {{package}}
```
#### Indique si un paquet est installé et à jour :
```shell
apt-cache policy {{package}}
```
#### Affiche les dépendances d'un paquet :
```shell
apt-cache depends {{package}}
```
#### Affiche les paquets qui dépendent d'un paquet particulier :
```shell
apt-cache rdepends {{package}}
```
{% endraw %}