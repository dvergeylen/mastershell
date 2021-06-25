---
layout: default
title: "vnstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vnstat">
  <a href="/en/linux/vnstat.html">vnstat</a> <a href="#vnstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A console-based network traffic monitor.

#### Display traffic summary for all interfaces:
```shell
vnstat
```
#### Display traffic summary for a specific network interface:
```shell
vnstat -i {{eth0}}
```
#### Display live stats for a specific network interface:
```shell
vnstat -l -i {{eth0}}
```
#### Show traffic statistics on an hourly basis for the last 24 hours using a bar graph:
```shell
vnstat -hg
```
#### Measure and show average traffic for 30 seconds:
```shell
vnstat -tr {{30}}
```
{% endraw %}