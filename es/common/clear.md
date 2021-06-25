---
layout: default
title: "clear"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clear">
  <a href="/es/common/clear.html">clear</a> <a href="#clear"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Limpia la pantalla de la terminal.
> Más información: <https://manned.org/clear>.

#### Limpia la pantalla de la terminal (equivale a presionar Control-L en la interfaz de línea de comandos Bash):
```shell
clear
```
#### Limpia la pantalla pero mantiene el buffer de desplazamiento:
```shell
clear -x
```
#### Indica el tipo de terminal a limpiar (por defecto se utiliza el valor de la variable de entorno `TERM`):
```shell
clear -T {{tipo_de_terminal}}
```
#### Muestra la versión de `ncurses` utilizada por `clear`:
```shell
clear -V
```
{% endraw %}