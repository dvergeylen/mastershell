---
layout: default
title: "lsb_release"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lsb_release">
  <a href="/es/linux/lsb_release.html">lsb_release</a> <a href="#lsb_release"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Proporciona información específica de la distribución y LSB (Linux Standard Base).

#### Muestra toda la información disponible:
```shell
lsb_release -a
```
#### Muestra una descripción del sistema operativo (normalmente el nombre completo):
```shell
lsb_release -d
```
#### Muestra solo el nombre del sistema operativo (ID) sin el campo nombre:
```shell
lsb_release -i -s
```
#### Muestra el número de versión y el nombre en clave de la distribución sin el campo de nombre:
```shell
lsb_release -rcs
```
{% endraw %}