---
layout: default
title: "pacman"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman">
  <a href="/fr/linux/pacman.html">pacman</a> <a href="#pacman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil de gestion de paquets sur Arch Linux.
> Plus d'informations : <https://man.archlinux.org/man/pacman.8>.

#### Synchronise et mets à jour tous les paquets :
```shell
pacman -Syu
```
#### Installe un nouveau paquet :
```shell
pacman -S {{nom_paquet}}
```
#### Efface un paquet et ses dépendances :
```shell
pacman -Rs {{nom_paquet}}
```
#### Recherche dans la base de données des paquets une expression régulière ou mot clé :
```shell
pacman -Ss "{{terme_recherche}}"
```
#### Liste les paquets installés et leurs versions :
```shell
pacman -Q
```
#### Liste seulement les paquets installés explicitement et leurs versions :
```shell
pacman -Qe
```
#### Trouve à quel paquet un certain fichier appartient :
```shell
pacman -Qo {{fichier}}
```
#### Vide le cache des paquets pour libérer de l'espace :
```shell
pacman -Scc
```
{% endraw %}