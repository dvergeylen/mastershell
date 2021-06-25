---
layout: default
title: "dhclient"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dhclient">
  <a href="/en/common/dhclient.html">dhclient</a> <a href="#dhclient"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> DHCP client.
> More information: <https://manned.org/dhclient>.

#### Get an IP address for the `eth0` interface:
```shell
sudo dhclient {{eth0}}
```
#### Release an IP address for the `eth0` interface:
```shell
sudo dhclient -r {{eth0}}
```
{% endraw %}