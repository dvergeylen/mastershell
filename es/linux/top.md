---
layout: default
title: "top"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="top">
  <a href="/es/linux/top.html">top</a> <a href="#top"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra información dinámica en tiempo real sobre procesos ejecutándose.

#### Inicia top:
```shell
top
```
#### No muestra ningún proceso inactivo o zombie:
```shell
top -i
```
#### Muestra solo procesos pertenecientes a un usuario dado:
```shell
top -u {{usuario}}
```
#### Ordena procesos por una columna:
```shell
top -o {{nombre_columna}}
```
#### Muestra los hilos individuales de un proceso dado:
```shell
top -Hp {{id_proceso}}
```
#### Muestra solo los procesos con un(os) PID(s) dado(s), sepadados por comas. (Normalmente no se conoce el PID de antemano. Este ejemplo lo obtiene del nombre del proceso):
```shell
top -p $(pgrep -d ',' {{nombre_proceso}})
```
#### Obtiene ayuda acerca de los comandos interactivos:
```shell
?
```
{% endraw %}