---
layout: default
title: "reboot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reboot">
  <a href="/en/linux/reboot.html">reboot</a> <a href="#reboot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reboot the system.
> More information: <https://www.man7.org/linux/man-pages/man8/reboot.8.html>.

#### Reboot the system:
```shell
reboot
```
#### Power off the system (same as `poweroff`):
```shell
reboot --poweroff
```
#### Halt the system (same as `halt`):
```shell
reboot --halt
```
#### Reboot immediately without contacting the system manager:
```shell
reboot --force --force
```
#### Write the wtmp shutdown entry without rebooting the system:
```shell
reboot --wtmp-only
```
{% endraw %}