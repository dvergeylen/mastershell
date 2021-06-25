---
layout: default
title: "dnf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dnf">
  <a href="/es/linux/dnf.html">dnf</a> <a href="#dnf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administrador de paquetes para RHEL, CentOS y Fedora (Reemplaza a yum).
> Más información: <https://dnf.readthedocs.io>.

#### Actualiza todos los paquetes a la última versión disponible:
```shell
sudo dnf update
```
#### Busca un paquete usando palabras clave:
```shell
dnf search {{palabra_clave}}
```
#### Muestra información acerca de un paquete:
```shell
dnf info {{paquete}}
```
#### Instala un nuevo paquete:
```shell
sudo dnf install {{paquete}}
```
#### Instala un nuevo paquete respondiendo si a todas las preguntas:
```shell
sudo dnf install -y {{paquete}}
```
#### Lista todos los paquetes instalados:
```shell
dnf list --installed
```
#### Encuentra que paquete provee un archivo determinado:
```shell
dnf provides {{archivo}}
```
{% endraw %}