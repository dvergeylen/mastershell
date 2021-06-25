---
layout: default
title: "touch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="touch">
  <a href="/es/common/touch.html">touch</a> <a href="#touch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambia el tiempo de accesso y modificación de un archivo (atime, mtime).
> Más información: <https://www.gnu.org/software/coreutils/touch>.

#### Crea un archivo nuevo o cambia los tiempos de archivos existentes al tiempo actual:
```shell
touch {{archivo}}
```
#### Establece los tiempos de un archivo a un dia y hora específicos:
```shell
touch -t {{YYYYMMDDHHMM.SS}} {{archivo}}
```
#### Usa los tiempos de un archivo para establecer los tiempos en otro archivo:
```shell
touch -r {{archivo}} {{archivo2}}
```
{% endraw %}