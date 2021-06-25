---
layout: default
title: "arping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arping">
  <a href="/en/common/arping.html">arping</a> <a href="#arping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Discover and probe hosts in a network using the ARP protocol.
> Useful for MAC address discovery.
> More information: <https://github.com/ThomasHabets/arping>.

#### Ping a host by ARP request packets:
```shell
arping {{host_ip}}
```
#### Ping a host on a specific interface:
```shell
arping -I {{interface}} {{host_ip}}
```
#### Ping a host and stop at the first reply:
```shell
arping -f {{host_ip}}
```
#### Ping a host a specific number of times:
```shell
arping -c {{count}} {{host_ip}}
```
#### Broadcast ARP request packets to update neighbours' ARP caches:
```shell
arping -U {{ip_to_broadcast}}
```
#### Detect duplicated IP addresses in the network by sending ARP requests with a 3 seconds timeout:
```shell
arping -D -w {{3}} {{ip_to_check}}
```
{% endraw %}