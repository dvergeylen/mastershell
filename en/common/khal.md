---
layout: default
title: "khal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="khal">
  <a href="/en/common/khal.html">khal</a> <a href="#khal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A text-based calendar and scheduling application for the command-line.
> More information: <https://lostpackets.de/khal>.

#### Start khal on interactive mode:
```shell
ikhal
```
#### Print all events scheduled in personal calendar for the next seven days:
```shell
khal list -a {{personal}} {{today}} {{7d}}
```
#### Print all events scheduled not in personal calendar for tomorrow at 10:00:
```shell
khal at -d {{personal}} {{tomorrow}} {{10:00}}
```
#### Print a calendar with a list of events for the next three months:
```shell
khal calendar
```
#### Add new event to personal calendar:
```shell
khal new -a {{personal}} {{2020-09-08}} {{18:00}} {{18:30}} "{{Dentist appointment}}"
```
{% endraw %}