---
layout: default
title: "docker-compose"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-compose">
  <a href="/es/common/docker-compose.html">docker-compose</a> <a href="#docker-compose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ejecuta y gestiona múltiples contenedores Docker.
> Más información: <https://docs.docker.com/compose/reference/overview/>.

#### Lista los contenedores en ejecución:
```shell
docker-compose ps
```
#### Crea e inicia todos los contenedores en segundo plano usando el archivo `docker-compose.yml` en el directorio actual:
```shell
docker-compose up -d
```
#### Inicia todos los contenedores y reconstruye si es ncesario:
```shell
docker-compose up --build
```
#### Inicia todos los contenedores usando un archivo compose alternativo:
```shell
docker-compose --file {{ruta/al/directorio}} up
```
#### Detiene todos los contenedores en ejecución:
```shell
docker-compose stop
```
#### Detiene y elimina todos los contenedores, redes, imágenes y volúmenes:
```shell
docker-compose down --rmi all --volumes
```
#### Sigue los registros de todos los contenedores:
```shell
docker-compose logs --follow
```
{% endraw %}