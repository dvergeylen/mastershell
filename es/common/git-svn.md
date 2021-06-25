---
layout: default
title: "git svn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-svn">
  <a href="/es/common/git-svn.html">git svn</a> <a href="#git-svn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Operacion bidreccional entre un repositorio Subversión y otro Git.
> Más información: <https://git-scm.com/docs/git-svn>.

#### Clona un repositorio SVN:
```shell
git svn clone {{https://ejemplo.com/repositorio_subversion}} {{directorio_local}}
```
#### Clona un repositorio SVN a partir un número de revisión específico:
```shell
git svn clone -r{{1234}}:HEAD {{https://svn.ejemplo.net/subversion/repo}} {{directorio_local}}
```
#### Actualiza el clon local apartir del repositorio SVN:
```shell
git svn rebase
```
#### Obtiene las actualización del repositorio SVN remoto sin cambiar el HEAD de Git:
```shell
git svn fetch
```
#### Realiza un commit al repositorio SVN:
```shell
git svn dcommit
```
{% endraw %}