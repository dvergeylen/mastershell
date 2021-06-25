---
layout: default
title: "free"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="free">
  <a href="/es/linux/free.html">free</a> <a href="#free"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra la cantidad de memoria libre y usada en el sistema.

#### Muestra la memoria del sistema:
```shell
free
```
#### Muestra la memoria del sistema en Bytes/KB/MB/GB:
```shell
free -{{b|k|m|g}}
```
#### Muestra la memoria del sistema en unidades legibles por humanos:
```shell
free -h
```
#### Actualiza la salida cada 2 segundos:
```shell
free -s {{2}}
```
{% endraw %}