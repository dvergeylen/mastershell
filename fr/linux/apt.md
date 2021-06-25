---
layout: default
title: "apt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt">
  <a href="/fr/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitaire de gestion des paquets pour les distributions basées sur Debian.
> Remplacement recommandé pour apt-get lorsqu'il est utilisé de manière interactive dans les versions 16.04 et ultérieures d'Ubuntu.
> Plus d'informations : <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Mettre à jour la liste des paquets et des versions disponibles (il est recommandé de l'exécuter avant les autres commandes `apt`) :
```shell
sudo apt update
```
#### Recherche d'un paquet donné :
```shell
apt search {{package}}
```
#### Afficher les informations pour un paquet :
```shell
apt show {{package}}
```
#### Installer un paquet, ou le mettre à jour avec la dernière version disponible :
```shell
sudo apt install {{package}}
```
#### Supprimer un paquet (utiliser `purge` à la place supprime également ses fichiers de configuration) :
```shell
sudo apt remove {{package}}
```
#### Mettre à jour tous les paquets installés vers les dernières versions disponibles :
```shell
sudo apt upgrade
```
#### Lister tous les paquets :
```shell
apt list
```
#### Lister les paquets installés :
```shell
apt list --installed
```
{% endraw %}