---
layout: default
title: "wol"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wol">
  <a href="/en/linux/wol.html">wol</a> <a href="#wol"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Client for sending Wake-on-LAN magic packets.
> More information: <https://sourceforge.net/projects/wake-on-lan/>.

#### Send a WoL packet to a device:
```shell
wol {{mac_address}}
```
#### Send a WoL packet to a device in another subnet based on its IP:
```shell
wol --ipaddr={{ip_address}} {{mac_address}}
```
#### Send a WoL packet to a device in another subnet based on its hostname:
```shell
wol --host={{hostname}} {{mac_address}}
```
#### Send a WoL packet to a specific port on a host:
```shell
wol --port={{port_number}} {{mac_address}}
```
#### Read hardware addresses, IP addresses/hostnames, optional ports and SecureON passwords from a file:
```shell
wol --file={{path/to/file}}
```
#### Turn on verbose output:
```shell
wol --verbose {{mac_address}}
```
{% endraw %}