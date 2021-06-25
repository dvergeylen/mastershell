---
layout: default
title: "git gc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-gc">
  <a href="/es/common/git-gc.html">git gc</a> <a href="#git-gc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Optimiza el repositorio local eliminando archivos innecesarios.
> Más información: <https://git-scm.com/docs/git-gc>.

#### Optimiza el repositorio:
```shell
git gc
```
#### Optimiza agresivamente (tarda más):
```shell
git gc --aggressive
```
#### No elimina objetos sueltos (por defecto los elimina):
```shell
git gc --no-prune
```
#### Suprime toda la salida:
```shell
git gc --quiet
```
#### Muestra todas sus funcionalidades:
```shell
git gc --help
```
{% endraw %}