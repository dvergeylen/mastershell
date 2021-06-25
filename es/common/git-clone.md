---
layout: default
title: "git clone"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-clone">
  <a href="/es/common/git-clone.html">git clone</a> <a href="#git-clone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clona un repositorio existente.
> Más información: <https://git-scm.com/docs/git-clone>.

#### Clona un repositorio existente:
```shell
git clone {{ubicacion_remota_del_repositorio}}
```
#### Clona un repositorio existente en un directorio específico:
```shell
git clone {{ubicacion_remota_del_repositorio}} {{ruta/al/directorio}}
```
#### Clona un repositorio existente y sus submódulos:
```shell
git clone --recursive {{ubicacion_remota_del_repositorio}}
```
#### Clona un repositorio local:
```shell
git clone -l {{ruta/al/repositorio/local}}
```
#### Clona silenciosamente:
```shell
git clone -q {{ubicacion_remota_del_repositorio}}
```
#### Clona un repositorio existente solo descargando los 10 commits más recientes de la rama por defecto (útil para ahorrar tiempo):
```shell
git clone --depth {{10}} {{ubicacion_remota_del_repositorio}}
```
#### Clona un repositorio existente solo descargando un branch específico:
```shell
git clone --branch {{nombre}} --single-branch {{ubicacion_remota_del_repositorio}}
```
{% endraw %}