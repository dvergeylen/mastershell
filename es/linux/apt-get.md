---
layout: default
title: "apt-get"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-get">
  <a href="/es/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de gestión de paquete para distribuciones basadas en Debian.
> Buscar paquetes utilizando `apt-cache`.
> Más información: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Actualiza la lista de paquetes y versiones disponibles (se recomienda ejecutar este comando antes que cualquier otro comando `apt-get`):
```shell
apt-get update
```
#### Instala un paquete o actualizarlo a su última versión disponible:
```shell
apt-get install {{paquete}}
```
#### Elimina un paquete:
```shell
apt-get remove {{paquete}}
```
#### Elimina un paquete y sus archivos de configuración:
```shell
apt-get purge {{paquete}}
```
#### Actualiza todos los paquetes instalados a sus nuevas versiones disponibles:
```shell
apt-get upgrade
```
#### Elimina todos los paquetes innecesarios:
```shell
apt-get autoremove
```
#### Actualiza paquetes instalados (como `upgrade`), pero elimina paquete obsoletos e instala paquetes adiciones para satisfacer nuevas dependencias:
```shell
apt-get dist-upgrade
```
{% endraw %}