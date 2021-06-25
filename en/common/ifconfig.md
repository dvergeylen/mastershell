---
layout: default
title: "ifconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ifconfig">
  <a href="/en/common/ifconfig.html">ifconfig</a> <a href="#ifconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Network Interface Configurator.

#### View network settings of an ethernet adapter:
```shell
ifconfig eth0
```
#### Display details of all interfaces, including disabled interfaces:
```shell
ifconfig -a
```
#### Disable eth0 interface:
```shell
ifconfig eth0 down
```
#### Enable eth0 interface:
```shell
ifconfig eth0 up
```
#### Assign IP address to eth0 interface:
```shell
ifconfig eth0 {{ip_address}}
```
{% endraw %}