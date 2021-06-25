---
layout: default
title: "k8s-unused-secret-detector"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="k8s-unused-secret-detector">
  <a href="/en/common/k8s-unused-secret-detector.html">k8s-unused-secret-detector</a> <a href="#k8s-unused-secret-detector"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface tool for detecting unused Kubernetes secrets.
> More information: <https://github.com/dtan4/k8s-unused-secret-detector>.

#### Detect unused secrets:
```shell
k8s-unused-secret-detector
```
#### Detect unused secrets in a specific namespace:
```shell
k8s-unused-secret-detector -n {{namespace}}
```
#### Delete unused secrets in a specific namespace:
```shell
k8s-unused-secret-detector -n {{namespace}} | kubectl delete secret -n {{namespace}}
```
{% endraw %}