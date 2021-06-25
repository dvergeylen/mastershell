---
layout: default
title: "docker container"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-container">
  <a href="/en/common/docker-container.html">docker container</a> <a href="#docker-container"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Docker containers.
> More information: <https://docs.docker.com/engine/reference/commandline/container/>.

#### List currently running Docker containers:
```shell
docker container ls
```
#### Start one or more stopped containers:
```shell
docker container start {{container1_name}} {{container2_name}}
```
#### Kill one or more running containers:
```shell
docker container kill {{container_name}}
```
#### Stop one or more running containers:
```shell
docker container stop {{container_name}}
```
#### Pause all processes within one or more containers:
```shell
docker container pause {{container_name}}
```
#### Display detailed information on one or more containers:
```shell
docker container inspect {{container_name}}
```
#### Export a container's filesystem as a tar archive:
```shell
docker container export {{container_name}}
```
#### Create a new image from a container's changes:
```shell
docker container commit {{container_name}}
```
{% endraw %}