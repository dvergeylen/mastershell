---
layout: default
title: "ls"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ls">
  <a href="/es/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lista los contenidos de directorios.
> Más información: <https://www.gnu.org/software/coreutils/ls>.

#### Lista un archivo por línea:
```shell
ls -1
```
#### Lista todos los archivos, incluyendo archivos ocultos:
```shell
ls -a
```
#### Lista todos los archivos, añadiendo `/` al final de los nombres de directorios:
```shell
ls -F
```
#### Lista todos los archivos con formato largo (permisos, propietario, tamaño y fecha de modificación):
```shell
ls -la
```
#### Lista con formato largo y tamaño legible por humanos (KiB, MiB, GiB):
```shell
ls -lh
```
#### Lista con formato largo y tamaño en orden descendente:
```shell
ls -lS
```
#### Lista todos los archivos con formato largo, ordenado por fecha de modificación (archivos más viejos en primer lugar):
```shell
ls -ltr
```
{% endraw %}