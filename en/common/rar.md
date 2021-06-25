---
layout: default
title: "rar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rar">
  <a href="/en/common/rar.html">rar</a> <a href="#rar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The RAR archiver. Supports multi-volume archives that can be optionally self-extracting.

#### Archive 1 or more files:
```shell
rar a {{path/to/archive_name.rar}} {{path/to/file1}} {{path/to/file2}} {{path/to/file3}}
```
#### Archive a directory:
```shell
rar a {{path/to/archive_name.rar}} {{path/to/directory}}
```
#### Split the archive into parts of equal size (50M):
```shell
rar a -v{{50M}} -R {{path/to/archive_name.rar}} {{path/to/file_or_directory}}
```
#### Password protect the resulting archive:
```shell
rar a -p{{password}} {{path/to/archive_name.rar}} {{path/to/file_or_directory}}
```
#### Encrypt file data and headers with password:
```shell
rar a -hp{{password}} {{path/to/archive_name.rar}} {{path/to/file_or_directory}}
```
#### Use a specific compression level (0-5):
```shell
rar a -m{{compression_level}} {{path/to/archive_name.rar}} {{path/to/file_or_directory}}
```
{% endraw %}