---
layout: default
title: "nmcli device"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nmcli-device">
  <a href="/en/linux/nmcli-device.html">nmcli device</a> <a href="#nmcli-device"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Hardware device management with NetworkManager.
> More information: <https://man.archlinux.org/man/nmcli.1>.

#### Print the statuses of all network interfaces:
```shell
nmcli device status
```
#### Print the available Wi-Fi access points:
```shell
nmcli device wifi
```
#### Connect to the Wi-Fi network with a specified name and password:
```shell
nmcli device wifi connect {{ssid}} password {{password}}
```
#### Print password and QR code for the current Wi-Fi network:
```shell
nmcli device wifi show-password
```
{% endraw %}