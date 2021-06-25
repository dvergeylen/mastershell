---
layout: default
title: "fortune"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fortune">
  <a href="/es/common/fortune.html">fortune</a> <a href="#fortune"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Imprime por pantalla una cita aleatoria (al estilo de una galleta de la suerte).
> Más información: <https://man.archlinux.org/man/fortune.6>.

#### Imprime por pantalla una cita:
```shell
fortune
```
#### Imprime por pantalla una cita ofensiva:
```shell
fortune -o
```
#### Imprime por pantalla una cita larga:
```shell
fortune -l
```
#### Imprime por pantalla una cita corta:
```shell
fortune -s
```
#### Muestra una lista de los archivos de citas disponibles:
```shell
fortune -f
```
#### Imprime por pantalla una cita de uno de los archivos mostrados en `fortune -f`:
```shell
fortune {{archivo}}
```
{% endraw %}