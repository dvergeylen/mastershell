---
layout: default
title: "exiftool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="exiftool">
  <a href="/en/common/exiftool.html">exiftool</a> <a href="#exiftool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read and write meta information in files.
> More information: <https://exiftool.org>.

#### Remove all EXIF metadata from the given files:
```shell
exiftool -All= {{file1 file2 ...}}
```
#### Move the date at which all photos in a directory were taken 1 hour forward:
```shell
exiftool "-AllDates+=0:0:0 1:0:0" {{path/to/directory}}
```
#### Move the date at which all JPEG photos in the current directory were taken 1 day and 2 hours backward:
```shell
exiftool "-AllDates-=0:0:1 2:0:0" -ext jpg
```
#### Only change the `DateTimeOriginal` field subtracting 1.5 hours, without keeping backups:
```shell
exiftool -DateTimeOriginal-=1.5 -overwrite_original
```
#### Recursively rename all JPEG photos in a directory based on the `DateTimeOriginal` field:
```shell
exiftool '-filename<DateTimeOriginal' -d %Y-%m-%d_%H-%M-%S%%lc.%%e {{path/to/directory}} -r -ext jpg
```
{% endraw %}