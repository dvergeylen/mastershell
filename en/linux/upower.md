---
layout: default
title: "upower"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="upower">
  <a href="/en/linux/upower.html">upower</a> <a href="#upower"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> System utility to provide power and battery information and statistics.
> More information: <https://upower.freedesktop.org/docs/upower.1.html>.

#### Display power and battery information:
```shell
upower --dump
```
#### List all power devices:
```shell
upower --enumerate
```
#### Watch for and print power status changes:
```shell
upower --monitor
```
#### Watch for and print detailed power status changes:
```shell
upower --monitor-detail
```
#### Display version:
```shell
upower --version
```
{% endraw %}