---
layout: default
title: "git clean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-clean">
  <a href="/es/common/git-clean.html">git clean</a> <a href="#git-clean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elimina archivos sin rastrear del árbol de trabajo.
> Más información: <https://git-scm.com/docs/git-clean>.

#### Elimina archivos que no son rastreados por Git:
```shell
git clean
```
#### Elimina interactivamente archivos que no son rastreados por Git:
```shell
git clean -i
```
#### Muestra que archivos serían borrados sin llegar a borrarlos:
```shell
git clean --dry-run
```
#### Elimina forzosamente los archivos que no son rastreados por Git:
```shell
git clean -f
```
#### Elimina forzosamente los directorios que no son rastreados por Git:
```shell
git clean -fd
```
#### Elimina archivos sin rastrear, incluyendo los archivos ignorados en `.gitignore` y los excluidos en `.git/info/exclude`:
```shell
git clean -x
```
{% endraw %}