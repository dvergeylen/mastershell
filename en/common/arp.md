---
layout: default
title: "arp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arp">
  <a href="/en/common/arp.html">arp</a> <a href="#arp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show and manipulate your system's ARP cache.
> More information: <https://manned.org/arp>.

#### Show the current ARP table:
```shell
arp -a
```
#### Clear the entire cache:
```shell
sudo arp -a -d
```
#### Delete a specific entry:
```shell
arp -d {{address}}
```
#### Create an entry in the ARP table:
```shell
arp -s {{address}} {{mac_address}}
```
{% endraw %}