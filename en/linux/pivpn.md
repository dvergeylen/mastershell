---
layout: default
title: "pivpn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pivpn">
  <a href="/en/linux/pivpn.html">pivpn</a> <a href="#pivpn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Easy security-hardened OpenVPN setup and manager.
> Originally designed for the Raspberry Pi, but works on other Linux devices too.
> More information: <http://www.pivpn.io/>.

#### Add a new client device:
```shell
sudo pivpn add
```
#### List all client devices:
```shell
sudo pivpn list
```
#### List currently connected devices and their statistics:
```shell
sudo pivpn clients
```
#### Revoke a previously authenticated device:
```shell
sudo pivpn revoke
```
#### Uninstall PiVPN:
```shell
sudo pivpn uninstall
```
{% endraw %}