---
layout: default
title: "readelf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="readelf">
  <a href="/en/linux/readelf.html">readelf</a> <a href="#readelf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays information about ELF files.
> More information: <http://man7.org/linux/man-pages/man1/readelf.1.html>.

#### Display all information about the ELF file:
```shell
readelf -all {{path/to/binary}}
```
#### Display all the headers present in the ELF file:
```shell
readelf --headers {{path/to/binary}}
```
#### Display the entries in symbol table section of the ELF file, if it has one:
```shell
readelf --symbols {{path/to/binary}}
```
#### Display the information contained in the ELF header at the start of the file:
```shell
readelf --file-header {{path/to/binary}}
```
{% endraw %}