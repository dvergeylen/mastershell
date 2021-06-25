---
layout: default
title: "create_ap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="create_ap">
  <a href="/en/linux/create_ap.html">create_ap</a> <a href="#create_ap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create an AP (Access Point) at any channel.

#### Create an open network with no passphrase:
```shell
create_ap {{wlan0}} {{eth0}} {{access_point_ssid}}
```
#### Use a WPA + WPA2 passphrase:
```shell
create_ap {{wlan0}} {{eth0}} {{access_point_ssid}} {{passphrase}}
```
#### Create an access point without Internet sharing:
```shell
create_ap -n {{wlan0}} {{acces_point_ssid}} {{passphrase}}
```
#### Create a bridged network with Internet sharing:
```shell
create_ap -m bridge {{wlan0}} {{eth0}} {{access_point_ssid}} {{passphrase}}
```
#### Create a bridged network with Internet sharing and a pre-configured bridge interface:
```shell
create_ap -m bridge {{wlan0}} {{br0}} {{access_point_ssid}} {{passphrase}}
```
#### Create an access port for Internet sharing from the same WiFi interface:
```shell
create_ap {{wlan0}} {{wlan0}} {{access_point_ssid}} {{passphrase}}
```
#### Choose a different WiFi adapter driver:
```shell
create_ap --driver {{wifi_adapter}} {{wlan0}} {{eth0}} {{access_point_ssid}} {{passphrase}}
```
{% endraw %}