---
layout: default
title: "git-grep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-grep">
  <a href="/es/common/git-grep.html">git-grep</a> <a href="#git-grep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encuentra dentro de archivos en cualquier parte del historial del repositorio.
> Acepta una gran cantidad de opciones, de la misma manera que el comando `grep`.
> Más información: <https://git-scm.com/docs/git-grep>.

#### Busca una cadena en los archivos rastreados:
```shell
git grep {{cadena_a_buscar}}
```
#### Busca una cadena en archivos que coincidan con un patrón entre los archivos rastreados:
```shell
git grep {{cadena_a_buscar}} -- {{patrón_de_archivos}}
```
#### Busca una cadena en los archivos rastreados, incluyendo submodulos:
```shell
git grep --recurse-submodules {{cadena_a_buscar}}
```
#### Busca una cadena en un punto específico del historial:
```shell
git grep {{cadena_a_buscar}} {{HEAD~2}}
```
#### Busca una cadena a través de todas las ramas:
```shell
git grep {{cadena_a_buscar}} $(git rev-list --all)
```
{% endraw %}