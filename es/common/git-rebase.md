---
layout: default
title: "git rebase"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-rebase">
  <a href="/es/common/git-rebase.html">git rebase</a> <a href="#git-rebase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vuelve a aplicar commits de una rama en lo más alto de otra rama.
> Se utiliza comúnmente para "mover" una rama entera a otra base, ya que crea copias de los commits en una nueva ubicación.
> Más información: <https://git-scm.com/docs/git-rebase>.

#### Reorganiza la rama actual en lo más alto de otra rama:
```shell
git rebase {{rama_de_reorganización}}
```
#### Inicia un rebase interactivo que permite reordenar los commits, omitirlos, combinarlos o modificarlos:
```shell
git rebase -i {{rama_base_objetivo_o_hash_del_commit}}
```
#### Continúa un rebase que fue interrumpido por una fusión fallida después de editar los archivos con conflictos:
```shell
git rebase --continue
```
#### Continúa un rebase que fue pausado para fusionar conflictos saltando el commit conflictivo:
```shell
git rebase --skip
```
#### Cancela un rebase en proceso (por ej., si es interrumpido por un conflicto de fusión):
```shell
git rebase --abort
```
#### Mueve parte de la rama actual a una nueva base proporcionando la base antigua para empezar:
```shell
git rebase --onto {{base_nueva}} {{base_antigua}}
```
#### Reaplica los últimos 5 commits en su lugar, evita que puedan ser reordenados, omitidos, combinados o modificados:
```shell
git rebase -i {{HEAD~5}}
```
#### Resuelve automáticamente cualquier conflicto favoreciendo la versión de la rama en la que se esta trabajando (en este caso la palabra `theirs` tiene un significado invertido):
```shell
git rebase -X theirs {{rama_de_reorganización}}
```
{% endraw %}