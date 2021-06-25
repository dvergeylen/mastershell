---
layout: default
title: "openvpn3"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openvpn3">
  <a href="/en/linux/openvpn3.html">openvpn3</a> <a href="#openvpn3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OpenVPN 3 Linux client.
> More information: <https://community.openvpn.net/openvpn/wiki/OpenVPN3Linux>.

#### Start a new VPN session:
```shell
openvpn3 session-start --config {{path/to/config.conf}}
```
#### List established sessions:
```shell
openvpn3 sessions-list
```
#### Disconnect the currently established session started with given configuration:
```shell
openvpn3 session-manage --config {{path/to/config.conf}} --disconnect
```
#### Import VPN configuration:
```shell
openvpn3 config-import --config {{path/to/config.conf}}
```
#### List imported configurations:
```shell
openvpn3 configs-list
```
{% endraw %}