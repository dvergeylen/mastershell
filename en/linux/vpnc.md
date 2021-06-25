---
layout: default
title: "vpnc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vpnc">
  <a href="/en/linux/vpnc.html">vpnc</a> <a href="#vpnc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A VPN client for the Cisco 3000 VPN Concentrator.

#### Connect with a defined configuration file:
```shell
sudo vpnc {{config_file}}
```
#### Terminate the previously created connection:
```shell
sudo vpnc-disconnect
```
{% endraw %}