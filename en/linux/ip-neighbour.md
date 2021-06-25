---
layout: default
title: "ip-neighbour"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ip-neighbour">
  <a href="/en/linux/ip-neighbour.html">ip-neighbour</a> <a href="#ip-neighbour"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Neighbour/ARP tables management IP subcommand.
> More information: <https://manned.org/ip-neighbour.8>.

#### Display the neighbour/ARP table entries:
```shell
ip neighbour
```
#### Remove entries in the neighbour table on device `eth0`:
```shell
sudo ip neighbour flush dev {{eth0}}
```
#### Perform a neighbour lookup and return a neighbour entry:
```shell
ip neighbour get {{lookup_ip}} dev {{eth0}}
```
#### Add or delete an ARP entry for the neighbour IP address to `eth0`:
```shell
sudo ip neighbour {{add|del}} {{ip_address}} lladdr {{mac_address}} dev {{eth0}} nud reachable
```
#### Change or replace an ARP entry for the neighbour IP address to `eth0`:
```shell
sudo ip neighbour {{change|replace}} {{ip_address}} lladdr {{new_mac_address}} dev {{eth0}}
```
{% endraw %}