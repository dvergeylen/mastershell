---
layout: default
title: "libreoffice"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="libreoffice">
  <a href="/en/linux/libreoffice.html">libreoffice</a> <a href="#libreoffice"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for the powerful and free office suite LibreOffice.
> More information: <https://www.libreoffice.org/>.

#### Open a space-separated list of files in read-only mode:
```shell
libreoffice --view {{path/to/file1}} {{path/to/file2}}
```
#### Display the content of specific files:
```shell
libreoffice --cat {{path/to/file1}} {{path/to/file2}}
```
#### Print files to a specific printer:
```shell
libreoffice --pt {{printer_name}} {{path/to/file1}} {{path/to/file2}}
```
#### Convert all `.doc` files in current directory to pdf:
```shell
libreoffice --convert-to {{pdf}} {{*.doc}}
```
{% endraw %}