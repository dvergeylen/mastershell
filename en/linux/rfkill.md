---
layout: default
title: "rfkill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rfkill">
  <a href="/en/linux/rfkill.html">rfkill</a> <a href="#rfkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable and disable wireless devices.

#### List devices:
```shell
rfkill
```
#### Filter by columns:
```shell
rfkill -o {{ID,TYPE,DEVICE}}
```
#### Block devices by type (e.g. bluetooth, wlan):
```shell
rfkill block {{bluetooth}}
```
#### Unblock devices by type (e.g. bluetooth, wlan):
```shell
rfkill unblock {{wlan}}
```
#### Output in JSON format:
```shell
rfkill -J
```
{% endraw %}