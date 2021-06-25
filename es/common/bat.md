---
layout: default
title: "bat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bat">
  <a href="/es/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Imprime y concatena archivos.
> Un clon de `cat` con resaltado de sintaxis e integración con Git.
> Más información: <https://github.com/sharkdp/bat>.

#### Imprime los contenidos de un archivo a la salida estándar:
```shell
bat {{archivo}}
```
#### Concatena varios archivos creando un nuevo archivo:
```shell
bat {{archivo1}} {{archivo2}} > {{archivo_final}}
```
#### Añade múltiples archivos al final de un archivo objetivo:
```shell
bat {{archivo1}} {{archivo2}} >> {{archivo_final}}
```
#### Numera las lineas del archivo:
```shell
bat -n {{archivo}}
```
#### Muestra un archivo JSON con resaltado de sintaxis:
```shell
bat --language json {{archivo.json}}
```
#### Muestra todos los lenguajes permitidos:
```shell
bat --list-languages
```
{% endraw %}