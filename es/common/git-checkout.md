---
layout: default
title: "git checkout"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-checkout">
  <a href="/es/common/git-checkout.html">git checkout</a> <a href="#git-checkout"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Comprueba una rama o rutas con el arbol de trabajo.
> Más información: <https://git-scm.com/docs/git-checkout>.

#### Crea una nueva rama y cambiarse a esta:
```shell
git checkout -b {{nombre_de_la_rama}}
```
#### Crea una nueva rama a partir de una referencia específica (rama, remoto/rama, las etiquetas son ejemplos de referencias válidas) y cambiarse a esta:
```shell
git checkout -b {{nombre_de_la_rama}} {{referencia}}
```
#### Cambia a una rama local existente:
```shell
git checkout {{nombre_de_la_rama}}
```
#### Cambia a la rama previamente comprobada:
```shell
git checkout -
```
#### Cambia a una rama remota existente:
```shell
git checkout --track {{nombre_remoto}}/{{nombre_de_la_rama}}
```
#### Descarta todos los cambios sin marcar en el directorio actual (véase `git reset` para más comandos para deshacer):
```shell
git checkout .
```
#### Decarta los cambios no marcados de un archivo específico:
```shell
git checkout {{nombre_del_archivo}}
```
#### Sustituir un archivo en el directorio actual con la versión de este en un commit de una rama específica:
```shell
git checkout {{nombre_de_la_rama}} -- {{nombre_del_archivo}}
```
{% endraw %}