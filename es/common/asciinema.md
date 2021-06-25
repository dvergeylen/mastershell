---
layout: default
title: "asciinema"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asciinema">
  <a href="/es/common/asciinema.html">asciinema</a> <a href="#asciinema"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Graba y reproduce sesiones de terminal, y opcionalmente compartelas en asciinema.org.
> Más información: <https://asciinema.org/>.

#### Asocia el programa local de `asciinema` con una cuenta de asciinema.org:
```shell
asciinema auth
```
#### Crea una nueva grabación (una vez acabada, se pregutará al usuario si la quiere cuardar en local, o subirla):
```shell
asciinema rec
```
#### Crea una nueva grabación y la guarda en un archivo local:
```shell
asciinema rec {{ruta/hacia/archivo}}.cast
```
#### Reproduce una grabación desde un archivo local:
```shell
asciinema play {{ruta/hacia/archivo}}.cast
```
#### Reproduce una grabación desde asciinema.org:
```shell
asciinema play https://asciinema.org/a/{{cast_id}}
```
#### Crea una nueva grabación, limitando el tiempo de espera máximo a 2.5 segundos:
```shell
asciinema rec -i {{2.5}}
```
#### Imprime la salida completa de un archivo local de grabación:
```shell
asciinema cat {{ruta/hacia/archivo}}.cast
```
#### Sube un archivo local de grabación a asciinema.org:
```shell
asciinema upload {{ruta/hacia/archivo}}.cast
```
{% endraw %}