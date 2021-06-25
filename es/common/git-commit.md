---
layout: default
title: "git commit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-commit">
  <a href="/es/common/git-commit.html">git commit</a> <a href="#git-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Realiza commits de los archivos al repositorio.
> Más información: <https://git-scm.com/docs/git-commit>.

#### Realiza un commit de los archivos marcados al repositorio con un mensaje:
```shell
git commit -m "{{mensaje}}"
```
#### Realiza un commit de los archivos marcados con un mensaje leído desde un archivo:
```shell
git commit --file {{ruta/al/archivo_del_mensaje_del_commit}}
```
#### Marca automáticamente todos los archivos modificados y realiza un commit con un mensaje:
```shell
git commit -a -m "{{mensaje}}"
```
#### Sustituye el último commit con los cambios marcados actualmente, cambiando el hash del commit:
```shell
git commit --amend
```
#### Realiza un commit para archivos específicos (marcados previamente):
```shell
git commit {{ruta/al/archivo1}} {{ruta/al/archivo2}}
```
{% endraw %}