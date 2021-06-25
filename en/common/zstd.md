---
layout: default
title: "zstd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zstd">
  <a href="/en/common/zstd.html">zstd</a> <a href="#zstd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compress or decompress files with Zstandard compression.
> More information: <https://github.com/facebook/zstd>.

#### Compress a file into a new file with the `.zst` suffix:
```shell
zstd {{file}}
```
#### Decompress a file:
```shell
zstd -d {{file}}.zst
```
#### Decompress to stdout:
```shell
zstd -dc {{file}}.zst
```
#### Compress a file specifying the compression level, where 1=fastest, 19=slowest and 3=default:
```shell
zstd -{{level}} {{file}}
```
#### Unlock higher compression levels (up to 22) using more memory (both for compression and decompression):
```shell
zstd --ultra -{{level}} {{file}}
```
{% endraw %}