---
layout: default
title: "lrunzip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lrunzip">
  <a href="/en/linux/lrunzip.html">lrunzip</a> <a href="#lrunzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A large file decompression program.
> See also `lrzip`, `lrztar`, `lrzuntar`.

#### Decompress a file:
```shell
lrunzip {{filename.lrz}}
```
#### Decompress a file using a specific number of processor threads:
```shell
lrunzip -p {{8}} {{filename.lrz}}
```
#### Decompress a file and silently overwrite files if they exist:
```shell
lrunzip -f {{filename.lrz}}
```
#### Keep broken or damaged files instead of deleting them when decompressing:
```shell
lrunzip -K {{filename.lrz}}
```
#### Specify output file name and/or path:
```shell
lrunzip -o {{outfilename}} {{filename.lrz}}
```
{% endraw %}