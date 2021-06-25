---
layout: default
title: "bmon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bmon">
  <a href="/en/linux/bmon.html">bmon</a> <a href="#bmon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitor bandwidth and capture network related statistics.

#### Display the list of all the interfaces:
```shell
bmon -a
```
#### Display data transfer rates in bits per second:
```shell
bmon -b
```
#### Set policy to define which network interface(s) is/are displayed:
```shell
bmon -p {{interface_1,interface_2,interface_3}}
```
#### Set interval (in seconds) in which rate per counter is calculated:
```shell
bmon -R {{2.0}}
```
{% endraw %}