---
layout: default
title: "date"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="date">
  <a href="/en/common/date.html">date</a> <a href="#date"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set or display the system date.
> More information: <https://www.gnu.org/software/coreutils/date>.

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
date -d @1473305798
```
#### Convert a specific date to the Unix timestamp format:
```shell
date -d "{{2018-09-01 00:00}}" +%s --utc
```
#### Display the current date using the RFC-3339 format (`YYYY-MM-DD hh:mm:ss TZ`):
```shell
date --rfc-3339=s
```
{% endraw %}