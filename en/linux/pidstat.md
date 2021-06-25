---
layout: default
title: "pidstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pidstat">
  <a href="/en/linux/pidstat.html">pidstat</a> <a href="#pidstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show system resource usage, including CPU, memory, IO etc.

#### Show CPU statistics at a 2 second interval for 10 times:
```shell
pidstat {{2}} {{10}}
```
#### Show page faults and memory utilization:
```shell
pidstat -r
```
#### Show input/output usage per process id:
```shell
pidstat -d
```
#### Show information on a specific PID:
```shell
pidstat -p {{PID}}
```
#### Show memory statistics for all processes whose command name include "fox" or "bird":
```shell
pidstat -C "{{fox|bird}}" -r -p ALL
```
{% endraw %}