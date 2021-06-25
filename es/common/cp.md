---
layout: default
title: "cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cp">
  <a href="/es/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copia archivos y directorios.
> Más información: <https://www.gnu.org/software/coreutils/cp>.

#### Copia un archivo a otra ruta:
```shell
cp {{ruta/hacia/archivo_original.ext}} {{ruta/hacia/archivo_copia.ext}}
```
#### Copia un archivo a un directorio, manteniendo el nombre del archivo:
```shell
cp {{ruta/hacia/archivo_original.ext}} {{ruta/hacia/directorio_destino}}
```
#### Copia de forma recursiva un directorio y su contenido a otra ruta (si la ruta de destino existe, el directorio se copiará dentro):
```shell
cp -R {{ruta/hacia/directorio_original}} {{ruta/hacia/directorio_copia}}
```
#### Copia de forma recursiva y verbosa un directorio (muestra un listado de los archivos copiados):
```shell
cp -vR {{ruta/hacia/directorio_original}} {{ruta/hacia/directorio_copia}}
```
#### Copia archivos de texto a otra ruta de forma interactiva (pregunta al usuario antes de sobreescribir):
```shell
cp -i {{*.txt}} {{ruta/hacia/directorio_destino}}
```
#### Copia enlaces simbólicos sin mantener la referencia al original:
```shell
cp -L {{enlace}} {{ruta/hacia/directorio_destino}}
```
{% endraw %}