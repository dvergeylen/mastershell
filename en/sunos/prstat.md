---
layout: default
title: "prstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="prstat">
  <a href="/en/sunos/prstat.html">prstat</a> <a href="#prstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report active process statistics.
> More information: <https://www.unix.com/man-page/sunos/1m/prstat>.

#### Examine all processes and reports statistics sorted by CPU usage:
```shell
prstat
```
#### Examine all processes and reports statistics sorted by memory usage:
```shell
prstat -s rss
```
#### Report total usage summary for each user:
```shell
prstat -t
```
#### Report microstate process accounting information:
```shell
prstat -m
```
#### Print out a list of top 5 CPU using processes every second:
```shell
prstat -c -n 5 -s cpu 1
```
{% endraw %}