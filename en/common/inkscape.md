---
layout: default
title: "inkscape"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="inkscape">
  <a href="/en/common/inkscape.html">inkscape</a> <a href="#inkscape"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An SVG (Scalable Vector Graphics) editing program.
> For Inkscape versions up to 0.92.x, use -e instead of -o.
> More information: <https://inkscape.org>.

#### Open an SVG file in the Inkscape GUI:
```shell
inkscape {{filename.svg}}
```
#### Export an SVG file into a bitmap with the default format (PNG) and the default resolution (96 DPI):
```shell
inkscape {{filename.svg}} -o {{filename.png}}
```
#### Export an SVG file into a bitmap of 600x400 pixels (aspect ratio distortion may occur):
```shell
inkscape {{filename.svg}} -o {{filename.png}} -w {{600}} -h {{400}}
```
#### Export the drawing (bounding box of all objects) of an SVG file into a bitmap:
```shell
inkscape {{filename.svg}} -o {{filename.png}} -D
```
#### Export a single object, given its ID, into a bitmap:
```shell
inkscape {{filename.svg}} -i {{id}} -o {{object.png}}
```
#### Export an SVG document to PDF, converting all texts to paths:
```shell
inkscape {{filename.svg}} -o {{filename.pdf}} --export-text-to-path
```
#### Duplicate the object with id="path123", rotate the duplicate 90 degrees, save the file, and quit Inkscape:
```shell
inkscape {{filename.svg}} --select=path123 --verb="{{EditDuplicate;ObjectRotate90;FileSave;FileQuit}}"
```
{% endraw %}