---
layout: default
title: "git remote"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-remote">
  <a href="/es/common/git-remote.html">git remote</a> <a href="#git-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestiona el conjunto de repositorios rastreados ("remotos").
> Más información: <https://git-scm.com/docs/git-remote>.

#### Muestra una lista de los remotos existentes, sus nombres y URL:
```shell
git remote -v
```
#### Muestra información de un remoto:
```shell
git remote show {{nombre_remoto}}
```
#### Añade un remoto:
```shell
git remote add {{nombre_remoto}} {{url_remoto}}
```
#### Cambiar la URL de un remoto (utiliza `--add` para mantener la URL existente):
```shell
git remote set-url {{nombre_remoto}} {{nueva_url}}
```
#### Elimina un remoto:
```shell
git remote remove {{nombre_remoto}}
```
#### Renombra un remoto:
```shell
git remote rename {{nombre_antiguo}} {{nombre_nuevo}}
```
{% endraw %}