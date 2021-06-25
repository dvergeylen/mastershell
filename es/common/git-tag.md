---
layout: default
title: "git tag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-tag">
  <a href="/es/common/git-tag.html">git tag</a> <a href="#git-tag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea, muestra, borra o verifica etiquetas.
> Una etiqueta es una referencia estática a un commit específico.
> Más información: <https://git-scm.com/docs/git-tag>.

#### Muestra todas las etiquetas:
```shell
git tag
```
#### Crea una etiqueta con el nombre especificado a partir del commit actual:
```shell
git tag {{nombre_de_la_etiqueta}}
```
#### Crea una etiqueta con el nombre especificado a partir del commit señalado:
```shell
git tag {{nombre_de_la_etiqueta}} {{commit}}
```
#### Crea una etiqueta anotada con el mensaje especificado:
```shell
git tag {{nombre_de_la_etiqueta}} -m {{mensaje_de_la_etiqueta}}
```
#### Elimina la etiqueta con el nombre especificado:
```shell
git tag -d {{nombre_de_la_etiqueta}}
```
#### Obtiene las etiquetas actualizadas de upstreams:
```shell
git fetch --tags
```
#### Muestra todas las etiquetas cuyos ancestros incluyan un commit específico:
```shell
git tag --contains {{commit}}
```
{% endraw %}