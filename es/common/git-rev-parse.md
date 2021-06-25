---
layout: default
title: "git rev-parse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rev-parse">
  <a href="/es/common/git-rev-parse.html">git rev-parse</a> <a href="#git-rev-parse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra metados relativos a revisiones específicas.
> Más información: <https://git-scm.com/docs/git-rev-parse>.

#### Obtiene el hash del commit de una rama:
```shell
git rev-parse {{nombre_de_la_rama}}
```
#### Obtiene el nombre de la rama actual:
```shell
git rev-parse --abbrev-ref {{HEAD}}
```
#### Obtiene la ruta absoluta al directorio raíz:
```shell
git rev-parse --show-toplevel
```
{% endraw %}