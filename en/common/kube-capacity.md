---
layout: default
title: "kube-capacity"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kube-capacity">
  <a href="/en/common/kube-capacity.html">kube-capacity</a> <a href="#kube-capacity"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple CLI that provides an overview of the resource requests, limits, and utilization in a Kubernetes cluster.
> Combine the best parts of `kubectl top` and `kubectl describe` into a CLI focused on cluster resources.
> More information: <https://github.com/robscott/kube-capacity>.

#### Output a list of nodes with the total CPU and Memory resource requests and limits:
```shell
kube-capacity
```
#### Include pods:
```shell
kube-capacity -p
```
#### Include utilization:
```shell
kube-capacity -u
```
{% endraw %}