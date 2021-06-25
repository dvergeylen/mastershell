---
layout: default
title: "paci"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="paci">
  <a href="/en/common/paci.html">paci</a> <a href="#paci"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A package manager for bash scripts.

#### Update the list of available packages and versions (it's recommended to run this before other `paci` commands):
```shell
paci refresh
```
#### Configure its behaviour:
```shell
paci configure
```
#### Search for a given package:
```shell
paci search {{package}}
```
#### Install a package:
```shell
paci install {{package}}
```
#### Update a package:
```shell
paci update {{package}}
```
{% endraw %}