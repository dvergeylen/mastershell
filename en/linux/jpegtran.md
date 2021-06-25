---
layout: default
title: "jpegtran"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jpegtran">
  <a href="/en/linux/jpegtran.html">jpegtran</a> <a href="#jpegtran"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Perform lossless transformation of JPEG files.
> More information: <https://manned.org/jpegtran>.

#### Mirror an image horizontally or vertically:
```shell
jpegtran -flip {{horizontal|vertical}} {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
#### Rotate an image 90, 180 or 270 degrees clockwise:
```shell
jpegtran -rotate {{90|180|270}} {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
#### Transpose the image across the upper left to lower right axis:
```shell
jpegtran -transpose {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
#### Transverse the image across the upper right to lower left axis:
```shell
jpegtran -transverse {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
#### Convert the image to grayscale:
```shell
jpegtran -grayscale {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
#### Crop the image to a rectangular region of width `W` and height `H` from the upper left corner, saving the output to a specific file:
```shell
jpegtran -crop {{W}}x{{H}} -outfile {{path/to/output.jpg}} {{path/to/image.jpg}}
```
#### Crop the image to a rectangular region of width `W` and height `H`, starting at point `X` and `Y` from the upper left corner:
```shell
jpegtran -crop {{W}}x{{H}}+{{X}}+{{Y}} {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
{% endraw %}