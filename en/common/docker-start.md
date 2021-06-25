---
layout: default
title: "docker start"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-start">
  <a href="/en/common/docker-start.html">docker start</a> <a href="#docker-start"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Start one or more stopped containers.
> More information: <https://docs.docker.com/engine/reference/commandline/start/>.

#### Show help:
```shell
docker start
```
#### Start a docker container:
```shell
docker start {{container}}
```
#### Start a container, attaching stdout and stderr and forwarding signals:
```shell
docker start --attach {{container}}
```
#### Start one or more space-separated containers:
```shell
docker start {{container(s)}}
```
{% endraw %}