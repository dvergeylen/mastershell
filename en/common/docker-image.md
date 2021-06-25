---
layout: default
title: "docker image"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-image">
  <a href="/en/common/docker-image.html">docker image</a> <a href="#docker-image"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Docker images.
> See also `docker build`, `docker import`, and `docker pull`.
> More information: <https://docs.docker.com/engine/reference/commandline/image/>.

#### List local Docker images:
```shell
docker image ls
```
#### Delete unused local Docker images:
```shell
docker image prune
```
#### Delete all unused images (not just those without a tag):
```shell
docker image prune --all
```
#### Show the history of a local Docker image:
```shell
docker image history {{image}}
```
{% endraw %}