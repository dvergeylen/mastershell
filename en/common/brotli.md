---
layout: default
title: "Brotli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brotli">
  <a href="/en/common/brotli.html">Brotli</a> <a href="#brotli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compress/uncompress files with brotli compression.
> More information: <https://github.com/google/brotli>.

#### Compress a file, creating a compressed version next to the file:
```shell
brotli {{file.ext}}
```
#### Decompress a file, creating an uncompressed version next to the file:
```shell
brotli -d {{file.ext}}.br
```
#### Compress a file specifying the output filename:
```shell
brotli {{file.ext}} -o {{compressed_file.ext.br}}
```
#### Decompress a brotli file specifying the output filename:
```shell
brotli -d {{compressed_file.ext.br}} -o {{file.ext}}
```
#### Specify the compression level. 1=Fastest (Worst), 11=Slowest (Best):
```shell
brotli -q {{11}} {{file.ext}} -o {{compressed_file.ext.br}}
```
{% endraw %}