---
layout: default
title: "lrzuntar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lrzuntar">
  <a href="/en/linux/lrzuntar.html">lrzuntar</a> <a href="#lrzuntar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A wrapper for `lrunzip` to simplify decompression of directories.
> See also: `lrztar`, `lrzip`.

#### Decompress from a file to the current directory:
```shell
lrzuntar {{path/to/archive.tar.lrz}}
```
#### Decompress from a file to the current directory using a specific number of processor threads:
```shell
lrzuntar -p {{8}} {{path/to/archive.tar.lrz}}
```
#### Decompress from a file to the current directory and silently overwrite items that already exist:
```shell
lrzuntar -f {{archive.tar.lrz}}
```
#### Specify the output path:
```shell
lrzuntar -O {{path/to/directory}} {{archive.tar.lrz}}
```
#### Delete the compressed file after decompression:
```shell
lrzuntar -D {{path/to/archive.tar.lrz}}
```
{% endraw %}