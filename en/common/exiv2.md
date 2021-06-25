---
layout: default
title: "exiv2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exiv2">
  <a href="/en/common/exiv2.html">exiv2</a> <a href="#exiv2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Image metadata manipulation tool.
> More information: <https://www.exiv2.org/manpage.html>.

#### Print a summary of the image Exif metadata:
```shell
exiv2 {{path/to/file}}
```
#### Print all metadata (Exif, IPTC, XMP) with interpreted values:
```shell
exiv2 -P kt {{path/to/file}}
```
#### Print all metadata with raw values:
```shell
exiv2 -P kv {{path/to/file}}
```
#### Delete all metadata from an image:
```shell
exiv2 -d a {{path/to/file}}
```
#### Delete all metadata, preserving the file timestamp:
```shell
exiv2 -d a -k {{path/to/file}}
```
#### Rename the file, prepending the date and time from metadata (not from the file timestamp):
```shell
exiv2 -r {{'%Y%m%d_%H%M%S_:basename:'}} {{path/to/file}}
```
{% endraw %}