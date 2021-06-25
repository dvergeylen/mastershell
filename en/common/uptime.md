---
layout: default
title: "uptime"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uptime">
  <a href="/en/common/uptime.html">uptime</a> <a href="#uptime"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tell how long the system has been running and other information.
> More information: <https://www.gnu.org/software/coreutils/uptime>.

#### Print current time, uptime, number of logged-in users and other information:
```shell
uptime
```
#### Show only the amount of time the system has been booted for:
```shell
uptime --pretty
```
#### Print the date and time the system booted up at:
```shell
uptime --since
```
#### Show version information:
```shell
uptime --version
```
{% endraw %}