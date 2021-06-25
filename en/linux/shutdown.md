---
layout: default
title: "shutdown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shutdown">
  <a href="/en/linux/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shutdown and reboot the system.

#### Power off (halt) immediately:
```shell
shutdown -h now
```
#### Reboot immediately:
```shell
shutdown -r now
```
#### Reboot in 5 minutes:
```shell
shutdown -r +{{5}} &
```
#### Shutdown at 1:00 pm (Uses 24h clock):
```shell
shutdown -h 13:00
```
#### Cancel a pending shutdown/reboot operation:
```shell
shutdown -c
```
{% endraw %}