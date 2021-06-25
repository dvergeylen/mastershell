---
layout: default
title: "st-flash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="st-flash">
  <a href="/en/common/st-flash.html">st-flash</a> <a href="#st-flash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Flash binary files to STM32 ARM Cortex microcontrollers.
> More information: <https://github.com/texane/stlink>.

#### Read 4096 bytes from the device starting from 0x8000000:
```shell
st-flash read {{firmware}}.bin {{0x8000000}} {{4096}}
```
#### Write firmware to device starting from 0x8000000:
```shell
st-flash write {{firmware}}.bin {{0x8000000}}
```
#### Erase firmware from device:
```shell
st-flash erase
```
{% endraw %}