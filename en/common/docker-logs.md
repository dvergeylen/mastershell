---
layout: default
title: "docker logs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-logs">
  <a href="/en/common/docker-logs.html">docker logs</a> <a href="#docker-logs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print container logs.
> More information: <https://docs.docker.com/engine/reference/commandline/logs>.

#### Print logs from a container:
```shell
docker logs {{container_name}}
```
#### Print logs and follow them:
```shell
docker logs -f {{container_name}}
```
#### Print last 5 lines:
```shell
docker logs {{container_name}} --tail {{5}}
```
#### Print logs and append them with timestamps:
```shell
docker logs -t {{container_name}}
```
#### Print logs from a certain point in time of container execution (i.e. 23m, 10s, 2013-01-02T13:23:37):
```shell
docker logs {{container_name}} --until {{time}}
```
{% endraw %}