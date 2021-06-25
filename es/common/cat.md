---
layout: default
title: "cat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cat">
  <a href="/es/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Imprime y concatena archivos.
> Más información: <https://www.gnu.org/software/coreutils/cat>.

#### Imprime el contenido de un archivo por la salida estándar:
```shell
cat {{archivo}}
```
#### Concatena múltiples archivos dentro de un archivo determinado:
```shell
cat {{archivo1}} {{archivo2}} > {{archivo_final}}
```
#### Añade múltiples archivos dentro de un archivo determinado:
```shell
cat {{archivo1}} {{archivo2}} >> {{archivo_final}}
```
#### Muestra el número de líneas de un archivo:
```shell
cat -n {{archivo}}
```
#### Muestra los carácteres no imprimibles y espacios en blanco (con el prefijo `M-` si no es ASCII):
```shell
cat -v -t -e {{archivo}}
```
{% endraw %}