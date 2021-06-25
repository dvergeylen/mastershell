---
layout: default
title: "cal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cal">
  <a href="/es/linux/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra el calendario, con el día actual resaltado.

#### Muestra el calendario para el mes actual:
```shell
cal
```
#### Muestra el mes anterior, actual y próximo:
```shell
cal -3
```
#### Usa el Lunes como primer día de la semana:
```shell
cal --monday
```
#### Muestra el calendario para un año concreto (4 dígitos):
```shell
cal {{year}}
```
#### Muestra el calendario para un año y mes concretos:
```shell
cal {{month}} {{year}}
```
{% endraw %}