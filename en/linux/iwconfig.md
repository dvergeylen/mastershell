---
layout: default
title: "iwconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="iwconfig">
  <a href="/en/linux/iwconfig.html">iwconfig</a> <a href="#iwconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configure and show the parameters of a wireless network interface.
> More information: <https://manned.org/iwconfig>.

#### Show the parameters and statistics of all the interfaces:
```shell
iwconfig
```
#### Show the parameters and statistics of the specified interface:
```shell
iwconfig {{interface}}
```
#### Set the ESSID (network name) of the specified interface (e.g., eth0 or wlp2s0):
```shell
iwconfig {{interface}} {{new_network_name}}
```
#### Set the operating mode of the specified interface:
```shell
iwconfig {{interface}} mode {{ad hoc|Managed|Master|Repeater|Secondary|Monitor|Auto}}
```
{% endraw %}