---
layout: default
title: "docker rmi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-rmi">
  <a href="/en/common/docker-rmi.html">docker rmi</a> <a href="#docker-rmi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove one or more Docker images.
> More information: <https://docs.docker.com/engine/reference/commandline/rmi/>.

#### Show help:
```shell
docker rmi
```
#### Remove one or more images given their names:
```shell
docker rmi {{image1 image2 ...}}
```
#### Force remove an image:
```shell
docker rmi --force {{image}}
```
#### Remove an image without deleting untagged parents:
```shell
docker rmi --no-prune {{image}}
```
{% endraw %}