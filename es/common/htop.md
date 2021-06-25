---
layout: default
title: "htop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="htop">
  <a href="/es/common/htop.html">htop</a> <a href="#htop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra información dinámica en tiempo real sobre los procesos ejecutándose. Una versión mejorada de `top`.

#### Inicia htop:
```shell
htop
```
#### Inicia htop mostrando solo procesos pertenecientes a un usuario dado:
```shell
htop -u {{usuario}}
```
#### Ordena procesos por columna (use `--sort-key help` para ver una lista de columnas):
```shell
htop -s {{nombre_columna}}
```
#### Recibe ayuda sobre comandos interactivos:
```shell
?
```
{% endraw %}