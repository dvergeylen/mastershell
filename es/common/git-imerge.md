---
layout: default
title: "git-imerge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-imerge">
  <a href="/es/common/git-imerge.html">git-imerge</a> <a href="#git-imerge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ejecuta una fusión o rebase entre dos ramas Git incrementalmente.
> Los conflictos entre las ramas se rastrean a pares de commits individuales para simplificar la resolución de conflictos.
> Más información: <https://github.com/mhagger/git-imerge>.

#### Inicia un rebase de tipo imerge (primero comprueba la rama a ser rebasada):
```shell
git imerge rebase {{rama_a_rebasar}}
```
#### Inicia una fusión de tipo imerge (primero comprueba la rama en la que fusionar):
```shell
git imerge merge {{rama_a_fusionar}}
```
#### Muestra una diagrama ASCII para la fusión o rebase en proceso:
```shell
git imerge diagram
```
#### Continua la operación imerge después de resolver los conflictos (primero añade con `git add` los archivos conflictivios):
```shell
git imerge continue --no-edit
```
#### Concluye una operación imerge después de que todos los conflictos se hayan resuelto:
```shell
git imerge finish
```
#### Aborta una operación imerge y vuelve a la rama anterior:
```shell
git-imerge remove && git checkout {{rama_anterior}}
```
{% endraw %}