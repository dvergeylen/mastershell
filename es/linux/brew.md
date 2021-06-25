---
layout: default
title: "brew"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew">
  <a href="/es/linux/brew.html">brew</a> <a href="#brew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestor de paquetes Homebrew para Linux.

#### Busca fórmulas disponibles:
```shell
brew search {{texto}}
```
#### Instala la última versión de una fórmula (usar `--devel` para la versión de desarrollo):
```shell
brew install {{formula}}
```
#### Lista todas las fórmulas instaladas:
```shell
brew list
```
#### Actualizar una fórmula instalada (si no se indica ninguna, todas las fórmulas son actualizadas):
```shell
brew upgrade {{formula}}
```
#### Actualiza a la última versión de Linuxbrew y de todas las fórmulas desde GitHub:
```shell
brew update
```
#### Mostrar las fórmulas que tienen una versión más reciente disponible:
```shell
brew outdated
```
#### Mostrar la información de una fórmula (versión, ruta de instalación, dependencias, etc.):
```shell
brew info {{fórmula}}
```
#### Revisar la instalación local de Linuxbrew en busca de problemas potenciales:
```shell
brew doctor
```
{% endraw %}