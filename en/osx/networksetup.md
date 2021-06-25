---
layout: default
title: "networksetup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="networksetup">
  <a href="/en/osx/networksetup.html">networksetup</a> <a href="#networksetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configuration tool for Network System Preferences.

#### List available network service providers (Ethernet, Wi-Fi, Bluetooth, etc):
```shell
networksetup -listallnetworkservices
```
#### Show network settings for a particular networking device:
```shell
networksetup -getinfo "{{Wi-Fi}}"
```
#### Get currently connected Wi-Fi network name (Wi-Fi device usually en0 or en1):
```shell
networksetup -getairportnetwork {{en0}}
```
#### Connect to a particular Wi-Fi network:
```shell
networksetup -setairportnetwork {{en0}} "{{Airport Network SSID}}" {{password}}
```
{% endraw %}