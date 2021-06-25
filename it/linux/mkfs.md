---
layout: default
title: "mkfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mkfs">
  <a href="/it/linux/mkfs.html">mkfs</a> <a href="#mkfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Costruisce un filesystem Linux su una partizione del disco rigido.
> Questo comando è deprecato in favore degli strumenti specifici per filesystem: mkfs.<tipo>.

#### Costruisce un filesystem Linux ext2 su una partizione:
```shell
mkfs {{percorso/alla/partizione}}
```
#### Costruisce un filesystem del tipo specificato:
```shell
mkfs -t {{ext4}} {{percorso/alla/partizione}}
```
#### Costruisce un filesystem del specificato e controlla la presenza di settori danneggiati:
```shell
mkfs -c -t {{ntfs}} {{percorso/alla/partizione}}
```
{% endraw %}