---
layout: default
title: "unrar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="unrar">
  <a href="/es/common/unrar.html">unrar</a> <a href="#unrar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extrae archivos RAR.

#### Extrae archivos comprimidos respetando la estructura original del archivo:
```shell
unrar x {{archivo_comprimido.rar}}
```
#### Extrae archivos comprimidos en una ruta determinada respetando la estructura original del archivo:
```shell
unrar x {{archivo_comprimido.rar}} {{ruta/donde/extraer}}
```
#### Extrae archivos comprimidos en el directorio actual, perdiendo la estructura original del archivo:
```shell
unrar e {{archivo_comprimido.rar}}
```
#### Comprueba la integridad de cada uno de los archivos dentro del archivo comprimido:
```shell
unrar t {{archivo_comprimido.rar}}
```
#### Muestra el listado de los archivos dentro del archivo comprimido sin descomprimirlo:
```shell
unrar l {{archivo_comprimido.rar}}
```
{% endraw %}