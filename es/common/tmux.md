---
layout: default
title: "tmux"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tmux">
  <a href="/es/common/tmux.html">tmux</a> <a href="#tmux"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multiplexa varias consolas virtuales.
> Más información: <https://github.com/tmux/tmux>.

#### Inicia una nueva sesión de tmux:
```shell
tmux
```
#### Inicia una nueva sesión de tmux y le asigna un nombre:
```shell
tmux new -s {{nombre}}
```
#### Muestra las sesiones:
```shell
tmux ls
```
#### Adjunta a una sesión:
```shell
tmux a
```
#### Adjunta a una sesión con un nombre específico:
```shell
tmux a -t {{nombre}}
```
#### Desconecta de la sesión:
```shell
Ctrl + B, D
```
#### Elimina una sesión con un nombre específico:
```shell
tmux kill-session -t {{nombre}}
```
#### Elimina una sesión cuando se adjunta:
```shell
Ctrl + B, x (luego se pulsa 'y' para confirmar que sí)
```
{% endraw %}