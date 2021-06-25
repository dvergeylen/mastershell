---
layout: default
title: "bzip2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bzip2">
  <a href="/en/common/bzip2.html">bzip2</a> <a href="#bzip2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A block-sorting file compressor.
> More information: <http://bzip.org>.

#### Compress a file:
```shell
bzip2 {{path/to/file_to_compress}}
```
#### Decompress a file:
```shell
bzip2 -d {{path/to/compressed_file.bz2}}
```
#### Decompress a file to standard output:
```shell
bzip2 -dc {{path/to/compressed_file.bz2}}
```
{% endraw %}