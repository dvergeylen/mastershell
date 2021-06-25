---
layout: default
title: "git config"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-config">
  <a href="/es/common/git-config.html">git config</a> <a href="#git-config"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestiona opciones personalizadas para la configuración de repositorios Git.
> Estas configuraciones pueden ser locales (para el repositorio actual) o globales (para el usuario actual).
> Más información: <https://git-scm.com/docs/git-config>.

#### Muestra solo las entradas de la configuración local (almacenadas en `.git/config` en el repositorio actual):
```shell
git config --list --local
```
#### Muestra solo las entradas de la configuración global (almacenadas en `~/.gitconfig`):
```shell
git config --list --global
```
#### Muestra todas las entradas de configuración que han sido definidas local o globalmente:
```shell
git config --list
```
#### Muestra el valor de una entrada específica de la configuración:
```shell
git config alias.unstage
```
#### Establece el valor global para una entrada específica de la configuración:
```shell
git config --global alias.unstage "reset HEAD --"
```
#### Revierte una entrada de la configuración global a su valor por defecto:
```shell
git config --global --unset alias.unstage
```
#### Edita la configuración de Git para el repositorio actual en el editor por defecto:
```shell
git config --edit
```
#### Edita la configuración global de Git en el editor por defecto:
```shell
git config --global --edit
```
{% endraw %}