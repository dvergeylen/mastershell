---
layout: default
title: "docker run"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-run">
  <a href="/en/common/docker-run.html">docker run</a> <a href="#docker-run"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a command in a new Docker container.
> More information: <https://docs.docker.com/engine/reference/commandline/run/>.

#### Run command in a new container from a tagged image:
```shell
docker run {{image:tag}} {{command}}
```
#### Run command in a new container in background and display its ID:
```shell
docker run -d {{image}} {{command}}
```
#### Run command in a one-off container in interactive mode and pseudo-TTY:
```shell
docker run --rm -it {{image}} {{command}}
```
#### Run command in a new container with passed environment variables:
```shell
docker run -e '{{variable}}={{value}}' -e {{variable}} {{image}} {{command}}
```
#### Run command in a new container with bind mounted volumes:
```shell
docker run -v {{path/to/host_path}}:{{path/to/container_path}} {{image}} {{command}}
```
#### Run command in a new container with published ports:
```shell
docker run -p {{host_port}}:{{container_port}} {{image}} {{command}}
```
{% endraw %}