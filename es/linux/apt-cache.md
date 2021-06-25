---
layout: default
title: "apt-cache"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-cache">
  <a href="/es/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de consulta de paquetes para Debian y Ubuntu.
> Más información: <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### Busca un paquete en tus fuentes actuales:
```shell
apt-cache search {{consulta}}
```
#### Muestra información de un paquete:
```shell
apt-cache show {{paquete}}
```
#### Muestra si un paquete está instalado y actualizado:
```shell
apt-cache policy {{paquete}}
```
#### Muestra las dependencias de un paquete:
```shell
apt-cache depends {{paquete}}
```
#### Muestra los paquetes que dependen de un paquete en particular:
```shell
apt-cache rdepends {{paquete}}
```
{% endraw %}