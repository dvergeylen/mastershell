---
layout: default
title: "unrar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unrar">
  <a href="/en/common/unrar.html">unrar</a> <a href="#unrar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extract RAR archives.

#### Extract files with original directory structure:
```shell
unrar x {{compressed.rar}}
```
#### Extract files to a specified path with the original directory structure:
```shell
unrar x {{compressed.rar}} {{path/to/extract}}
```
#### Extract files into current directory, losing directory structure in the archive:
```shell
unrar e {{compressed.rar}}
```
#### Test integrity of each file inside the archive file:
```shell
unrar t {{compressed.rar}}
```
#### List files inside the archive file without decompressing it:
```shell
unrar l {{compressed.rar}}
```
{% endraw %}