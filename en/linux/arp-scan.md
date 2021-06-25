---
layout: default
title: "arp-scan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arp-scan">
  <a href="/en/linux/arp-scan.html">arp-scan</a> <a href="#arp-scan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send ARP packets to hosts (specified as IP addresses or hostnames) to scan the local network.

#### Scan the current local network:
```shell
arp-scan --localnet
```
#### Scan an IP network with a custom bitmask:
```shell
arp-scan {{192.168.1.1}}/{{24}}
```
#### Scan an IP network within a custom range:
```shell
arp-scan {{127.0.0.0}}-{{127.0.0.31}}
```
#### Scan an IP network with a custom net mask:
```shell
arp-scan {{10.0.0.0}}:{{255.255.255.0}}
```
{% endraw %}