---
layout: default
title: "convert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="convert">
  <a href="/en/common/convert.html">convert</a> <a href="#convert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ImageMagick image conversion tool.
> More information: <https://imagemagick.org/script/convert.php>.

#### Convert an image from JPG to PNG:
```shell
convert {{image.jpg}} {{image.png}}
```
#### Scale an image 50% its original size:
```shell
convert {{image.png}} -resize 50% {{image2.png}}
```
#### Scale an image keeping the original aspect ratio to a maximum dimension of 640x480:
```shell
convert {{image.png}} -resize 640x480 {{image2.png}}
```
#### Horizontally append images:
```shell
convert {{image1.png}} {{image2.png}} {{image3.png}} +append {{image123.png}}
```
#### Vertically append images:
```shell
convert {{image1.png}} {{image2.png}} {{image3.png}} -append {{image123.png}}
```
#### Create a gif from a series of images with 100ms delay between them:
```shell
convert {{image1.png}} {{image2.png}} {{image3.png}} -delay {{10}} {{animation.gif}}
```
#### Create an image with nothing but a solid background:
```shell
convert -size {{800x600}} "xc:{{#ff0000}}" {{image.png}}
```
#### Create a favicon from several images of different sizes:
```shell
convert {{image1.png}} {{image2.png}} {{image3.png}} {{image.ico}}
```
{% endraw %}