---
layout: default
title: "gcal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gcal">
  <a href="/en/common/gcal.html">gcal</a> <a href="#gcal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays calendar.
> More information: <https://www.gnu.org/software/gcal>.

#### Display calendar for the current month:
```shell
gcal
```
#### Display calendar for the month of February of the year 2010:
```shell
gcal {{2}} {{2010}}
```
#### Provide calendar sheet with week numbers:
```shell
gcal --with-week-number
```
#### Change starting day of week to 1st day of the week (Monday):
```shell
gcal --starting-day={{1}}
```
#### Display the previous, current and next month surrounding today:
```shell
gcal .
```
{% endraw %}