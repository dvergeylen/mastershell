---
layout: default
title: "git pull"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-pull">
  <a href="/es/common/git-pull.html">git pull</a> <a href="#git-pull"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Obtener rama de un repositorio remoto y fusionarlo con el repositorio local.
> Más información: <https://git-scm.com/docs/git-pull>.

#### Descargar cambios del repositorio remoto por defecto y fusionarlo:
```shell
git pull
```
#### Descargar cambios del repositorio remoto por defecto y usar avance rápido (*fast forward*):
```shell
git pull --rebase
```
#### Descargar cambios de un repositorio remoto y una rama específica para fusionarlos en HEAD:
```shell
git pull {{nombre_remoto}} {{rama}}
```
{% endraw %}