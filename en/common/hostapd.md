---
layout: default
title: "hostapd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hostapd">
  <a href="/en/common/hostapd.html">hostapd</a> <a href="#hostapd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Start an access point using a wireless interface.
> More information: <https://w1.fi/hostapd/>.

#### Start an access point:
```shell
sudo hostapd {{path/to/hostapd.conf}}
```
#### Start an access point, forking into the background:
```shell
sudo hostapd -B {{path/to/hostapd.conf}}
```
{% endraw %}