---
layout: default
title: "bluetoothctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bluetoothctl">
  <a href="/en/linux/bluetoothctl.html">bluetoothctl</a> <a href="#bluetoothctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Handling bluetooth devices from the shell.

#### Enter the bluetoothctl shell:
```shell
bluetoothctl
```
#### List devices:
```shell
bluetoothctl -- devices
```
#### Pair a device:
```shell
bluetoothctl -- pair {{mac_address}}
```
#### Remove a device:
```shell
bluetoothctl -- remove {{mac_address}}
```
#### Connect a paired device:
```shell
bluetoothctl -- connect {{mac_address}}
```
#### Disconnect a paired device:
```shell
bluetoothctl -- disconnect {{mac_address}}
```
{% endraw %}