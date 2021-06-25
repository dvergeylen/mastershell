---
layout: default
title: "git stash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-stash">
  <a href="/es/common/git-stash.html">git stash</a> <a href="#git-stash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Guarda cambios locales de Git en un área temporal.
> Más información: <https://git-scm.com/docs/git-stash>.

#### Guarda cambios actuales, excepto los archivos nuevos (sin rastrear):
```shell
git stash [push -m {{mensaje_opcional_del_guardado}}]
```
#### Guarda cambios actuales, incluyendo los archivos nuevos (sin rastrear):
```shell
git stash -u
```
#### Selecciona interactivamente las partes de archivos cambiados que deben ser guardadas:
```shell
git stash -p
```
#### Muestra todos los guardados (muestra el nombre del guardado, la rama relacionada y el mensaje):
```shell
git stash list
```
#### Aplica un guardado (por defecto aplica el último, llamado stash@{0}):
```shell
git stash apply {{nombre_opcional_del_guardado_o_commit}}
```
#### Aplica un guardado (por defecto es stash@{0} y lo traslada desde la lista de guardado si no causa conflictos:
```shell
git stash pop {{nombre_opcional_del_guardado}}
```
#### Elimina un guardado (por defecto es stash@{0}):
```shell
git stash drop {{nombre_opcional_del_guardado}}
```
#### Elimina todos los guardados:
```shell
git stash clear
```
{% endraw %}