---
layout: default
title: "docker network"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-network">
  <a href="/en/common/docker-network.html">docker network</a> <a href="#docker-network"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and manage docker networks.
> More information: <https://docs.docker.com/engine/reference/commandline/network/>.

#### List all available and configured networks on docker daemon:
```shell
docker network ls
```
#### Create a user defined network:
```shell
docker network create --driver {{driver_name}} {{network_name}}
```
#### Display detailed information of a space-separated list of networks:
```shell
docker network inspect {{network_name}}
```
#### Connect a container to a network using a name or ID:
```shell
docker network connect {{network_name}} {{container_name|ID}}
```
#### Disconnect a container from a network:
```shell
docker network disconnect {{network_name}} {{container_name|ID}}
```
#### Remove all unused (not referenced by any container) networks:
```shell
docker network prune
```
#### Remove a space-separated list of unused networks:
```shell
docker network rm {{network_name}}
```
{% endraw %}