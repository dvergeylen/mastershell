---
layout: default
title: "perf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="perf">
  <a href="/en/linux/perf.html">perf</a> <a href="#perf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Framework for linux performance counter measurements.

#### Display basic performance counter stats for a command:
```shell
perf stat {{gcc hello.c}}
```
#### Display system-wide real time performance counter profile:
```shell
sudo perf top
```
#### Run a command and record its profile into `perf.data`:
```shell
sudo perf record {{command}}
```
#### Read `perf.data` (created by `perf record`) and display the profile:
```shell
sudo perf report
```
{% endraw %}