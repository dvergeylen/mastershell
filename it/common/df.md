---
layout: default
title: "df"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="df">
  <a href="/it/common/df.html">df</a> <a href="#df"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fornisce una panoramica dello spazio utilizzato dai file system sui dischi.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/df>.

#### Mostra tutti i file system ed il loro utilizzo del disco:
```shell
df
```
#### Mostra tutti i file system ed il loro utilizzo del disco in formato leggibile dall'uomo:
```shell
df -h
```
#### Mostra il file system ed contenente il file o directory dato ed il suo utilizzo del disco:
```shell
df {{percorso/a/file_o_directory}}
```
{% endraw %}