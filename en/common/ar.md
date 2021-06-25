---
layout: default
title: "ar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ar">
  <a href="/en/common/ar.html">ar</a> <a href="#ar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create, modify, and extract from archives (`.a`, `.so`, `.o`).
> More information: <https://manned.org/ar>.

#### Extract all members from an archive:
```shell
ar -x {{path/to/file.a}}
```
#### List the members of an archive:
```shell
ar -t {{path/to/file.a}}
```
#### Replace or add files to an archive:
```shell
ar -r {{path/to/file.a}} {{path/to/file1.o}} {{path/to/file2.o}}
```
#### Insert an object file index (equivalent to using `ranlib`):
```shell
ar -s {{path/to/file.a}}
```
#### Create an archive with files and an accompanying object file index:
```shell
ar -rs {{path/to/file.a}} {{path/to/file1.o}} {{path/to/file2.o}}
```
{% endraw %}