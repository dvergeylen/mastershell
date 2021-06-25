---
layout: default
title: "git revert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-revert">
  <a href="/es/common/git-revert.html">git revert</a> <a href="#git-revert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea nuevos commits que revierten el efecton de los anteriores.
> Más información: <https://git-scm.com/docs/git-revert>.

#### Revierte el commit más reciente:
```shell
git revert {{@}}
```
#### Revierte el quinto último commit:
```shell
git revert HEAD~{{4}}
```
#### Revierte múltiples commits:
```shell
git revert {{rama~5..rama~2}}
```
#### No crea nuevos commits, solo cambia el árbol de trabajo:
```shell
git revert -n {{0c01a9..9a1743}}
```
{% endraw %}