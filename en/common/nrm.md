---
layout: default
title: "nrm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nrm">
  <a href="/en/common/nrm.html">nrm</a> <a href="#nrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> NPM registry manager.
> Helps to easily switch between different npm registries.
> More information: <https://github.com/Pana/nrm>.

#### List all registries:
```shell
nrm ls
```
#### Change to a particular registry:
```shell
nrm use {{registry}}
```
#### Show the response time for all registries:
```shell
nrm test
```
#### Add a custom registry:
```shell
nrm add {{registry}} {{url}}
```
#### Delete a registry:
```shell
nrm del {{registry}}
```
{% endraw %}