---
layout: default
title: "wpa_passphrase"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wpa_passphrase">
  <a href="/en/linux/wpa_passphrase.html">wpa_passphrase</a> <a href="#wpa_passphrase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a WPA-PSK key from an ASCII passphrase for a given SSID.

#### Compute and display the WPA-PSK key for a given SSID reading the passphrase from stdin:
```shell
wpa_passphrase {{SSID}}
```
#### Compute and display WPA-PSK key for a given SSID specifying the passphrase as an argument:
```shell
wpa_passphrase {{SSID}} {{passphrase}}
```
{% endraw %}