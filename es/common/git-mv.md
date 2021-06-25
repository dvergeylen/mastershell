---
layout: default
title: "git mv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-mv">
  <a href="/es/common/git-mv.html">git mv</a> <a href="#git-mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mueve o renombra archivos y actualiza el índice Git.
> Más información: <https://git-scm.com/docs/git-mv>.

#### Mueve el archivo dentro del repositorio y añade el movimiento al siguiente commit:
```shell
git mv {{ruta/al/archivo}} {{nueva/ruta/al/archivo}}
```
#### Renombra un archivo y añade el renombre al siguiente commit:
```shell
git mv {{nombre_de_archivo}} {{nuevo_nombre_de_archivo}}
```
#### Sobrescribir el archivo en la ruta objetivo si existe:
```shell
git mv --force {{archivo}} {{objetivo}}
```
{% endraw %}