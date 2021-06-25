---
layout: default
title: "sar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sar">
  <a href="/en/linux/sar.html">sar</a> <a href="#sar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitor performance of various Linux subsystems.

#### Report I/O and transfer rate issued to physical devices, one per second (press CTRL+C to quit):
```shell
sar -b {{1}}
```
#### Report a total of 10 network device statistics, one per 2 seconds:
```shell
sar -n DEV {{2}} {{10}}
```
#### Report CPU utilization, one per 2 seconds:
```shell
sar -u ALL {{2}}
```
#### Report a total of 20 memory utilization statistics, one per second:
```shell
sar -r ALL {{1}} {{20}}
```
#### Report the run queue length and load averages, one per second:
```shell
sar -q {{1}}
```
#### Report paging statistics, one per 5 seconds:
```shell
sar -B {{5}}
```
{% endraw %}