---
layout: default
title: "wpa_supplicant"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wpa_supplicant">
  <a href="/en/common/wpa_supplicant.html">wpa_supplicant</a> <a href="#wpa_supplicant"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage protected wireless networks.

#### Join a protected wireless network:
```shell
wpa_supplicant -i {{interface}} -c {{path/to/wpa_supplicant_conf.conf}}
```
#### Join a protected wireless network and run it in a daemon:
```shell
wpa_supplicant -B -i {{interface}} -c {{path/to/wpa_supplicant_conf.conf}}
```
{% endraw %}