---
layout: default
title: "stern"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stern">
  <a href="/en/common/stern.html">stern</a> <a href="#stern"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tail multiple pods and containers from Kubernetes.
> More information: <https://github.com/wercker/stern/>.

#### Tail all pods within a current namespace:
```shell
stern .
```
#### Tail all pods with a specific status:
```shell
stern . --container-state {{running|waiting|terminated}}
```
#### Tail all pods that matches a given regular expression:
```shell
stern {{pod_query}}
```
#### Tail matched pods from all namespaces:
```shell
stern {{pod_query}} --all-namespaces
```
#### Tail matched pods from 15 minutes ago:
```shell
stern {{pod_query}} --since {{15m}}
```
#### Tail matched pods with a specific label:
```shell
stern {{pod_query}} --selector {{release=canary}}
```
{% endraw %}