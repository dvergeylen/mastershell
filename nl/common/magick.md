---
layout: default
title: "magick"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="magick">
  <a href="/nl/common/magick.html">magick</a> <a href="#magick"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creër, bewerk, vorm, of converteer bitmapafbeeldingen.
> ImageMagick versie 7+. Bekijk `convert` versies 6 en lager.
> Meer informatie: <https://imagemagick.org/>.

#### Converteer bestandstype:
```shell
magick {{afbeelding.png}} {{afbeelding.jpg}}
```
#### Formaat van een afbeelding wijzigen, maak een nieuw kopie:
```shell
magick convert -resize {{100x100}} {{afbeelding.jpg}} {{afbeelding.jpg}}
```
#### Creër een GIF door middel van afbeeldingen:
```shell
magick {{*.jpg}} {{afbeelding.gif}}
```
#### Creër een dambordpatroon:
```shell
magick -size {{640x480}} pattern:checkerboard {{dambordpatroon.png}}
```
#### Converteer afbeeldingen naar individuele PDF-pagina's:
```shell
magick {{*.jpg}} +adjoin {{pagina-%d.pdf}}
```
{% endraw %}