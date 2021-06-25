---
layout: default
title: "aptitude"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aptitude">
  <a href="/es/linux/aptitude.html">aptitude</a> <a href="#aptitude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de gestión de paquetes para Debian y Ubuntu.
> Más información: <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

#### Sincroniza la lista de paquetes y versiones disponible (se recomienda ejecutar este comando antes que cualquier otro comando `aptitude`):
```shell
aptitude update
```
#### Instalar un nuevo paquete y sus dependencias:
```shell
aptitude install {{paquete}}
```
#### Buscar un paquete:
```shell
aptitude search {{paquete}}
```
#### Buscar un paquete instalado (`?installed` es un término de búsqueda de `aptitude`):
```shell
aptitude search '?installed({{paquete}})'
```
#### Elimina un paquete y todos los paquetes que dependen de él:
```shell
aptitude remove {{paquete}}
```
#### Actualiza todos los paquetes sus nuevas versiones disponibles:
```shell
aptitude upgrade
```
#### Actualiza paquetes instalados (como `aptitude upgrade`), elimina los paquetes obsoletos e instala paquetes adicionales para satisfacer sus dependencias:
```shell
aptitude full-upgrade
```
#### Mantiente un paquete instalado para que no sea actualizado automáticamente:
```shell
aptitude hold '?installed({{paquete}})'
```
{% endraw %}