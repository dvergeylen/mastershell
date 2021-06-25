---
layout: default
title: "sysctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sysctl">
  <a href="/en/osx/sysctl.html">sysctl</a> <a href="#sysctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Access kernel state information.

#### Show all available variables and their values:
```shell
sysctl -a
```
#### Show Apple model identifier:
```shell
sysctl -n hw.model
```
#### Show CPU model:
```shell
sysctl -n machdep.cpu.brand_string
```
#### Show available CPU features (MMX, SSE, SSE2, SSE3, AES, etc):
```shell
sysctl -n machdep.cpu.features
```
#### Set a changeable kernel state variable:
```shell
sysctl -w {{section.tunable}}={{value}}
```
{% endraw %}