---
layout: default
title: "jcal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jcal">
  <a href="/en/common/jcal.html">jcal</a> <a href="#jcal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display calendar information in the Jalali format, with the current day highlighted.
> More information: <http://www.nongnu.org/jcal/>.

#### Display a calendar for the current month:
```shell
jcal
```
#### Display the previous, current, and next months:
```shell
jcal -3
```
#### Display a calendar for a specific year (4 digits):
```shell
jcal {{year}}
```
#### Display a calendar for a specific month and year:
```shell
jcal {{year}} {{month}}
```
{% endraw %}