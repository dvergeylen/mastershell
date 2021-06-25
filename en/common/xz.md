---
layout: default
title: "xz"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xz">
  <a href="/en/common/xz.html">xz</a> <a href="#xz"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compress or decompress .xz and .lzma files.
> More information: <https://tukaani.org/xz/format.html>.

#### Compress a file to the xz file format:
```shell
xz {{file}}
```
#### Decompress a xz file:
```shell
xz -d {{file.xz}}
```
#### Compress a file to the lzma file format:
```shell
xz --format=lzma {{file}}
```
#### Decompress an lzma file:
```shell
xz -d --format=lzma {{file.lzma}}
```
#### Decompress a file and write to stdout:
```shell
xz -dc {{file.xz}}
```
#### Compress a file, but don't delete the original:
```shell
xz -k {{file}}
```
#### Compress a file using the fastest compression:
```shell
xz -0 {{file}}
```
#### Compress a file using the best compression:
```shell
xz -9 {{file}}
```
{% endraw %}