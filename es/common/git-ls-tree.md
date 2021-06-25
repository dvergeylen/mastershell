---
layout: default
title: "git ls-tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-ls-tree">
  <a href="/es/common/git-ls-tree.html">git ls-tree</a> <a href="#git-ls-tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra los contenidos de un objeto árbol.
> Más información: <https://git-scm.com/docs/git-ls-tree>.

#### Muestra el contenido del árbol en una rama:
```shell
git ls-tree {{nombre_de_la_rama}}
```
#### Muestra el contenido del árbol en un commit (recursivo en subárboles):
```shell
git ls-tree -r {{hash_del_commit}}
```
#### Muestra solo los nombres de archivos del árbol en un commit:
```shell
git ls-tree --name-only {{hash_del_commit}}
```
{% endraw %}