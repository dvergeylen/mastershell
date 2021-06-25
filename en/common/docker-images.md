---
layout: default
title: "docker images"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-images">
  <a href="/en/common/docker-images.html">docker images</a> <a href="#docker-images"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Docker images.
> More information: <https://docs.docker.com/engine/reference/commandline/images/>.

#### List all Docker images:
```shell
docker images
```
#### List all Docker images including intermediates:
```shell
docker images --all
```
#### List the output in quiet mode (only numeric IDs):
```shell
docker images --quiet
```
#### List all Docker images not used by any container:
```shell
docker images --filter dangling=true
```
#### List images that contain a substring in their name:
```shell
docker images "{{*name*}}"
```
{% endraw %}