---
layout: default
title: "docker-build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-build">
  <a href="/fr/common/docker-build.html">docker-build</a> <a href="#docker-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Construit une image à partir d'un Dockerfile.
> Plus d'informations : <https://docs.docker.com/engine/reference/commandline/build/>.

#### Construire une image Docker en utilisant le Dockerfile du répertoire courant :
```shell
docker build .
```
#### Construire une image Docker à partir d'un Dockerfile situé à une URL précisée :
```shell
docker build {{github.com/creack/docker-firefox}}
```
#### Construire une image Docker et l'étiquette :
```shell
docker build --tag {{nom:etiquette}} .
```
#### Ne pas utiliser le cache lors de la construction de l'image :
```shell
docker build --no-cache --tag {{nom:etiquette}} .
```
#### Construire une image Docker utilisant un Dockerfile spécifique :
```shell
docker build --file {{Dockerfile}} .
```
#### Construire avec des variables personnalisées définies à la volée :
```shell
docker build --build-arg {{HTTP_PROXY=http://10.20.30.2:1234}} --build-arg {{FTP_PROXY=http://40.50.60.5:4567}} .
```
{% endraw %}