---
layout: default
title: "cal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cal">
  <a href="/en/linux/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prints calendar information, with the current day highlighted.

#### Display a calendar for the current month:
```shell
cal
```
#### Display previous, current and next month:
```shell
cal -3
```
#### Use monday as the first day of the week:
```shell
cal --monday
```
#### Display a calendar for a specific year (4 digits):
```shell
cal {{year}}
```
#### Display a calendar for a specific month and year:
```shell
cal {{month}} {{year}}
```
{% endraw %}