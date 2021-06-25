---
layout: default
title: "apt-mark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-mark">
  <a href="/es/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta para cambiar el estado de los paquetes instalados.
> Más información: <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### Marca un paquete como instalado automáticamente:
```shell
sudo apt-mark auto {{nombre_paquete}}
```
#### Mantiene un paquete en su versión actual y evita que se actualice:
```shell
sudo apt-mark hold {{nombre_paquete}}
```
#### Permite que un paquete pueda ser actualizado de nuevo:
```shell
sudo apt-mark unhold {{nombre_paquete}}
```
#### Muestra los paquetes instalados manualmente:
```shell
apt-mark showmanual
```
#### Muestra los paquetes mantenidos que no son actualizados:
```shell
apt-mark showhold
```
{% endraw %}