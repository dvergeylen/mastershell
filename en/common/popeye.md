---
layout: default
title: "popeye"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="popeye">
  <a href="/en/common/popeye.html">popeye</a> <a href="#popeye"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility that reports potential issues with Kubernetes deployment manifests.
> More information: <https://github.com/derailed/popeye>.

#### Scan the current Kubernetes cluster:
```shell
popeye
```
#### Scan a specific namespace:
```shell
popeye -n {{namespace}}
```
#### Scan specific Kubernetes context:
```shell
popeye --context={{context}}
```
#### Use a spinach configuration file for scanning:
```shell
popeye -f {{spinach.yaml}}
```
{% endraw %}