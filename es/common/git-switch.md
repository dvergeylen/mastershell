---
layout: default
title: "git switch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-switch">
  <a href="/es/common/git-switch.html">git switch</a> <a href="#git-switch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alterna entre ramas Git. Requiere una versión 2.23+ de Git.
> Véase también `git checkout`.
> Más información: <https://git-scm.com/docs/git-switch>.

#### Cambia a una rama existente:
```shell
git switch {{nombre_de_la_rama}}
```
#### Crea una nueva rama y se cambia a esta:
```shell
git switch --create {{nombre_de_la_rama}}
```
#### Crea una nueva rama basada en un commit específico y se cambia a esta:
```shell
git switch --create {{nombre_de_la_rama}} {{commit}}
```
#### Cambia a la rama anterior:
```shell
git switch -
```
#### Cambia a una rama y actualiza todos los submódulos para coincidir:
```shell
git switch --recurse-submodules {{nombre_de_la_rama}}
```
#### Cambia a una rama y automáticamente fusiona la rama actual y cualquier cambio sin commit en ella:
```shell
git switch --merge {{nombre_de_la_rama}}
```
{% endraw %}