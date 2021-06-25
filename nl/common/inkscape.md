---
layout: default
title: "inkscape"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="inkscape">
  <a href="/nl/common/inkscape.html">inkscape</a> <a href="#inkscape"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Een SVG (Scalable Vector Graphics) bewerkingsprogramma.
> Voor Inkscape versies tot en met 0.92.x, gebruik -e in plaats van -o.
> Meer informatie: <https://inkscape.org>.

#### Open een SVG-bestand in de Inkscape GUI:
```shell
inkscape {{bestandsnaam.svg}}
```
#### Exporteer een SVG-bestand in een bitmap met het standaardformaat (PNG) en de standaardresolutie (96 DPI):
```shell
inkscape {{bestandsnaam.svg}} -o {{bestandsnaam.png}}
```
#### Exporteer een SVG-bestand in een bitmap van 600x400 pixels (vervorming van de aspectverhouding mogelijk):
```shell
inkscape {{bestandsnaam.svg}} -o {{bestandsnaam.png}} -w {{600}} -h {{400}}
```
#### Exporteer de tekening (selectiekader van alle objecten) van een SVG-bestand in een bitmap:
```shell
inkscape {{bestandsnaam.svg}} -o {{bestandsnaam.png}} -D
```
#### Exporteer een enkel object, gezien zijn ID, in een bitmap:
```shell
inkscape {{bestandsnaam.svg}} -i {{id}} -o {{object.png}}
```
#### Exporteer een SVG-document naar PDF, converteer alle teksten naar paden:
```shell
inkscape {{bestandsnaam.svg}} -o {{bestandsnaam.pdf}} --export-text-to-path
```
#### Dupliceer het object met id="pad123", roteer het duplicaat 90 graden, sla het bestand op, en sluit Inkscape af:
```shell
inkscape {{bestandsnaam.svg}} --select=path123 --verb="{{EditDuplicate;ObjectRotate90;FileSave;FileQuit}}"
```
{% endraw %}