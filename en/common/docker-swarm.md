---
layout: default
title: "docker swarm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="docker-swarm">
  <a href="/en/common/docker-swarm.html">docker swarm</a> <a href="#docker-swarm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A container orchestration tool.
> More information: <https://docs.docker.com/engine/swarm/>.

#### Initialize a swarm cluster:
```shell
docker swarm init
```
#### Display the token to join a manager or a worker:
```shell
docker swarm join-token {{worker|manager}}
```
#### Join a new node to the cluster:
```shell
docker swarm join --token {{token}} {{manager_node_url:2377}}
```
#### Remove a worker from the swarm (run inside the worker node):
```shell
docker swarm leave
```
#### Display the current CA certificate in PEM format:
```shell
docker swarm ca
```
#### Rotate the current CA certificate and display the new certificate:
```shell
docker swarm ca --rotate
```
#### Change the valid period for node certificates:
```shell
docker swarm update --cert-expiry {{hours}}h{{minutes}}m{{seconds}}s
```
{% endraw %}