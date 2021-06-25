---
layout: default
title: "docker images"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-images">
  <a href="/it/common/docker-images.html">docker images</a> <a href="#docker-images"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestisci immagini Docker.
> Maggiori informazioni: <https://docs.docker.com/engine/reference/commandline/images/>.

#### Elenca tutte le immagini Docker:
```shell
docker images
```
#### Elenca tutte le immagini Docker incluse quelle intermedie:
```shell
docker images -a
```
#### Elenca in modalità silenziosa (solo gli ID numerici):
```shell
docker images -q
```
#### Elenca tutte le immagini Docker che non sono usate da alcun container:
```shell
docker images --filter dangling=true
```
{% endraw %}