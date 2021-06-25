---
layout: default
title: "apt-mark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-mark">
  <a href="/fr/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitaire permettant de modifier l'état des paquets installés.
> Plus d'informations : <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### Marquer un paquet comme étant automatiquement installé :
```shell
sudo apt-mark auto {{package_name}}
```
#### Maintenir un paquet à sa version actuelle et empêcher les mises à jour :
```shell
sudo apt-mark hold {{package_name}}
```
#### Permettre une nouvelle mise à jour d'un paquet :
```shell
sudo apt-mark unhold {{package_name}}
```
#### Afficher les paquets installés manuellement :
```shell
apt-mark showmanual
```
#### Afficher les paquets détenus qui ne sont pas mis à jour :
```shell
apt-mark showhold
```
{% endraw %}