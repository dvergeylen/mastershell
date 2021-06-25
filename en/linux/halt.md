---
layout: default
title: "halt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="halt">
  <a href="/en/linux/halt.html">halt</a> <a href="#halt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Halt the system.
> More information: <https://www.man7.org/linux/man-pages/man8/halt.8.html>.

#### Halt the system:
```shell
halt
```
#### Power off the system (same as `poweroff`):
```shell
halt --poweroff
```
#### Reboot the system (same as `reboot`):
```shell
halt --reboot
```
#### Halt immediately without contacting the system manager:
```shell
halt --force --force
```
#### Write the wtmp shutdown entry without halting the system:
```shell
halt --wtmp-only
```
{% endraw %}