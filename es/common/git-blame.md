---
layout: default
title: "git blame"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-blame">
  <a href="/es/common/git-blame.html">git blame</a> <a href="#git-blame"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra el hash del commit y el último autor de cada línea de un archivo.
> Más información: <https://git-scm.com/docs/git-blame>.

#### Muestra el archivo con el nombre del autor y el hash del commit en cada línea:
```shell
git blame {{archivo}}
```
#### Muestra el archivo con correo electrónico del autor y hash del commit en cada línea:
```shell
git blame -e {{archivo}}
```
{% endraw %}