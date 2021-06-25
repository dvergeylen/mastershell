---
layout: default
title: "st-util"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="st-util">
  <a href="/en/common/st-util.html">st-util</a> <a href="#st-util"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run GDB (GNU Debugger) server to interact with STM32 ARM Cortex microcontoller.
> More information: <https://github.com/texane/stlink>.

#### Run GDB server on port 4500:
```shell
st-util -p {{4500}}
```
#### Connect to GDB server:
```shell
(gdb) target extended-remote {{localhost}}:{{4500}}
```
#### Write firmware to device:
```shell
(gdb) load {{firmware.elf}}
```
{% endraw %}