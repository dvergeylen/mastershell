---
layout: default
title: "docker image"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-image">
  <a href="/it/common/docker-image.html">docker image</a> <a href="#docker-image"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisci immagini Docker.
> Vedi anche `docker build`, `docker import` e `docker pull`.
> Maggiori informazioni: <https://docs.docker.com/engine/reference/commandline/image/>.

#### Elenca tutte le immagini Docker locali:
```shell
docker image ls
```
#### Elimina le immagini Docker locali inutilizzate:
```shell
docker image prune
```
#### Cancella tutte le immagini inutilizzate (non solo quelle sprovviste di tag):
```shell
docker image prune --all
```
#### Mostra la cronologia di un'immagine Docker locale:
```shell
docker image history {{immagine}}
```
{% endraw %}