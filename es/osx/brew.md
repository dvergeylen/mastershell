---
layout: default
title: "brew"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew">
  <a href="/es/osx/brew.html">brew</a> <a href="#brew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administrador de paquetes para macOS.
> Más información: <https://brew.sh>.

#### Busca fórmulas y paquetes disponibles:
```shell
brew search {{text}}
```
#### Instala la última versión estable de una fórmula (usa `--devel` para versiones de desarrollo):
```shell
brew install {{formula}}
```
#### Muestra todas las fórmulas instaladas:
```shell
brew list
```
#### Muestra fórmulas instaladas que no dependen de otras:
```shell
brew leaves
```
#### Actualiza una fórmula instalada (si no se indica el nombre, se actualizan todas las fórmulas):
```shell
brew upgrade {{formula}}
```
#### Actualiza a la última versión de Homebrew y todas sus fórmulas desde GitHub:
```shell
brew update
```
#### Muestra información acerca de una fórmula (versión, ruta de instalación, dependencias, etc.):
```shell
brew info {{formula}}
```
#### Verifica la instalación local de Homebrew en busca de problemas potenciales:
```shell
brew doctor
```
{% endraw %}