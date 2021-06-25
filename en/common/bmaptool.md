---
layout: default
title: "bmaptool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bmaptool">
  <a href="/en/common/bmaptool.html">bmaptool</a> <a href="#bmaptool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create or copy block maps intelligently (designed to be faster than `cp` or `dd`).
> More information: <https://source.tizen.org/documentation/reference/bmaptool>.

#### Create a blockmap from image file:
```shell
bmaptool create -o {{blockmap.bmap}} {{source.img}}
```
#### Copy an image file into sdb:
```shell
bmaptool copy --bmap {{blockmap.bmap}} {{source.img}} {{/dev/sdb}}
```
#### Copy a compressed image file into sdb:
```shell
bmaptool copy --bmap {{blockmap.bmap}} {{source.img.gz}} {{/dev/sdb}}
```
#### Copy an image file into sdb without using a blockmap:
```shell
bmaptool copy --nobmap {{source.img}} {{/dev/sdb}}
```
{% endraw %}