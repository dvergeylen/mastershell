---
layout: default
title: "as"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="as">
  <a href="/es/osx/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ensamblador portable GNU.
> Principalmente destinado a ensamblar la salida de `gcc` para ser utilizada por` ld`.

#### Ensambla un archivo, escribiendo la salida en `a.out`:
```shell
as {{archivo.s}}
```
#### Ensambla la salida a un archivo especificado:
```shell
as {{archivo.s}} -o {{salida.o}}
```
#### Genera resultados más rápido omitiendo los espacios en blanco y el preprocesamiento de comentarios. (Solo debe usarse para compiladores de confianza):
```shell
as -f {{archivo.s}}
```
#### Incluye una ruta determinada a la lista de directorios para buscar archivos especificados en las directivas `.include`:
```shell
as -I {{ruta/al/directorio}} {{archivo.s}}
```
{% endraw %}