---
layout: default
title: "xclip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xclip">
  <a href="/fr/linux/xclip.html">xclip</a> <a href="#xclip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil de manipulation de presse-papiers X11, semblable à `xsel`.
> Gère les sélections primaires et secondaires de X, en plus du presse-papier système (`Ctrl + C`/`Ctrl + V`).

#### Copie la sortie d'une commande vers la zone de sélection primaire de X11 (presse-papiers) :
```shell
echo 123 | xclip
```
#### Copie la sortie d'une commande vers une zone de sélection de X11 donnée :
```shell
echo 123 | xclip -selection {{primary|secondary|clipboard}}
```
#### Copie le contenu d'un fichier vers le presse-papiers système, avec la notation courte :
```shell
echo 123 | xclip -sel clip
```
#### Copie le contenu d'un fichier vers le presse-papiers système :
```shell
xclip -sel clip {{fichier_entrée.txt}}
```
#### Copie le contenu d'une image PNG vers le presse-papiers système (peut être collé dans d'autres programmes correctement) :
```shell
xclip -sel clip -t image/png {{fichier_entrée.png}}
```
#### Colle le contenu de la zone de sélection de X11 à la console :
```shell
xclip -o
```
#### Colle le contenu du presse-papier système à la console :
```shell
xclip -o -sel clip
```
#### Colle le contenu du presse-papier système à un fichier :
```shell
xclip -o -sel clip > {{fichier_sortie.txt}}
```
{% endraw %}