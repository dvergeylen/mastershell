---
layout: default
title: "gedit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gedit">
  <a href="/en/linux/gedit.html">gedit</a> <a href="#gedit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Text editor of the GNOME Desktop project.

#### Open a text file:
```shell
gedit {{path/to/file}}
```
#### Open multiple text files:
```shell
gedit {{file1 file2 ...}}
```
#### Open a text file with a specific encoding:
```shell
gedit --encoding={{UTF-8}} {{path/to/file}}
```
#### Display a list of supported encodings:
```shell
gedit --list-encodings
```
{% endraw %}