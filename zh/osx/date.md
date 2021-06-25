---
layout: default
title: "date"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="date">
  <a href="/zh/osx/date.html">date</a> <a href="#date"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 设置或显示系统日期.

#### 使用默认区域设置的格式显示当前日期 :
```shell
date +"%c"
```
#### 以 UTC 和 ISO 8601 格式显示当前日期:
```shell
date -u +"%Y-%m-%dT%H:%M:%SZ"
```
#### 将当前日期显示为 unix 时间戳（自 1970-01-01 00:00:00 以来的秒数）
```shell
date +%s
```
#### 使用默认格式显示特定日期（格式化指定 UNIX 时间戳）:
```shell
date -r 1473305798
```
{% endraw %}