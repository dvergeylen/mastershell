---
layout: default
title: "tar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tar">
  <a href="/es/common/tar.html">tar</a> <a href="#tar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta para archivos.
> A veces combinada con un método de compresión, como gzip o bzip2.
> Más información: <https://www.gnu.org/software/tar>.

#### Crear un archivo a partir de otros archivos:
```shell
tar cf {{archivo_destino.tar}} {{archivo1}} {{archivo2}} {{archivo3}}
```
#### Crear un archivo comprimido con gzip:
```shell
tar czf {{archivo_destino.tar.gz}} {{archivo1}} {{archivo2}} {{archivo3}}
```
#### Extraer un archivo (comprimido) en el directorio actual:
```shell
tar xf {{archivo.tar[.gz|.bz2|.xz]}}
```
#### Extraer un archivo en un directorio:
```shell
tar xf {{archivo.tar}} -C {{directorio}}
```
#### Crear un archivo comprimido usando el sufijo para determinar el programa de compresión:
```shell
tar caf {{archivo_destino.tar.xz}} {{archivo1}} {{archivo2}} {{archivo3}}
```
#### Mostrar el contenido de un archivo tar:
```shell
tar tvf {{archivo.tar}}
```
#### Extraer archivos que coinciden con un patrón:
```shell
tar xf {{archivo.tar}} --wildcards "{{*.html}}"
```
{% endraw %}