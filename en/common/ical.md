---
layout: default
title: "ical"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ical">
  <a href="/en/common/ical.html">ical</a> <a href="#ical"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A Hirji/Islamic calendar and converter for the terminal.
> More information: <https://manned.org/ical>.

#### Display the current month's calendar:
```shell
ical
```
#### Convert a Gregorian date to a Hijri date:
```shell
ical --gregorian {{yyyymmdd}}
```
#### Convert a Hirji date to a Gregorian date:
```shell
ical --hijri {{yyyymmdd}}
```
{% endraw %}