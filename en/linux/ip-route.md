---
layout: default
title: "ip route"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ip-route">
  <a href="/en/linux/ip-route.html">ip route</a> <a href="#ip-route"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> IP Routing table management subcommand.
> More information: <https://manned.org/ip-route>.

#### Display the routing table:
```shell
ip route {{show|list}}
```
#### Add a default route using gateway forwarding:
```shell
sudo ip route add default via {{gateway_ip}}
```
#### Add a default route using `eth0`:
```shell
sudo ip route add default dev {{eth0}}
```
#### Add a static route:
```shell
sudo ip route add {{destination_ip}} via {{gateway_ip}} dev {{eth0}}
```
#### Delete a static route:
```shell
sudo ip route del {{destination_ip}} dev {{eth0}}
```
#### Change or replace a static route:
```shell
sudo ip route {{change|replace}} {{destination_ip}} via {{gateway_ip}} dev {{eth0}}
```
#### Show which route will be used by the kernel to reach an IP address:
```shell
ip route get {{destination_ip}}
```
{% endraw %}