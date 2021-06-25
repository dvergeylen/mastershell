---
layout: default
title: "docker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker">
  <a href="/es/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administra contenedores e imágenes de Docker.
> Más información: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Lista los contenedores de Docker en ejecución:
```shell
docker ps
```
#### Lista todos los contenedores de Docker (en ejecución y detenidos):
```shell
docker ps -a
```
#### Inicia un contenedor desde una imagen con un nombre personalizado:
```shell
docker run --name {{nombre_de_contenedor}} {{imagen}}
```
#### Inicia o detiene un contenedor existente:
```shell
docker {{start|stop}} {{nombre_de_contenedor}}
```
#### Descarga una imagen desde un registro de Docker:
```shell
docker pull {{imagen}}
```
#### Inicia una línea de Comandos dentro de un contenedor en ejecución:
```shell
docker exec -it {{nombre_de_contenedor}} {{sh}}
```
#### Elimina un contenedor detenido:
```shell
docker rm {{nombre_de_contenedor}}
```
#### Obtiene y sigue los registros de un contenedor:
```shell
docker logs -f {{nombre_de_contenedor}}
```
{% endraw %}