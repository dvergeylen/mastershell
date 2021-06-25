---
layout: default
title: "apt-file"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-file">
  <a href="/es/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Busca archivos en paquetes apt, incluyendo los que aún no fueron instalados.
> Más información: <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### Actualiza los metadatos de la base de datos:
```shell
sudo apt update
```
#### Busca paquetes que contengan el archivo o ruta especificada:
```shell
apt-file search {{ruta/al/archivo}}
```
#### Muestra el contenido del paquete especificado:
```shell
apt-file list {{nombre_paquete}}
```
{% endraw %}