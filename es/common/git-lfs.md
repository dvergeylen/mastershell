---
layout: default
title: "git lfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-lfs">
  <a href="/es/common/git-lfs.html">git lfs</a> <a href="#git-lfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Trabaja con archivos grandes en repositorios de Git.
> Más información: <https://git-lfs.github.com>.

#### Inicializa Git LFS:
```shell
git lfs install
```
#### Rastrea archivos que coinciden con un patrón:
```shell
git lfs track '{{*.bin}}'
```
#### Cambia la URL a la que apunta Git LFS (útil si el servidor LFS está separado del servidor Git):
```shell
git config -f .lfsconfig lfs.url {{url_del_punto_de_acceso_LFS}}
```
#### Muestra los patrones rastreados:
```shell
git lfs track
```
#### Muestra los archivos que han sido añadidos con un commit:
```shell
git lfs ls-files
```
#### Introduce todos los objetos LFS en el servidor remoto (útil si se encuentran errores):
```shell
git lfs push --all {{nombre_remoto}} {{nombre_de_la_rama}}
```
#### Trae todos los objetos de Git LFS:
```shell
git lfs fetch
```
#### Verifica todos los objetos de Git LFS:
```shell
git lfs checkout
```
{% endraw %}