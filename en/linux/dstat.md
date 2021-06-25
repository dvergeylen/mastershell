---
layout: default
title: "dstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dstat">
  <a href="/en/linux/dstat.html">dstat</a> <a href="#dstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Versatile tool for generating system resource statistics.
> More information: <http://dag.wieers.com/home-made/dstat>.

#### Display CPU, disk, net, paging and system statistics:
```shell
dstat
```
#### Display statistics every 5 seconds and 4 updates only:
```shell
dstat {{5}} {{4}}
```
#### Display CPU and memory statistics only:
```shell
dstat --cpu --mem
```
#### List all available dstat plugins:
```shell
dstat --list
```
#### Display the process using the most memory and most CPU:
```shell
dstat --top-mem --top-cpu
```
#### Display battery percentage and remaining battery time:
```shell
dstat --battery --battery-remain
```
{% endraw %}