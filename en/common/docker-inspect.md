---
layout: default
title: "docker inspect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-inspect">
  <a href="/en/common/docker-inspect.html">docker inspect</a> <a href="#docker-inspect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Return low-level information on Docker objects.
> More information: <https://docs.docker.com/engine/reference/commandline/inspect/>.

#### Show help:
```shell
docker inspect
```
#### Display information about a container, image, or volume using a name or ID:
```shell
docker inspect {{container|image|ID}}
```
#### Display a container's IP address:
```shell
docker inspect --format='{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' {{container}}
```
#### Display the path to the container's log file:
```shell
docker inspect --format='{{.LogPath}}' {{container}}
```
#### Display the image name of the container:
```shell
docker inspect --format='{{.Config.Image}}' {{container}}
```
#### Display the configuration information as JSON:
```shell
docker inspect --format='{{json .Config}}' {{container}}
```
#### Display all port bindings:
```shell
docker inspect --format='{{range $p, $conf := .NetworkSettings.Ports}} {{$p}} -> {{(index $conf 0).HostPort}} {{end}}' {{container}}
```
{% endraw %}