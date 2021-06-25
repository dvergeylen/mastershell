---
layout: default
title: "ipconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ipconfig">
  <a href="/en/windows/ipconfig.html">ipconfig</a> <a href="#ipconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display and manage the network configuration of Windows.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/ipconfig>.

#### Show a list of network adapters:
```shell
ipconfig
```
#### Show a detailed list of network adapters:
```shell
ipconfig /all
```
#### Renew the IP addresses for a network adapter:
```shell
ipconfig /renew {{adapter}}
```
#### Free up the IP addresses for a network adapter:
```shell
ipconfig /release {{adapter}}
```
#### Remove all data from the DNS cache:
```shell
ipconfig /flushdns
```
{% endraw %}