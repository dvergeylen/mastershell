---
layout: default
title: "kind"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kind">
  <a href="/en/common/kind.html">kind</a> <a href="#kind"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for running local Kubernetes clusters using Docker container "nodes".
> Designed for testing Kubernetes itself, but may be used for local development or continuous integration.
> More information: <https://github.com/kubernetes-sigs/kind>.

#### Create a local Kubernetes cluster:
```shell
kind create cluster --name {{cluster_name}}
```
#### Delete one or more clusters:
```shell
kind delete clusters {{cluster_name}}
```
#### Get details about clusters, nodes, or the kubeconfig:
```shell
kind get {{clusters|nodes|kubeconfig}}
```
#### Export the kubeconfig or the logs:
```shell
kind export {{kubeconfig|logs}}
```
{% endraw %}