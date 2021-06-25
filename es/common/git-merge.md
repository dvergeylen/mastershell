---
layout: default
title: "git merge"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-merge">
  <a href="/es/common/git-merge.html">git merge</a> <a href="#git-merge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fusiona ramas.
> Más información: <https://git-scm.com/docs/git-merge>.

#### Fusiona una rama con la rama actual:
```shell
git merge {{nombre_de_la_rama}}
```
#### Edita el mensaje de fusión:
```shell
git merge -e {{nombre_de_la_rama}}
```
#### Fusiona una rama y crea un commit para la fusión:
```shell
git merge --no-ff {{nombre_de_la_rama}}
```
#### Cancela una fusión en caso de conflictos:
```shell
git merge --abort
```
{% endraw %}