---
layout: default
title: "git restore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-restore">
  <a href="/es/common/git-restore.html">git restore</a> <a href="#git-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restaura los archivos del árbol de trabajo. Requiere la version 2.23+ de Git.
> Véase también `git checkout` y `git reset`.
> Más información: <https://git-scm.com/docs/git-restore>.

#### Restaura un archivo sin marcar a la versión del commit actual (HEAD):
```shell
git restore {{ruta/al/archivo}}
```
#### Restaura un archivo sin marcar a la versión de un commit específico:
```shell
git restore --source {{commit}} {{ruta/al/archivo}}
```
#### Descarta los cambios sin commit para los archivos rastreados:
```shell
git restore :/
```
#### Desmarca un archivo:
```shell
git restore --staged {{ruta/al/archivo}}
```
#### Desmarca todos los archivos:
```shell
git restore --staged :/
```
#### Descarta todos los cambios de los archivos, marcados o no:
```shell
git restore --worktree --staged :/
```
#### Selecciona interactivamente secciones de archivos para restaurar:
```shell
git restore --patch
```
{% endraw %}