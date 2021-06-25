---
layout: default
title: "ethtool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ethtool">
  <a href="/en/linux/ethtool.html">ethtool</a> <a href="#ethtool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display and modify Network Interface Controller (NIC) parameters.
> More information: <http://man7.org/linux/man-pages/man8/ethtool.8.html>.

#### Display the current settings for an interface:
```shell
ethtool {{eth0}}
```
#### Display the driver information for an interface:
```shell
ethtool --driver {{eth0}}
```
#### Display the network usage statistics for an interface:
```shell
ethtool --statistics {{eth0}}
```
#### Blink one or more LEDs on an interface for 10 seconds:
```shell
ethtool --identify {{eth0}} {{10}}
```
#### Set the link speed, duplex mode, and parameter auto-negotiation for a given interface:
```shell
ethtool -s {{eth0}} speed {{10|100|1000}} duplex {{half|full}} autoneg {{on|off}}
```
{% endraw %}