---
layout: default
title: "yes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yes">
  <a href="/es/common/yes.html">yes</a> <a href="#yes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retorna algo repetidamente.
> Este comando es frecuentemente utilizado para aceptar todas las confirmaciones en comandos de instalación (como apt-get).
> Más información: <https://www.gnu.org/software/coreutils/yes>.

#### Retornar repetidamente "mensaje":
```shell
yes {{mensaje}}
```
#### Retornar repetidamente "y":
```shell
yes
```
#### Aceptar todas las confirmaciones que muestre el comando `apt-get`:
```shell
yes | sudo apt-get install {{programa}}
```
{% endraw %}