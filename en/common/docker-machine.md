---
layout: default
title: "docker-machine"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-machine">
  <a href="/en/common/docker-machine.html">docker-machine</a> <a href="#docker-machine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and manage machines running Docker.
> More information: <https://docs.docker.com/machine/reference/>.

#### List currently running docker machines:
```shell
docker-machine ls
```
#### Create a new docker machine with specific name:
```shell
docker-machine create {{name}}
```
#### Get the status of a machine:
```shell
docker-machine status {{name}}
```
#### Start a machine:
```shell
docker-machine start {{name}}
```
#### Stop a machine:
```shell
docker-machine stop {{name}}
```
#### Inspect information about a machine:
```shell
docker-machine inspect {{name}}
```
{% endraw %}