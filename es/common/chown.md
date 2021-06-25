---
layout: default
title: "chown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chown">
  <a href="/es/common/chown.html">chown</a> <a href="#chown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambia la propiedad de usuario y grupo sobre archivos y directorios.
> Más información: <https://www.gnu.org/software/coreutils/chown>.

#### Cambia el usuario propietario de un archivo/directorio:
```shell
chown {{usuario}} {{ruta/hacia/archivo_o_directorio}}
```
#### Cambia el usuario y grupo propietario de un archivo/directorio:
```shell
chown {{usuario}}:{{grupo}} {{ruta/hacia/archivo_o_directorio}}
```
#### Cambia de forma recursiva el propietario sobre un directorio y su contenido:
```shell
chown -R {{usuario}} {{ruta/hacia/directorio}}
```
#### Cambia el propietario de un enlace simbólico:
```shell
chown -h {{usuario}} {{ruta/hacia/enlace_simbolico}}
```
#### Copia la información de propiedad del archivo/directorio de referencia a otro:
```shell
chown --reference={{ruta/hacia/archivo_o_directorio_de_referencia}} {{ruta/hacia/archivo_o_directorio}}
```
{% endraw %}