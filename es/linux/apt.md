---
layout: default
title: "apt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt">
  <a href="/es/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de gestión de paquete para distribuciones basadas en Debian.
> Se recomienda sustituirlo por apt-get cuando se use interactivamente en Ubuntu 16.04 o versiones posteriores.
> Más información: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Actualiza la lista de paquetes y versiones disponibles (se recomienda ejecutar este comando antes que cualquier otro comando `apt`):
```shell
sudo apt update
```
#### Busca un paquete:
```shell
apt search {{paquete}}
```
#### Muestra la información de un paquete:
```shell
apt show {{paquete}}
```
#### Instala un paquete o lo actualiza a su última versión disponible:
```shell
sudo apt install {{paquete}}
```
#### Elimina un paquete (si se utiliza `purge` también elimina sus archivos de configuración):
```shell
sudo apt remove {{paquete}}
```
#### Actualiza todos los paquetes a sus nuevas versiones disponibles:
```shell
sudo apt upgrade
```
#### Muestra todos los paquetes:
```shell
apt list
```
#### Muestra los paquetes instalados:
```shell
apt list --installed
```
{% endraw %}