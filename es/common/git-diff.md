---
layout: default
title: "git diff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-diff">
  <a href="/es/common/git-diff.html">git diff</a> <a href="#git-diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra los cambios de los archivos rastreados.
> Más información: <https://git-scm.com/docs/git-diff>.

#### Muestra los cambios sin marcar ni commit:
```shell
git diff
```
#### Muestra todos los cambios sin commit, pero incluye los marcados:
```shell
git diff HEAD
```
#### Muestra solo los cambios marcados pero que no tienen commit:
```shell
git diff --staged
```
#### Muestra los cambios de todos los commits a partir de una fecha/tiempo específico (una expresión de fecha, por ej., "1 week 2 days" o una fecha ISO):
```shell
git diff 'HEAD@{3 months|weeks|days|hours|seconds ago}
```
#### Muestra solo los nombres de los archivos cambiados con un commit específico:
```shell
git diff --name-only {{commit}}
```
#### Muestra un resumen de la creación, renombre y modos de cambio con un commit específico:
```shell
git diff --summary {{commit}}
```
#### Compara un único archivo entre dos ramas o commits:
```shell
git diff {{rama_1}}..{{rama_2}} [--] {{ruta/al/archivo}}
```
#### Compara diferentes archivos de la rama actual con otra rama:
```shell
git diff {{rama}}:{{ruta/al/archivo}} {{ruta/al/archivo2}}
```
{% endraw %}