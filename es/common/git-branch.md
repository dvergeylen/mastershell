---
layout: default
title: "git branch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-branch">
  <a href="/es/common/git-branch.html">git branch</a> <a href="#git-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Comando Git principal para trabajar con ramas.
> Más información: <https://git-scm.com/docs/git-branch>.

#### Muestra las ramas locales. La rama actual está resaltada por `*`:
```shell
git branch
```
#### Muestra todas las ramas (locales y remotas):
```shell
git branch -a
```
#### Muestra el nombre de la rama actual:
```shell
git branch --show-current
```
#### Crea una nueva rama basada en el commit actual:
```shell
git branch {{nombre_de_la_rama}}
```
#### Crea una nueva rama basada en un commit específico:
```shell
git branch {{nombre_de_rama}} {{hash_del_commit}}
```
#### Renombra una rama (no debe haber sido fusionada para hacer esto):
```shell
git branch -m {{antiguo_nombre_de_la_rama}} {{nuevo_nombre_de_la_rama}}
```
#### Borra una rama local (no debe haber sido fusionada para hacer esto):
```shell
git branch -d {{nombre_de_la_rama}}
```
#### Borra una rama remota:
```shell
git push {{nombre_remoto}} --delete {{nombre_de_la_rama_remota}}
```
{% endraw %}