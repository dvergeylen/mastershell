---
layout: default
title: "ipcalc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ipcalc">
  <a href="/en/linux/ipcalc.html">ipcalc</a> <a href="#ipcalc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Perform simple operations and calculations on IP addresses and networks.

#### Show information about an address or network with a given subnet mask:
```shell
ipcalc {{1.2.3.4}} {{255.255.255.0}}
```
#### Show information about an address or network in CIDR notation:
```shell
ipcalc {{1.2.3.4}}/{{24}}
```
#### Show the broadcast address of an address or network:
```shell
ipcalc -b {{1.2.3.4}}/{{30}}
```
#### Show the network address of provided IP address and netmask:
```shell
ipcalc -n {{1.2.3.4}}/{{24}}
```
#### Display geographic information about a given IP address:
```shell
ipcalc -g {{1.2.3.4}}
```
{% endraw %}