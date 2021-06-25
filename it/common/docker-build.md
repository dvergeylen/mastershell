---
layout: default
title: "docker build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-build">
  <a href="/it/common/docker-build.html">docker build</a> <a href="#docker-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea un'immagine a partire da un Dockerfile. La creazione di un'immagine docker è chiamata build.
> Maggiori informazioni: <https://docs.docker.com/engine/reference/commandline/build/>.

#### Crea un'immagine docker usando il Dockerfile nella directory corrente:
```shell
docker build .
```
#### Crea un'immagine docker usando il Dockerfile disponibile a un dato URL:
```shell
docker build {{github.com/creack/docker-firefox}}
```
#### Crea e tagga un'immagine docker:
```shell
docker build --tag {{nome:tag}} .
```
#### Non usare la cache per la creazione di un'immagine docker:
```shell
docker build --no-cache --tag {{nome:tag}} .
```
#### Crea un'immagine docker usando un dato Dockerfile:
```shell
docker build --file {{Dockerfile}} .
```
#### Crea un'immagine docker usando variabili fornite in fase di build:
```shell
docker build --build-arg {{HTTP_PROXY=http://10.20.30.2:1234}} --build-arg {{FTP_PROXY=http://40.50.60.5:4567}} .
```
{% endraw %}