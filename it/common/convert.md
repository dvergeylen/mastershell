---
layout: default
title: "convert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="convert">
  <a href="/it/common/convert.html">convert</a> <a href="#convert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento della suite immagineMagick per la conversione di immagini.
> Maggiori informazioni: <https://imagemagick.org/script/convert.php>.

#### Converti un'immagine da JPG a PNG:
```shell
convert {{immagine.jpg}} {{immagine.png}}
```
#### Scala un'immagine al 50% delle sue dimensioni originali:
```shell
convert {{immagine.png}} -resize 50% {{immagine2.png}}
```
#### Scala un'immagine ad una dimensione massima di 640x480 mantenendo le proporzioni originali:
```shell
convert {{immagine.png}} -resize 640x480 {{immagine2.png}}
```
#### Concatena più immagini orizzontalmente:
```shell
convert {{immagine1.png}} {{immagine2.png}} {{immagine3.png}} +append {{immagine123.png}}
```
#### Crea una GIF da una serie di immagini con un intervallo di 100ms tra ogni immagine:
```shell
convert {{immagine1.png}} {{immagine2.png}} {{immagine3.png}} -delay {{100}} {{animazione.gif}}
```
#### Crea un'immagine a tinta unita di un determinato colore:
```shell
convert -size {{800x600}} "xc:{{#ff0000}}" {{immagine.png}}
```
{% endraw %}