---
layout: default
title: "iw"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iw">
  <a href="/en/linux/iw.html">iw</a> <a href="#iw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show and manipulate wireless devices.

#### Scan for available wireless networks:
```shell
iw dev {{wlp}} scan
```
#### Join an open wireless network:
```shell
iw dev {{wlp}} connect {{SSID}}
```
#### Close the current connection:
```shell
iw dev {{wlp}} disconnect
```
#### Show information about the current connection:
```shell
iw dev {{wlp}} link
```
{% endraw %}