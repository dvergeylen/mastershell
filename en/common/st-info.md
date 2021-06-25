---
layout: default
title: "st-info"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="st-info">
  <a href="/en/common/st-info.html">st-info</a> <a href="#st-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Provides information about connected STLink and STM32 devices.
> More information: <https://github.com/texane/stlink>.

#### Display amount of program memory available:
```shell
st-info --flash
```
#### Display amount of sram memory available:
```shell
st-info --sram
```
#### Display summarized information of the device:
```shell
st-info --probe
```
{% endraw %}