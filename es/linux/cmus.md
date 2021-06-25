---
layout: default
title: "cmus"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmus">
  <a href="/es/linux/cmus.html">cmus</a> <a href="#cmus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reproductor de música para la línea de comandos.
> Usa las teclas de dirección para navegar, `<enter/return>` para seleccionar, y los números 1-8 para cambiar entra las diferentes vistas.

#### Abre cmus en un directorio concreto:
```shell
cmus {{ruta/al/directorio}}
```
#### Añade un archivo/directorio a la librería:
```shell
:add {{ruta/al/archivo_o_directorio}}
```
#### Pausa/reproduce la canción actual:
```shell
c
```
#### Activa/desactiva modo aleatorio:
```shell
s
```
#### Cierra cmus:
```shell
q
```
{% endraw %}