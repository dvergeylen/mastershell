---
layout: default
title: "date"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="date">
  <a href="/en/osx/date.html">date</a> <a href="#date"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set or display the system date.

#### Display the current date using the default locale's format:
```shell
date +"%c"
```
#### Display the current date in UTC and ISO 8601 format:
```shell
date -u +"%Y-%m-%dT%H:%M:%SZ"
```
#### Display the current date as a Unix timestamp (seconds since the Unix epoch):
```shell
date +%s
```
#### Display a specific date (represented as a Unix timestamp) using the default format:
```shell
date -r 1473305798
```
{% endraw %}