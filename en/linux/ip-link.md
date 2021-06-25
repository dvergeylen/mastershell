---
layout: default
title: "ip link"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ip-link">
  <a href="/en/linux/ip-link.html">ip link</a> <a href="#ip-link"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage network interfaces.
> More information: <https://man7.org/linux/man-pages/man8/ip-link.8.html>.

#### Show information about all network interfaces:
```shell
ip link
```
#### Show information about a specific network interface:
```shell
ip link show {{ethN}}
```
#### Bring a network interface up or down:
```shell
ip link set {{ethN}} {{up|down}}
```
#### Give a meaningful name to a network interface:
```shell
ip link set {{ethN}} alias "{{LAN Interface}}"
```
#### Change the MAC address of a network interface:
```shell
ip link set {{ethN}} address {{ff:ff:ff:ff:ff:ff}}
```
#### Change the MTU size for a network interface to use jumbo frames:
```shell
ip link set {{ethN}} mtu {{9000}}
```
{% endraw %}