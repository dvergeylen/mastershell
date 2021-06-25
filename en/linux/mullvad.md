---
layout: default
title: "mullvad"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mullvad">
  <a href="/en/linux/mullvad.html">mullvad</a> <a href="#mullvad"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI client for Mullvad VPN.
> More information: <https://mullvad.net/>.

#### Link your mullvad account with the specified account number:
```shell
mullvad account set {{account_number}}
```
#### Enable LAN access while VPN is on:
```shell
mullvad lan set allow
```
#### Establish the VPN tunnel:
```shell
mullvad connect
```
#### Check status of VPN tunnel:
```shell
mullvad status
```
{% endraw %}