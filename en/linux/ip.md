---
layout: default
title: "ip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ip">
  <a href="/en/linux/ip.html">ip</a> <a href="#ip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show / manipulate routing, devices, policy routing and tunnels.
> More information: <https://www.man7.org/linux/man-pages/man8/ip.8.html>.

#### List interfaces with detailed info:
```shell
ip address
```
#### List interfaces with brief network layer info:
```shell
ip -brief address
```
#### List interfaces with brief link layer info:
```shell
ip -brief link
```
#### Display the routing table:
```shell
ip route
```
#### Show neighbors (ARP table):
```shell
ip neighbour
```
#### Make an interface up/down:
```shell
ip link set {{interface}} up/down
```
#### Add/Delete an ip address to an interface:
```shell
ip addr add/del {{ip}}/{{mask}} dev {{interface}}
```
#### Add a default route:
```shell
ip route add default via {{ip}} dev {{interface}}
```
{% endraw %}