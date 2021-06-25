---
layout: default
title: "git submodule"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-submodule">
  <a href="/es/common/git-submodule.html">git submodule</a> <a href="#git-submodule"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inspecciona, actualiza y gestiona los submódulos.
> Más información: <https://git-scm.com/docs/git-submodule>.

#### Instala los submódulos específicos de un repositorio:
```shell
git submodule update --init --recursive
```
#### Añade un repositorio como un submódulo:
```shell
git submodule add {{url_del_repositorio}}
```
#### Añade un repositorio Git como submulo en un directorio específico:
```shell
git submodule add {{url_del_repositorio}} {{ruta/al/directorio}}
```
#### Actualiza cada submódulo a su último commit:
```shell
git submodule foreach git pull
```
{% endraw %}