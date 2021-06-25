---
layout: default
title: "docker-compose"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-compose">
  <a href="/en/common/docker-compose.html">docker-compose</a> <a href="#docker-compose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run and manage multi container docker applications.
> More information: <https://docs.docker.com/compose/reference/overview/>.

#### List all running containers:
```shell
docker-compose ps
```
#### Create and start all containers in the background using a `docker-compose.yml` file from the current directory:
```shell
docker-compose up -d
```
#### Start all containers, rebuild if necessary:
```shell
docker-compose up --build
```
#### Start all containers using an alternate compose file:
```shell
docker-compose --file {{path/to/file}} up
```
#### Stop all running containers:
```shell
docker-compose stop
```
#### Stop and remove all containers, networks, images, and volumes:
```shell
docker-compose down --rmi all --volumes
```
#### Follow logs for all containers:
```shell
docker-compose logs --follow
```
#### Follow logs for a specific container:
```shell
docker-compose logs --follow {{container_name}}
```
{% endraw %}