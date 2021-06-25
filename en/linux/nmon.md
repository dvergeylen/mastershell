---
layout: default
title: "nmon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nmon">
  <a href="/en/linux/nmon.html">nmon</a> <a href="#nmon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A system administrator, tuner, and benchmark tool.

#### Start nmon:
```shell
nmon
```
#### Save records to file ("-s 300 -c 288" by default):
```shell
nmon -f
```
#### Save records to file with a total of 240 measurements, by taking 30 seconds between each measurement:
```shell
nmon -f -s {{30}} -c {{240}}
```
{% endraw %}