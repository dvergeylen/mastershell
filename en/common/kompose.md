---
layout: default
title: "kompose"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kompose">
  <a href="/en/common/kompose.html">kompose</a> <a href="#kompose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to convert docker-compose applications to Kubernetes.
> More information: <https://github.com/kubernetes/kompose>.

#### Deploy a dockerized application to Kubernetes:
```shell
kompose up -f {{docker-compose.yml}}
```
#### Delete instantiated services/deployments from Kubernetes:
```shell
kompose down -f {{docker-compose.yml}}
```
#### Convert a docker-compose file into Kubernetes resources file:
```shell
kompose convert -f {{docker-compose.yml}}
```
{% endraw %}