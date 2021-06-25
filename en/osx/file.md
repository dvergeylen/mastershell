---
layout: default
title: "file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="file">
  <a href="/en/osx/file.html">file</a> <a href="#file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Determine file type.

#### Give a description of the type of the specified file. Works fine for files with no file extension:
```shell
file {{filename}}
```
#### Look inside a zipped file and determine the file type(s) inside:
```shell
file -z {{foo.zip}}
```
#### Allow file to work with special or device files:
```shell
file -s {{filename}}
```
#### Don't stop at first file type match; keep going until the end of the file:
```shell
file -k {{filename}}
```
#### Determine the mime encoding type of a file:
```shell
file -I {{filename}}
```
{% endraw %}