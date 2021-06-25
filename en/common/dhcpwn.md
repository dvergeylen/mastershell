---
layout: default
title: "dhcpwn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dhcpwn">
  <a href="/en/common/dhcpwn.html">dhcpwn</a> <a href="#dhcpwn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Test DHCP IP exhaustion attacks and sniff local DHCP traffic.
> More information: <https://github.com/mschwager/dhcpwn>.

#### Flood the network with IP requests:
```shell
dhcpwn --interface {{network_interface}} flood --count {{number_of_requests}}
```
#### Sniff local DHCP traffic:
```shell
dhcpwn --interface {{network_interface}} sniff
```
{% endraw %}