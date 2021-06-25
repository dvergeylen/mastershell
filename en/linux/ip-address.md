---
layout: default
title: "ip address"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ip-address">
  <a href="/en/linux/ip-address.html">ip address</a> <a href="#ip-address"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> IP Address management subcommand.

#### List network interfaces and their associated IP addresses:
```shell
ip address
```
#### Filter to show only active network interfaces:
```shell
ip address show up
```
#### Display information about a specific network interface:
```shell
ip address show dev {{eth0}}
```
#### Add an IP address to a network interface:
```shell
ip address add {{ip_address}} dev {{eth0}}
```
#### Remove an IP address from a network interface:
```shell
ip address delete {{ip_address}} dev {{eth0}}
```
#### Delete all IP addresses in a given scope from a network interface:
```shell
ip address flush dev {{eth0}} scope {{global|host|link}}
```
{% endraw %}