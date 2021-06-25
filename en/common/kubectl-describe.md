---
layout: default
title: "kubectl describe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kubectl-describe">
  <a href="/en/common/kubectl-describe.html">kubectl describe</a> <a href="#kubectl-describe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show details of Kubernetes objects and resources.
> More information: <https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands#describe>.

#### Show details of pods in a namespace:
```shell
kubectl describe pods -n {{namespace}}
```
#### Show details of nodes in a namespace:
```shell
kubectl describe nodes -n {{namespace}}
```
#### Show the details of a specific pod in a namespace:
```shell
kubectl describe pods {{pod_name}} -n {{namespace}}
```
#### Show the details of a specific node in a namespace:
```shell
kubectl describe nodes {{node_name}} -n {{namespace}}
```
#### Show details of Kubernetes objects defined in a YAML manifest:
```shell
kubectl describe -f {{path/to/manifest}}.yaml
```
{% endraw %}