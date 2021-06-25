---
layout: default
title: "lz4"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lz4">
  <a href="/en/common/lz4.html">lz4</a> <a href="#lz4"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compress or decompress .lz4 files.
> More information: <https://github.com/lz4/lz4>.

#### Compress a file:
```shell
lz4 {{file}}
```
#### Decompress a file:
```shell
lz4 -d {{file.lz4}}
```
#### Decompress a file and write to stdout:
```shell
lz4 -dc {{file.lz4}}
```
#### Package and compress a directory and its contents:
```shell
tar cvf - {{path/to/directory}} | lz4 - {{dir.tar.lz4}}
```
#### Decompress and unpack a directory and its contents:
```shell
lz4 -d {{dir.tar.lz4}} | tar -xv
```
#### Compress a file using the best compression:
```shell
lz4 -9 {{file}}
```
{% endraw %}