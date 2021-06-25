---
layout: default
title: "dos2unix"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dos2unix">
  <a href="/es/linux/dos2unix.html">dos2unix</a> <a href="#dos2unix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambia saltos de línea con formato DOS a saltos de línea con formato Unix.
> Reemplaza CRLF con CR.

#### Cambia los saltos de línea de un archivo:
```shell
dos2unix {{nombre_de_archivo}}
```
#### Crea una copia con saltos de línea en formato Unix:
```shell
dos2unix -n {{nombre_de_archivo}} {{nombre_de_archivo}}
```
{% endraw %}