---
layout: default
title: "git init"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-init">
  <a href="/es/common/git-init.html">git init</a> <a href="#git-init"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inicializa un nuevo repositorio Git local.
> Más información: <https://git-scm.com/docs/git-init>.

#### Inicializa un nuevo repositorio local:
```shell
git init
```
#### Inicializa un repositorio con un nombre especifico para la rama inicial:
```shell
git init --initial-branch={{nombre_de_la_rama}}
```
#### Inicializa un repositorio usando SHA256 como hash del objeto (requiere la versión 2.29+ de Git):
```shell
git init --object-format={{sha256}}
```
#### Inicializa un repositorio vacío, adecuado para usarlo como remoto a través de ssh:
```shell
git init --bare
```
{% endraw %}