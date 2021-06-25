---
layout: default
title: "git fetch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-fetch">
  <a href="/es/common/git-fetch.html">git fetch</a> <a href="#git-fetch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Descarga objetos y referencias de un repositorio remoto.
> Más información: <https://git-scm.com/docs/git-fetch>.

#### Recibe los últimos cambios del repositorio remoto upstream por defecto (si se ha establecido):
```shell
git fetch
```
#### Recibe las ramas nuevas de un repositorio remoto upstream específico:
```shell
git fetch {{remote_name}}
```
#### Recibe los últimos cambios de todos los repositorios remotos upstream:
```shell
git fetch --all
```
#### Recibe también las etiquetas de un repositorio upstream:
```shell
git fetch --tags
```
#### Elimina las referencias locales a ramas remotas que han sido eliminadas de upstream:
```shell
git fetch --prune
```
{% endraw %}