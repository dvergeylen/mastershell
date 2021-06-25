---
layout: default
title: "poweroff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="poweroff">
  <a href="/en/linux/poweroff.html">poweroff</a> <a href="#poweroff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Power off the system.
> More information: <https://www.man7.org/linux/man-pages/man8/poweroff.8.html>.

#### Power off the system:
```shell
poweroff
```
#### Halt the system (same as `halt`):
```shell
poweroff --halt
```
#### Reboot the system (same as `reboot`):
```shell
poweroff --reboot
```
#### Shut down immediately without contacting the system manager:
```shell
poweroff --force --force
```
#### Write the wtmp shutdown entry without shutting down the system:
```shell
poweroff --wtmp-only
```
{% endraw %}