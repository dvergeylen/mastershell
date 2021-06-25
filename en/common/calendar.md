---
layout: default
title: "calendar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="calendar">
  <a href="/en/common/calendar.html">calendar</a> <a href="#calendar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display upcoming events from a calendar file.
> More information: <https://www.commandlinux.com/man-page/man1/calendar.1.html>.

#### Show events for today and tomorrow (or the weekend on Friday) from the default calendar:
```shell
calendar
```
#### Look [A]head, showing events for the next 30 days:
```shell
calendar -A {{30}}
```
#### Look [B]ack, showing events for the previous 7 days:
```shell
calendar -B {{7}}
```
#### Show events from a custom calendar [f]ile:
```shell
calendar -f {{path/to/file}}
```
{% endraw %}