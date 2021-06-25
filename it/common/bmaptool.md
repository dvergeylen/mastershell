---
layout: default
title: "bmaptool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bmaptool">
  <a href="/it/common/bmaptool.html">bmaptool</a> <a href="#bmaptool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea o copia blockmap intelligentemente (e quindi più velocemente di `cp` o `dd`).
> Maggiori informazioni: <https://source.tizen.org/documentation/reference/bmaptool>.

#### Crea una blockmap da un file immagine:
```shell
bmaptool create -o {{blockmap.bmap}} {{sorgente.img}}
```
#### Copia un file immagine su sdb:
```shell
bmaptool copy --bmap {{blockmap.bmap}} {{sorgente.img}} {{/dev/sdb}}
```
#### Copia un file immagine compresso su sdb:
```shell
bmaptool copy --bmap {{blockmap.bmap}} {{sorgente.img.gz}} {{/dev/sdb}}
```
#### Copia un file immagine su sdb senza utilizzare una blockmap:
```shell
bmaptool copy --nobmap {{sorgente.img}} {{/dev/sdb}}
```
{% endraw %}