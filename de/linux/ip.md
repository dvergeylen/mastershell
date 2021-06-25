---
layout: default
title: "ip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ip">
  <a href="/de/linux/ip.html">ip</a> <a href="#ip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige und manipuliere routing, Geräte, Policy routing und Tunnel.

#### Zeige Interfaces mit detaillierten Informationen:
```shell
ip address
```
#### Zeige Interfaces mit kurzen Netzwerkinformationen:
```shell
ip -brief address
```
#### Zeige Interfaces mit kurzen link layer Informationen:
```shell
ip -brief link
```
#### Zeige die Routing Tabelle:
```shell
ip route
```
#### Zeige Nachbarn (ARP Tabelle):
```shell
ip neighbour
```
#### Schaltee ein bestimmten Interface ein oder aus:
```shell
ip link set {{interface}} {{up|down}}
```
#### Entferne oder füge eine IP zu einem Interface hinzu:
```shell
ip addr add/del {{ip}}/{{mask}} dev {{interface}}
```
#### Füge eine Standard Route hinzu:
```shell
ip route add default via {{ip}} dev {{interface}}
```
{% endraw %}