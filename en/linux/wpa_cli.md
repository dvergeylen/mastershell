---
layout: default
title: "wpa_cli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wpa_cli">
  <a href="/en/linux/wpa_cli.html">wpa_cli</a> <a href="#wpa_cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add and configure wlan interfaces.

#### Scan for available networks:
```shell
wpa_cli scan
```
#### Show scan results:
```shell
wpa_cli scan_results
```
#### Add a network:
```shell
wpa_cli add_network {{number}}
```
#### Set a network's SSID:
```shell
wpa_cli set_network {{number}} ssid "{{SSID}}"
```
#### Enable network:
```shell
wpa_cli enable_network {{number}}
```
#### Save config:
```shell
wpa_cli save_config
```
{% endraw %}