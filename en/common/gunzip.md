---
layout: default
title: "gunzip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gunzip">
  <a href="/en/common/gunzip.html">gunzip</a> <a href="#gunzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extract file(s) from a gzip (.gz) archive.
> More information: <https://manned.org/gunzip>.

#### Extract a file from an archive, replacing the original file if it exists:
```shell
gunzip {{archive.tar.gz}}
```
#### Extract a file to a target destination:
```shell
gunzip -c {{archive.tar.gz}} > {{archive.tar}}
```
#### List the contents of a compressed file:
```shell
gunzip -l {{file.txt.gz}}
```
{% endraw %}