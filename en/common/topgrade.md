---
layout: default
title: "topgrade"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="topgrade">
  <a href="/en/common/topgrade.html">topgrade</a> <a href="#topgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Update all applications on the system.
> More information: <https://github.com/r-darwish/topgrade>.

#### Run updates:
```shell
topgrade
```
#### Say yes to all updates:
```shell
topgrade -y
```
#### Cleanup temporary/old files:
```shell
topgrade -c
```
#### Disable a certain update operation:
```shell
topgrade -disable {{operation}}
```
#### Only perform a certain update operation:
```shell
topgrade --only {{operation}}
```
#### Edit the config file with default editor:
```shell
topgrade --edit-config
```
{% endraw %}