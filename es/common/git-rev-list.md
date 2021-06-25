---
layout: default
title: "git rev-list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rev-list">
  <a href="/es/common/git-rev-list.html">git rev-list</a> <a href="#git-rev-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra las revisiones (commits) en orden cronológico inverso.
> Más información: <https://git-scm.com/docs/git-rev-list>.

#### Muestra todos los commits de la rama actual:
```shell
git rev-list {{HEAD}}
```
#### Muestra los commits más recientes a partir de una fecha y una rama específica:
```shell
git rev-list --since={{'2019-12-01 00:00:00'}} {{nombre_de_rama}}
```
#### Muestra todos los commits fusionados en un commit específico:
```shell
git rev-list --merges {{commit}}
```
{% endraw %}