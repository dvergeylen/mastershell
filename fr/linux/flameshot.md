---
layout: default
title: "flameshot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="flameshot">
  <a href="/fr/linux/flameshot.html">flameshot</a> <a href="#flameshot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil de capture d'écran avec une interface graphique.
> Ajoute du texte, des formes, des couleurs et envoie à imgur.
> Plus d'informations : <https://flameshot.js.org>.

#### Lancez Flameshot en mode graphique :
```shell
flameshot launcher
```
#### Prenez une capture d'écran en cliquant et en faisant glisser :
```shell
flameshot gui
```
#### Prenez une capture d'écran en plein écran :
```shell
flameshot full
```
#### Définissez le chemin de sauvegarde :
```shell
flameshot full --path {{path/to/directory}}
```
#### Retardez la capture d'écran de N millisecondes et la sortie dans le presse-papiers :
```shell
flameshot full --delay {{2000}} --clipboard
```
{% endraw %}