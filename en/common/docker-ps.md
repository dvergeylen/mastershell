---
layout: default
title: "docker ps"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-ps">
  <a href="/en/common/docker-ps.html">docker ps</a> <a href="#docker-ps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List Docker containers.
> More information: <https://docs.docker.com/engine/reference/commandline/ps/>.

#### List currently running docker containers:
```shell
docker ps
```
#### List all docker containers (running and stopped):
```shell
docker ps --all
```
#### Show the latest created container (includes all states):
```shell
docker ps --latest
```
#### Filter containers that contain a substring in their name:
```shell
docker ps --filter="name={{name}}"
```
#### Filter containers that share a given image as an ancestor:
```shell
docker ps --filter "ancestor={{image}}:{{tag}}"
```
#### Filter containers by exit status code:
```shell
docker ps --all --filter="exited={{code}}"
```
#### Filter containers by status (created, running, removing, paused, exited and dead):
```shell
docker ps --filter="status={{status}}"
```
#### Filter containers that mount a specific volume or have a volume mounted in a specific path:
```shell
docker ps --filter="volume={{path/to/directory}}" --format "table {{.ID}}\t{{.Image}}\t{{.Names}}\t{{.Mounts}}"
```
{% endraw %}