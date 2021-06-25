---
layout: default
title: "afinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="afinfo">
  <a href="/es/osx/afinfo.html">afinfo</a> <a href="#afinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analizador de metadatos de archivos de audio para OS X.
> Comando nativo de OS X.

#### Muestra información de un archivo de audio dado:
```shell
afinfo {{ruta/al/archivo}}
```
#### Muestra una descripción de una línea del archivo de audio:
```shell
afinfo -b {{ruta/al/archivo}}
```
#### Muestra información de metadatos y contenido del InfoDictionary del archivo de audio:
```shell
afinfo -i {{ruta/al/archivo}}
```
#### Imprime la salida en formato XML:
```shell
afinfo -x {{ruta/al/archivo}}
```
#### Muestra advertencias para el archivo de audio, si las hubiera:
```shell
afinfo --warnings {{ruta/al/archivo}}
```
#### Muestra ayuda para un uso completo:
```shell
afinfo -h
```
{% endraw %}