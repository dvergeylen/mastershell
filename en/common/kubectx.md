---
layout: default
title: "kubectx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kubectx">
  <a href="/en/common/kubectx.html">kubectx</a> <a href="#kubectx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to manage and switch between `kubectl` contexts.
> More information: <https://github.com/ahmetb/kubectx>.

#### List the contexts:
```shell
kubectx
```
#### Switch to a named context:
```shell
kubectx {{name}}
```
#### Switch to the previous context:
```shell
kubectx -
```
#### Delete a named context:
```shell
kubectx -d {{name}}
```
{% endraw %}