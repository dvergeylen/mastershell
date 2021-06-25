---
layout: default
title: "apt-get"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-get">
  <a href="/fr/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitaire de gestion des paquets Debian et Ubuntu.
> Recherche des paquets en utilisant `apt-cache`.
> Plus d'informations : <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Mise à jour de la liste des paquets et des versions disponibles (il est recommandé de l'exécuter avant les autres commandes `apt-get`) :
```shell
apt-get update
```
#### Installation d'un paquet, ou mise à jour avec la dernière version disponible :
```shell
apt-get install {{package}}
```
#### Suppression d'un paquet :
```shell
apt-get remove {{package}}
```
#### Suppression d'un paquet et de ses fichiers de configuration :
```shell
apt-get purge {{package}}
```
#### Mise à jour de tous les paquets installés vers les dernières versions disponibles :
```shell
apt-get upgrade
```
#### Nettoyage du dépôt local - supprime les fichiers de paquets (`.deb`) des téléchargements interrompus qui ne peuvent plus être téléchargés:
```shell
apt-get autoclean
```
#### Suppression de tous les paquets qui ne sont plus nécessaires :
```shell
apt-get autoremove
```
#### Mise à jour des paquets installés (comme la commande `upgrade`), mais avec suppression des paquets obsolètes et installation des paquets supplémentaires pour répondre aux nouvelles dépendances :
```shell
apt-get dist-upgrade
```
{% endraw %}