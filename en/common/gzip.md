---
layout: default
title: "gzip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gzip">
  <a href="/en/common/gzip.html">gzip</a> <a href="#gzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compress/uncompress files with gzip compression (LZ77).
> More information: <https://www.gnu.org/software/gzip/manual/gzip.html>.

#### Compress a file, replacing it with a gzipped compressed version:
```shell
gzip {{file.ext}}
```
#### Decompress a file, replacing it with the original uncompressed version:
```shell
gzip -d {{file.ext}}.gz
```
#### Compress a file specifying the output filename:
```shell
gzip -c {{file.ext}} > {{compressed_file.ext.gz}}
```
#### Decompress a gzipped file specifying the output filename:
```shell
gzip -c -d {{file.ext}}.gz > {{uncompressed_file.ext}}
```
#### Specify the compression level. 1=Fastest (Worst), 9=Slowest (Best), Default level is 6:
```shell
gzip -9 -c {{file.ext}} > {{compressed_file.ext.gz}}
```
{% endraw %}