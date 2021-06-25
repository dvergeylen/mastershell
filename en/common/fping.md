---
layout: default
title: "fping"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fping">
  <a href="/en/common/fping.html">fping</a> <a href="#fping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A more powerful ping which can ping multiple hosts.
> More information: <https://fping.org>.

#### List alive hosts within a subnet generated from a netmask:
```shell
fping -a -g 192.168.1.0/24
```
#### List alive hosts within a subnet generated from an IP range:
```shell
fping -a -g 192.168.1.1 192.168.1.254
```
#### List unreachable hosts within a subnet generated from a netmask:
```shell
fping -u -g 192.168.1.0/24
```
{% endraw %}