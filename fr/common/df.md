---
layout: default
title: "df"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="df">
  <a href="/fr/common/df.html">df</a> <a href="#df"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Montre un aperçu de l'utilisation de l'espace disque.
> Plus d'informations : <https://www.gnu.org/software/coreutils/df>.

#### Afficher tous les systèmes de fichiers et leur utilisation d'espace disque :
```shell
df
```
#### Afficher tous les systèmes de fichiers et leur utilisation d'espace disque dans un format plus facilement :
```shell
df -h
```
#### Afficher le système de fichiers et son utilisation d'espace disque rattaché au chemin donné :
```shell
df {{chemin/vers/fichier_ou_dossier}}
```
#### Afficher des statistiques sur le nombre d'inodes disponibles :
```shell
df -i
```
#### Afficher les systèmes de fichiers sauf ceux de types spécifiques :
```shell
df -x {{squashfs}} -x {{tmpfs}}
```
{% endraw %}