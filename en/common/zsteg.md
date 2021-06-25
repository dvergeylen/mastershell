---
layout: default
title: "zsteg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zsteg">
  <a href="/en/common/zsteg.html">zsteg</a> <a href="#zsteg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Steganography detection tool for PNG and BMP file formats.
> It detects LSB steganography, ZLIB-compressed data, OpenStego, Camouflage and LSB with the Eratosthenes set.
> More information: <https://github.com/zed-0xff/zsteg>.

#### Detect embedded data in a PNG image:
```shell
zsteg {{path/to/image.png}}
```
#### Detect embedded data in a BMP image, using all known methods:
```shell
zsteg --all {{path/to/image.bmp}}
```
#### Detect embedded data in a PNG image, iterating pixels vertically and using MSB first:
```shell
zsteg --msb --order yx {{path/to/image.png}}
```
#### Detect embedded data in a BMP image, specifying the bits to consider:
```shell
zsteg --bits {{1,2,3|1-3}} {{path/to/image.bmp}}
```
#### Detect embedded data in a PNG image, extracting only prime pixels and inverting bits:
```shell
zsteg --prime --invert {{path/to/image.png}}
```
#### Detect embedded data in a BMP image, specifying the minimum length of the strings to be found and the find mode:
```shell
zsteg --min-str-len {{10}} --strings {{first|all|longest|none}} {{path/to/image.bmp}}
```
{% endraw %}