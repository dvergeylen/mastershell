---
layout: default
title: "bzip2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bzip2">
  <a href="/it/common/bzip2.html">bzip2</a> <a href="#bzip2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compressore di file a blocchi ordinati.
> Maggiori informazioni: <http://bzip.org>.

#### Comprimi un file:
```shell
bzip2 {{percorso/al/file}}
```
#### Decomprimi un file:
```shell
bzip2 -d {{percorso/al/file_compresso.bz2}}
```
#### Decomprimi un file e mostrane il contenuto su standard output:
```shell
bzip2 -dc {{percorso/al/file_compresso.bz2}}
```
{% endraw %}