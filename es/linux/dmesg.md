---
layout: default
title: "dmesg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dmesg">
  <a href="/es/linux/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Escribe los mensajes del núcleo a la salida estándar.

#### Muestra los mensajes del núcleo:
```shell
dmesg
```
#### Muestra los mensajes de error del núcleo:
```shell
dmesg --level err
```
#### Muestra los mensajes del núcleo y sigue leyedos los nuevos, similar a `tail -f` (disponible en los núcleos 3.5.0 y posteriores):
```shell
dmesg -w
```
#### Muestra cuanta memoria física hay disponible en este sistema:
```shell
dmesg | grep -i memory
```
#### Muestra los mensajes del núcleo, página a página:
```shell
dmesg | less
```
#### Muestra los mensajes del núcleo con una estampilla temporal (disponible en los núcleos 3.5.0 y posteriores):
```shell
dmesg -T
```
#### Muestra los mensajes del núcleo de forma legible para humanos (disponible en los núcleos 3.5.0 y posteriores):
```shell
dmesg -H
```
#### Colorea la salida (disponible en los núcleos 3.5.0 y posteriores):
```shell
dmesg -L
```
{% endraw %}