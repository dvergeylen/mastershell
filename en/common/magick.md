---
layout: default
title: "magick"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="magick">
  <a href="/en/common/magick.html">magick</a> <a href="#magick"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create, edit, compose, or convert bitmap images.
> ImageMagick version 7+. See `convert` for versions 6 and below.
> More information: <https://imagemagick.org/>.

#### Convert file type:
```shell
magick {{image.png}} {{image.jpg}}
```
#### Resize an image, making a new copy:
```shell
magick convert -resize {{100x100}} {{image.jpg}} {{image.jpg}}
```
#### Create a GIF using images:
```shell
magick {{*.jpg}} {{images.gif}}
```
#### Create checkerboard pattern:
```shell
magick -size {{640x480}} pattern:checkerboard {{checkerboard.png}}
```
#### Convert images to individual PDF pages:
```shell
magick {{*.jpg}} +adjoin {{page-%d.pdf}}
```
{% endraw %}