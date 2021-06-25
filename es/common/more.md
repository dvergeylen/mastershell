---
layout: default
title: "more"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="more">
  <a href="/es/common/more.html">more</a> <a href="#more"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Abre un archivo para lectura interactiva, permitiendo navegar y buscar.
> Más información: <https://manned.org/more>.

#### Abre un archivo:
```shell
more {{ruta/al/archivo}}
```
#### Abre un archivo mostrando desde una línea especifica:
```shell
more +{{numero_linea}} {{ruta/al/archivo}}
```
#### Muestra la ayuda:
```shell
more --help
```
#### Avanza hacia la siguiente página:
```shell
<Espacio>
```
#### Busca una cadena (presione `n` para ir a la siguiente coincidencia):
```shell
/{{cadena}}
```
#### Salir:
```shell
q
```
#### Muestra la ayuda sobre comandos interactivos:
```shell
h
```
{% endraw %}