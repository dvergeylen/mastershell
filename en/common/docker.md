---
layout: default
title: "docker"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker">
  <a href="/en/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Docker containers and images.
> More information: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### List currently running docker containers:
```shell
docker ps
```
#### List all docker containers (running and stopped):
```shell
docker ps -a
```
#### Start a container from an image, with a custom name:
```shell
docker run --name {{container_name}} {{image}}
```
#### Start or stop an existing container:
```shell
docker {{start|stop}} {{container_name}}
```
#### Pull an image from a docker registry:
```shell
docker pull {{image}}
```
#### Open a shell inside of an already running container:
```shell
docker exec -it {{container_name}} {{sh}}
```
#### Remove a stopped container:
```shell
docker rm {{container_name}}
```
#### Fetch and follow the logs of a container:
```shell
docker logs -f {{container_name}}
```
{% endraw %}