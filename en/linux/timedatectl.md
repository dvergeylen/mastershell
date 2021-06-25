---
layout: default
title: "timedatectl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="timedatectl">
  <a href="/en/linux/timedatectl.html">timedatectl</a> <a href="#timedatectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control the system time and date.
> More information: <https://manned.org/timedatectl.1>.

#### Check the current system clock time:
```shell
timedatectl
```
#### Set the local time of the system clock directly:
```shell
timedatectl set-time "{{yyyy-MM-dd hh:mm:ss}}"
```
#### List available timezones:
```shell
timedatectl list-timezones
```
#### Set the system timezone:
```shell
timedatectl set-timezone {{timezone}}
```
#### Enable Network Time Protocol (NTP) synchronization:
```shell
timedatectl set-ntp on
```
{% endraw %}