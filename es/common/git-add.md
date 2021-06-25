---
layout: default
title: "git add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-add">
  <a href="/es/common/git-add.html">git add</a> <a href="#git-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Añade los archivos cambiados al índice.
> Más información: <https://git-scm.com/docs/git-add>.

#### Añade un archivo al índice:
```shell
git add {{ruta/al/archivo}}
```
#### Añade todos los archivos (rastreados o no rastreados):
```shell
git add -A
```
#### Añade los archivos ya rastreados:
```shell
git add -u
```
#### Añade también los archivos ignorados:
```shell
git add -f
```
#### Añade partes de archivos interactivamente:
```shell
git add -p
```
#### Añade partes de un archivo dado interactivamente:
```shell
git add -p {{ruta/al/archivo}}
```
#### Añade un archivo interactivamente:
```shell
git add -i
```
{% endraw %}