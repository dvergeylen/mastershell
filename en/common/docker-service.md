---
layout: default
title: "docker service"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-service">
  <a href="/en/common/docker-service.html">docker service</a> <a href="#docker-service"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the services on a docker daemon.
> More information: <https://docs.docker.com/engine/reference/commandline/service/>.

#### List the services on a docker daemon:
```shell
docker service ls
```
#### Create a new service:
```shell
docker service create --name {{service_name}} {{image}}:{{tag}}
```
#### Display detailed information of a space-separated list of services:
```shell
docker service inspect {{service_name|ID}}
```
#### List the tasks of a space-separated list of services:
```shell
docker service ps {{service_name|ID}}
```
#### Scale to a specific number of replicas for a space-separated list of services:
```shell
docker service scale {{service_name}}={{count_of_replicas}}
```
#### Remove a space-separated list of services:
```shell
docker service rm {{service_name|ID}}
```
{% endraw %}