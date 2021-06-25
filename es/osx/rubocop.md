---
layout: default
title: "rubocop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rubocop">
  <a href="/es/osx/rubocop.html">rubocop</a> <a href="#rubocop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analiza archivos de Ruby.

#### Verifica todos los archivos en el directorio actual (incluyendo subdirectorios):
```shell
rubocop
```
#### Verifica uno o más archivos o directorios determinados:
```shell
rubocop {{path/to/file}} {{path/to/directory}}
```
#### Guarda la salida en un archivo:
```shell
rubocop --out {{path/to/file}}
```
#### Muestra la lista de cops (reglas de análisis):
```shell
rubocop --show-cops
```
#### Excluye una regla:
```shell
rubocop --except {{cop_1}} {{cop_2}}
```
#### Ejecuta sólo determinadas reglas:
```shell
rubocop --only {{cop_1}} {{cop_2}}
```
#### Autocorrige archivos (experimental):
```shell
rubocop --auto-correct
```
{% endraw %}