---
layout: default
title: "lspci"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lspci">
  <a href="/en/linux/lspci.html">lspci</a> <a href="#lspci"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List all PCI devices.

#### Show a brief list of devices:
```shell
lspci
```
#### Display additional info:
```shell
lspci -v
```
#### Display drivers and modules handling each device:
```shell
lspci -k
```
#### Show a specific device:
```shell
lspci -s {{00:18.3}}
```
#### Dump info in a readable form:
```shell
lspci -vm
```
{% endraw %}