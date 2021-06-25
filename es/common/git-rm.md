---
layout: default
title: "git rm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rm">
  <a href="/es/common/git-rm.html">git rm</a> <a href="#git-rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elimina archivos del índice del repositorio y del sistema de archivos local.
> Más información: <https://git-scm.com/docs/git-rm>.

#### Elimina un archivo del índice de un repositorio y del sistema de archivos local:
```shell
git rm {{archivo}}
```
#### Elimina un directorio:
```shell
git rm -r {{directorio}}
```
#### Elimina un archivo del índice del repositorio, pero mantiene intacto el archivo local:
```shell
git rm --cached {{archivo}}
```
{% endraw %}