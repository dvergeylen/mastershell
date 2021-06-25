---
layout: default
title: "zcat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zcat">
  <a href="/en/common/zcat.html">zcat</a> <a href="#zcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print data from gzip compressed files.

#### Print the uncompressed contents of a gzipped file to the standard output:
```shell
zcat {{file.txt.gz}}
```
#### Print compression details of a gzipped file to the standard output:
```shell
zcat -l {{file.txt.gz}}
```
{% endraw %}