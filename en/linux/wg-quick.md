---
layout: default
title: "wg-quick"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wg-quick">
  <a href="/en/linux/wg-quick.html">wg-quick</a> <a href="#wg-quick"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Quickly set up WireGuard tunnels based on config files.
> More information: <https://www.wireguard.com/quickstart/>.

#### Set up a VPN tunnel:
```shell
wg-quick up {{interface_name}}
```
#### Delete a VPN tunnel:
```shell
wg-quick down {{interface_name}}
```
{% endraw %}