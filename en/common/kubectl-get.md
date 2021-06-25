---
layout: default
title: "kubectl get"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kubectl-get">
  <a href="/en/common/kubectl-get.html">kubectl get</a> <a href="#kubectl-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get Kubernetes objects and resources.
> More information: <https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands#get>.

#### Get all namespaces in the current cluster:
```shell
kubectl get namespaces
```
#### Get nodes in a specified namespace:
```shell
kubectl get nodes -n {{namespace}}
```
#### Get pods in a specified namespace:
```shell
kubectl get pods -n {{namespace}}
```
#### Get deployments in a specified namespace:
```shell
kubectl get deployments -n {{namespace}}
```
#### Get services in a specified namespace:
```shell
kubectl get services -n {{namespace}}
```
#### Get Kubernetes objects defined in a YAML manifest:
```shell
kubectl get -f {{path/to/manifest}}.yaml
```
{% endraw %}