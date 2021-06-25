---
layout: default
title: "rm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rm">
  <a href="/es/common/rm.html">rm</a> <a href="#rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elimina archivos o directorios.
> Más información: <https://www.gnu.org/software/coreutils/rm>.

#### Elimina archivos de ubicaciones arbitrarias:
```shell
rm {{ruta/al/archivo}} {{ruta/al/otro/archivo}}
```
#### Elimina, de forma recursiva, un directorio y todos sus subdirectorios:
```shell
rm -r {{ruta/al/directorio}}
```
#### Elimina un directorio a la fuerza, sin pedir confirmación ni mostrar mensajes de error:
```shell
rm -rf {{ruta/al/directorio}}
```
#### Elimina varios archivos de forma interactiva, solicitando confirmación antes de eliminar cada archivo:
```shell
rm -i {{archivo(s)}}
```
#### Elimina archivos en modo detallado, imprimiendo un mensaje por cada archivo eliminado:
```shell
rm -v {{ruta/hacia/directorio/*}}
```
{% endraw %}