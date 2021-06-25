---
layout: default
title: "cal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cal">
  <a href="/en/osx/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prints calendar information.

#### Display a calendar for the current month:
```shell
cal
```
#### Display previous, current and next month:
```shell
cal -3
```
#### Display a calendar for a specific month (1-12 or name):
```shell
cal -m {{month}}
```
#### Display a calendar for the current year:
```shell
cal -y
```
#### Display a calendar for a specific year (4 digits):
```shell
cal {{year}}
```
#### Display a calendar for a specific month and year:
```shell
cal {{month}} {{year}}
```
#### Display date of Easter (Western Christian churches) in a given year:
```shell
ncal -e {{year}}
```
{% endraw %}