---
layout: default
title: "ip address"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ip-address">
  <a href="/de/linux/ip-address.html">ip address</a> <a href="#ip-address"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> IP Adressen Management Unterbefehl.

#### Zeige Netzwerk-Interfaces mit ihren Adressen:
```shell
ip address
```
#### Zeige nur die aktiven Netzwerk-Interfaces:
```shell
ip address show up
```
#### Zeige Informationen über ein bestimmtes Interface:
```shell
ip address show dev {{eth0}}
```
#### Füge eine Adresse zu einem Interface hinzu:
```shell
ip address add {{ip_adresse}} dev {{eth0}}
```
#### Entferne eine Adresse von einem Interface:
```shell
ip address delete {{ip_adresse}} dev {{eth0}}
```
#### Entfernt alle IP Adressen in einem speziellen Bereich von einem Interface:
```shell
ip address flush dev {{eth0}} scope {{global|host|link}}
```
{% endraw %}