---
layout: default
title: "git reset"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-reset">
  <a href="/es/common/git-reset.html">git reset</a> <a href="#git-reset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Deshace commits o desmarca cambios mediante el reseteo del actual HEAD de Git al estado especificado.
> Si se pasa una ruta, funciona como "desmarcar", si se pasa el hash de un commit o una rama, funciona como "deshacer" el commit.
> Más información: <https://git-scm.com/docs/git-reset>.

#### Desmarcar todo:
```shell
git reset
```
#### Desmarcar un archivo o archivos específicos:
```shell
git reset {{ruta/al/archivo_o_archivos}}
```
#### Interactivamente desmarca partes de un archivo:
```shell
git reset --patch {{ruta/al/archivo}}
```
#### Deshace el último commit, manteniendo sus cambios,y cualquier otro cambios sin commit,en el sistema de archivo:
```shell
git reset HEAD~
```
#### Deshace los últimos dos commits al añadir sus cambios al índice (por ej., marcado para commit):
```shell
git reset --soft HEAD~2
```
#### Descartar cualquier cambio sin commit, marcado o no (se puede `git checkout` solo para los cambios sin marcar):
```shell
git reset --hard
```
#### Resetea el repositorio a un commit específico y descarta a partir de este los cambios con y sin commit, y los marcados:
```shell
git reset --hard {{commit}}
```
{% endraw %}