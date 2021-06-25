---
layout: default
title: "ect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ect">
  <a href="/it/common/ect.html">ect</a> <a href="#ect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Efficiente Tool di Compressione (o ECT) è un ottimizzatore di file scritto in C++. Supporta file PNG, JPEG, GZIP e ZIP.
> Maggiori informazioni: <https://github.com/fhanau/Efficient-Compression-Tool>.

#### Comprimi un file:
```shell
ect {{file.png}}
```
#### Comprimi un file con il massimo livello di compressione utilizzanto più thread:
```shell
ect -9 --mt-deflate {{file.png}}
```
#### Comprimi tutti i file in una directory ricorsivamente, mantenendo la data di modifica originale:
```shell
ect -keep -recurse {{percorso/a/directory}}
```
{% endraw %}