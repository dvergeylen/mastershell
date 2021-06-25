---
layout: default
title: "git shortlog"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-shortlog">
  <a href="/es/common/git-shortlog.html">git shortlog</a> <a href="#git-shortlog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Resume la salida de `git log`.
> Más información: <https://git-scm.com/docs/git-shortlog>.

#### Muestra un resumen de todos los commits realizados, agrupados alfabéticamente por autor:
```shell
git shortlog
```
#### Muestra un resumen de todos los commits realizados, agrupados por el número de commits realizados:
```shell
git shortlog -n
```
#### Muestra un resumen de todos los commits realizados, agrupados por la identidad de quien realiza el commit (usuario y correo electrónico):
```shell
git shortlog -c
```
#### Muestra un resumen de los últimos 5 commits (i. e., un rango de revisiones específico):
```shell
git shortlog HEAD~{{5}}..HEAD
```
#### Muestra todos los usuarios, correos electrónicos y número de commits en la rama actual:
```shell
git shortlog -sne
```
#### Muestra todos los usuarios, correos electrónicos y número de commits en todas las ramas:
```shell
git shortlog -sne --all
```
{% endraw %}