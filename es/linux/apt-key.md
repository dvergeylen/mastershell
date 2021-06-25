---
layout: default
title: "apt-key"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-key">
  <a href="/es/linux/apt-key.html">apt-key</a> <a href="#apt-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta para la gestión de claves para el Gestor de Paquetes APT (APT Package Manager) en Debian y Ubuntu.
> Más información: <https://manpages.debian.org/latest/apt/apt-key.8.html>.

#### Muestra las claves de confianza:
```shell
apt-key list
```
#### Añade una clave al almacén de claves de confianza):
```shell
apt-key add {{archivo_clave_pública.asc}}
```
#### Borrar una clave del almacén de claves de confianza:
```shell
apt-key del {{id_clave}}
```
#### Añadir un clave remota al almacén de claves de confianza:
```shell
wget -qO - {{https://host.tld/archivo.clave}} | apt-key add -
```
#### Añadir una clave de un servidor de claves con el identificador de la clave:
```shell
apt-key adv --keyserver {{pgp.mit.edu}} --recv {{id_clave}}
```
{% endraw %}