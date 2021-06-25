---
layout: default
title: "exif"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exif">
  <a href="/en/linux/exif.html">exif</a> <a href="#exif"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show and change EXIF information in JPEG files.
> More information: <https://github.com/libexif/exif/>.

#### Show all recognized EXIF information in an image:
```shell
exif {{path/to/image.jpg}}
```
#### Show a table listing known EXIF tags and whether each one exists in an image:
```shell
exif --list-tags --no-fixup {{image.jpg}}
```
#### Extract the image thumbnail into the file `thumbnail.jpg`:
```shell
exif --extract-thumbnail --output={{thumbnail.jpg}} {{image.jpg}}
```
#### Show the raw contents of the "Model" tag in the given image:
```shell
exif --ifd={{0}} --tag={{Model}} --machine-readable {{image.jpg}}
```
#### Change the value of the "Artist" tag to John Smith and save to `new.jpg`:
```shell
exif --output={{new.jpg}} --ifd={{0}} --tag="{{Artist}}" --set-value="{{John Smith}}" --no-fixup {{image.jpg}}
```
{% endraw %}