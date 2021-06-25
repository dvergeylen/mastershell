---
layout: default
title: "airmon-ng"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="airmon-ng">
  <a href="/en/common/airmon-ng.html">airmon-ng</a> <a href="#airmon-ng"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Activate monitor mode on wireless network devices.
> More information: <https://www.aircrack-ng.org/doku.php?id=airmon-ng>.

#### List wireless devices and their statuses:
```shell
sudo airmon-ng
```
#### Turn on monitor mode for a specific device:
```shell
sudo airmon-ng start {{wlan0}}
```
#### Kill disturbing processes that use wireless devices:
```shell
sudo airmon-ng check kill
```
#### Turn off monitor mode for a specific network interface:
```shell
sudo airmon-ng stop {{wlan0mon}}
```
{% endraw %}