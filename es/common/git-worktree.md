---
layout: default
title: "git worktree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-worktree">
  <a href="/es/common/git-worktree.html">git worktree</a> <a href="#git-worktree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestiona múltiples árboles de trabajo adjuntos al mismo repositorio.
> Más información: <https://git-scm.com/docs/git-worktree>.

#### Crea un nuevo directorio con la rama específicada y se cambia él:
```shell
git worktree add {{ruta/al/directorio}} {{rama}}
```
#### Crea un nuevo directorio con un nueva rama y se cambia a él:
```shell
git worktree add {{ruta/al/directorio}} -b {{rama_nueva}}
```
#### Muestra todos los directorios de trabajo adjuntos a este repositorio:
```shell
git worktree list
```
#### Elimina un árbol de trabajo (después de eliminar el directorio del árbol de trabajo):
```shell
git worktree prune
```
{% endraw %}