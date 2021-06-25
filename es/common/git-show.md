---
layout: default
title: "git show"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-show">
  <a href="/es/common/git-show.html">git show</a> <a href="#git-show"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra varios tipos de objetos Git (commits, etiquetas, etcétera).
> Más información: <https://git-scm.com/docs/git-show>.

#### Muestra información sobre el último commit (hash, mensaje, cambios y otros metadatos):
```shell
git show
```
#### Muestra información de un commit específico:
```shell
git show {{commit}}
```
#### Muestra información del commit asociado a una determinada etiqueta:
```shell
git show {{etiqueta}}
```
#### Muestra información del tercer commit desde la punta de una rama:
```shell
git show {{rama}}~{{3}}
```
#### Muestra el mensaje de un commit en una única línea, eliminando el resultado de la diferencia:
```shell
git show --oneline -s {{commit}}
```
#### Muestra solo estadísticas (caracteres agregados o removidos) de los archivos modificados:
```shell
git show --stat {{commit}}
```
#### Muestra solo la lista de archivos agregados, renombrados o eliminados:
```shell
git show --summary {{commit}}
```
#### Muestra el contenido de una archivo en una revisión específica (por ej., una rama, una etiqueta o un commit):
```shell
git show {{revisión}}:{{ruta/al/archivo}}
```
{% endraw %}