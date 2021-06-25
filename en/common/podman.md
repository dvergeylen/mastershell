---
layout: default
title: "podman"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="podman">
  <a href="/en/common/podman.html">podman</a> <a href="#podman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple management tool for pods, containers and images.
> Podman provides a Docker-CLI comparable command-line. Simply put: `alias docker=podman`.
> More information: <https://github.com/containers/libpod/blob/master/commands.md>.

#### Print out information about containers:
```shell
podman ps
```
#### List all containers (both running and stopped):
```shell
podman ps --all
```
#### Start one or more containers:
```shell
podman start {{container_name}} {{container_id}}
```
#### Stop one or more running containers:
```shell
podman stop {{container_name}} {{container_id}}
```
#### Pull an image from a registry (defaults to the Docker Hub):
```shell
podman pull {{image_name}}:{{image_tag}}
```
#### Open a shell inside of an already running container:
```shell
podman exec --interactive --tty {{container_name}} {{sh}}
```
#### Remove one or more stopped containers:
```shell
podman rm {{container_name}} {{container_id}}
```
#### Display the logs of one or more containers and follow log output:
```shell
podman logs --follow {{container_name}} {{container_id}}
```
{% endraw %}