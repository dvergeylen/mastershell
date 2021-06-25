---
layout: default
title: "git status"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-status">
  <a href="/es/common/git-status.html">git status</a> <a href="#git-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra los cambios realizados en los archivos del repositorio Git.
> Lista los archivos cambiados, añadidos y eliminados comparándolos con el último commit.
> Más información: <https://git-scm.com/docs/git-status>.

#### Muestra los archivos cambiados que aún no han sido añadidos a un commit:
```shell
git status
```
#### Muestra la salida en formato breve:
```shell
git status -s
```
#### No muestra los archivos sin rastrear en la salida:
```shell
git status --untracked-files=no
```
#### Muestra la salida en formato breve junto a la información del branch:
```shell
git status --short --branch
```
{% endraw %}