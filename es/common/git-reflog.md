---
layout: default
title: "git reflog"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-reflog">
  <a href="/es/common/git-reflog.html">git reflog</a> <a href="#git-reflog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra un registro de cambios de las referencias (*reflog*) locales como HEAD, ramas o etiquetas.
> Más información: <https://git-scm.com/docs/git-reflog>.

#### Muestra un registro de referencias para HEAD:
```shell
git reflog
```
#### Muestra el registro de referencias para una rama:
```shell
git reflog {{nombre_de_la_rama}}
```
#### Muestra solo las últimas 5 entradas en el registro de referencias:
```shell
git reflog -n {{5}}
```
{% endraw %}