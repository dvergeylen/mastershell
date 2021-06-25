---
layout: default
title: "kubens"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kubens">
  <a href="/en/common/kubens.html">kubens</a> <a href="#kubens"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to switch between Kubernetes namespaces.
> More information: <https://github.com/ahmetb/kubectx>.

#### List the namespaces:
```shell
kubens
```
#### Change the active namespace:
```shell
kubens {{name}}
```
#### Switch to the previous namespace:
```shell
kubens -
```
{% endraw %}