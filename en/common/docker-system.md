---
layout: default
title: "docker system"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-system">
  <a href="/en/common/docker-system.html">docker system</a> <a href="#docker-system"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Docker data and display system-wide information.
> More information: <https://docs.docker.com/engine/reference/commandline/system/>.

#### Show help:
```shell
docker system
```
#### Show docker disk usage:
```shell
docker system df
```
#### Show detailed information on disk usage:
```shell
docker system df --verbose
```
#### Remove unused data:
```shell
docker system prune
```
#### Remove unused data created more than a specified amount of time in the past:
```shell
docker system prune --filter="until={{hours}}h{{minutes}}m"
```
#### Display real-time events from the Docker daemon:
```shell
docker system events
```
#### Display real-time events from containers streamed as valid JSON Lines:
```shell
docker system events --filter 'type=container' --format '{{json .}}'
```
#### Display system-wide information:
```shell
docker system info
```
{% endraw %}