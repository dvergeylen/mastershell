---
layout: default
title: "sips"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sips">
  <a href="/en/osx/sips.html">sips</a> <a href="#sips"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apple Scriptable Image Processing System.
> Raster/Query images and ColorSync ICC Profiles.

#### Specify an output directory so that originals do not get modified:
```shell
sips --out {{path/to/out_dir}}
```
#### Resample image at specified size, Image aspect ratio may be altered:
```shell
sips -z {{1920}} {{300}} {{image.ext}}
```
#### Resample image so height and width aren't greater than specified size (notice the capital Z):
```shell
sips -Z {{1920}} {{300}} {{image.ext}}
```
#### Resample all images in a directory to fit a width of 960px (honoring aspect ratio):
```shell
sips --resampleWidth {{960}} {{path/to/images}}
```
#### Convert an image from CMYK to RGB:
```shell
sips --matchTo '/System/Library/ColorSync/Profiles/Generic RGB Profile.icc' {{path/to/image.ext}} {{path/to/out_dir}}
```
#### Remove ColorSync ICC profile from an image:
```shell
sips -d profile --deleteColorManagementProperties {{path/to/image.ext}}
```
{% endraw %}