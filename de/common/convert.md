---
layout: default
title: "convert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="convert">
  <a href="/de/common/convert.html">convert</a> <a href="#convert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ImageMagick Bildkonvertierungswerkzeug.
> Weitere Informationen: <https://imagemagick.org/script/convert.php>.

#### Konvertiere ein Bild von JPG nach PNG:
```shell
convert {{pfad/zu/bild.jpg}} {{pfad/zu/bild.png}}
```
#### Skaliere ein Bild auf 50% seiner Originalgröße:
```shell
convert {{pfad/zu/bild.png}} -resize 50% {{pfad/zu/bild2.png}}
```
#### Skaliere ein Bild unter Beibehaltung des ursprünglichen Seitenverhältnisses auf eine maximale Größe von 640x480:
```shell
convert {{pfad/zu/bild.png}} -resize 640x480 {{pfad/zu/bild2.png}}
```
#### Hänge Bilder horizontal aneinader:
```shell
convert {{pfad/zu/bild1.png}} {{pfad/zu/bild2.png}} {{pfad/zu/bild3.png}} +append {{pfad/zu/bild123.png}}
```
#### Hänge Bilder vertikal aneinander:
```shell
convert {{pfad/zu/bild1.png}} {{pfad/zu/bild2.png}} {{pfad/zu/bild3.png}} -append {{pfad/zu/bild123.png}}
```
#### Erstelle ein animiertes GIF aus einer Serie von Bildern mit einer Verzögerung von 100 ms zwischen den Bildern:
```shell
convert {{pfad/zu/bild1.png}} {{pfad/zu/bild2.png}} {{pfad/zu/bild3.png}} -delay {{10}} {{pfad/zu/animation.gif}}
```
#### Erstelle ein Bild mit nichts als einem festen Hintergrund:
```shell
convert -size {{800x600}} "xc:{{#ff0000}}" {{pfad/zu/bild.png}}
```
{% endraw %}