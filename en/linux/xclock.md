---
layout: default
title: "xclock"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xclock">
  <a href="/en/linux/xclock.html">xclock</a> <a href="#xclock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the time in analog or digital form.

#### Display an analog clock:
```shell
xclock
```
#### Display a 24-hour digital clock with the hour and minute fields only:
```shell
xclock -digital -brief
```
#### Display a digital clock using an strftime format string (see strftime(3)):
```shell
xclock -digital -strftime {{format}}
```
#### Display a 24-hour digital clock with the hour, minute and second fields that updates every second:
```shell
xclock -digital -strftime '%H:%M:%S' -update 1
```
#### Display a 12-hour digital clock with the hour and minute fields only:
```shell
xclock -digital -twelve -brief
```
{% endraw %}