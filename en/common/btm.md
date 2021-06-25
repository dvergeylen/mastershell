---
layout: default
title: "btm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="btm">
  <a href="/en/common/btm.html">btm</a> <a href="#btm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An alternative to `top`.
> Aims to be lightweight, cross-platform and more graphical than `top`.
> More information: <https://github.com/ClementTsang/bottom>.

#### Show the default layout (cpu, memory, temperatures, disk, network, and processes):
```shell
btm
```
#### Enable basic mode, removing charts and condensing data (similar to `top`):
```shell
btm --basic
```
#### Use big dots instead of small ones in charts:
```shell
btm --dot_marker
```
#### Show also battery charge and health status:
```shell
btm --battery
```
#### Refresh every 250 milliseconds and show the last 30 seconds in the charts:
```shell
btm --rate 250 --default_time_value 30000
```
{% endraw %}