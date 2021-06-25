---
layout: default
title: "convert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="convert">
  <a href="/fr/common/convert.html">convert</a> <a href="#convert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil de conversion d'image d'ImageMagick.
> Plus d'informations : <https://imagemagick.org/script/convert.php>.

#### Convertir une image JPG en PNG :
```shell
convert {{image.jpg}} {{image.png}}
```
#### Redimensionner une image à 50% de ses dimensions d'origine :
```shell
convert {{image.png}} -resize 50% {{image2.png}}
```
#### Redimensionner une image en conservant son ratio hauteur/largeur initial pour une taille maximum de 640x480 :
```shell
convert {{image.png}} -resize 640x480 {{image2.png}}
```
#### Coller plusieurs images horizontallement :
```shell
convert {{image1.png}} {{image2.png}} {{image3.png}} +append {{image123.png}}
```
#### Coller plusieurs images verticalement :
```shell
convert {{image1.png}} {{image2.png}} {{image3.png}} -append {{image123.png}}
```
#### Créer un gif à partir d'une série d'images avec un délai de 100ms entre chaque :
```shell
convert {{image1.png}} {{image2.png}} {{image3.png}} -delay {{100}} {{animation.gif}}
```
#### Créer une image avec un simple arrière-plan uni :
```shell
convert -size {{800x600}} "xc:{{#ff0000}}" {{image.png}}
```
{% endraw %}