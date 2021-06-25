---
layout: default
title: "chmod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chmod">
  <a href="/es/common/chmod.html">chmod</a> <a href="#chmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambiar los permisos de acceso de un archivo o directorio.
> Más información: <https://www.gnu.org/software/coreutils/chmod>.

#### Otorga al [u]suario que es propietario del archivo permiso para [x] ejecutarlo:
```shell
chmod u+x {{archivo}}
```
#### Otorga al usuario derechos para leer (r) y escribir (w) un archivo o directorio:
```shell
chmod u+rw {{archivo_o_directorio}}
```
#### Elimina los derechos de ejecución del [g]rupo:
```shell
chmod g-x {{archivo}}
```
#### Otorga a todos los usuarios (a) derechos para leer y ejecutar:
```shell
chmod a+rx {{archivo}}
```
#### Otorga a [o]tros (que no están en el grupo del propietario) los mismos derechos que los del grupo:
```shell
chmod o=g {{archivo}}
```
#### Otorga al [g]rupo y a [o]tros el derecho para escribir (w) un directorio y su contenido:
```shell
chmod -R g+w,o+w {{directorio}}
```
{% endraw %}