---
layout: default
title: "yay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yay">
  <a href="/fr/linux/yay.html">yay</a> <a href="#yay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Yet Another Yogurt : Un outil pour Arch Linux pour construire et installer des paquets depuis le Arch User Repository.
> À regarder : `pacman`.
> Plus d'informations : <https://github.com/Jguer/yay>.

#### Recherche interactivement et installe des paquets depuis les dépôts et l'AUR :
```shell
yay {{nom_paquet|terme_recherche}}
```
#### Synchronise et met à jour tous les paquets depuis les dépôts et l'AUR :
```shell
yay
```
#### Synchronise et met à jour seulement les paquets de l'AUR :
```shell
yay -Sua
```
#### Installe un nouveau paquet depuis les dépôts et l'AUR :
```shell
yay -S {{nom_paquet}}
```
#### Recherche dans la base de données de paquets un mot clé depuis les dépôts et l'AUR :
```shell
yay -Ss {{mot_clé}}
```
#### Montre des statistiques sur les paquets installés et la santé du système :
```shell
yay -Ps
```
{% endraw %}