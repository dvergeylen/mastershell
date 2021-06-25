---
layout: default
title: "xbacklight"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xbacklight">
  <a href="/fr/linux/xbacklight.html">xbacklight</a> <a href="#xbacklight"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil pour ajuster la luminosité du rétroéclairage en utilisant l'extension RandR.
> Plus d'informations : <https://gitlab.freedesktop.org/xorg/app/xbacklight>.

#### Obtient le niveau de luminosité de l'écran actuel comme un pourcentage :
```shell
xbacklight
```
#### Régle la luminosité de l'écran à 40% :
```shell
xbacklight -set {{40}}
```
#### Augmente la luminosité de l'écran actuel de 25% :
```shell
xbacklight -inc {{25}}
```
#### Diminue la luminosité de l'écran actuel de 75% :
```shell
xbacklight -dec {{75}}
```
#### Augment la luminosité de l'écran à 100%, étendu sur 60 secondes (valeur donnée en ms), en 60 pas :
```shell
xbacklight -set {{100}} -time {{60000}} -steps {{60}}
```
{% endraw %}