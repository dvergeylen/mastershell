---
layout: default
title: "cal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cal">
  <a href="/zh/osx/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打印日历信息.

#### 打印本月日历:
```shell
cal
```
#### 显示上个月，当前月，下个月的日历:
```shell
cal -3
```
#### 显示指定月份的日历（月份为 1-12 月）:
```shell
cal -m {{月}}
```
#### 显示全年日历:
```shell
cal -y
```
#### 显示指定某年的日历（年份为 4 个数字）:
```shell
cal {{年}}
```
#### 显示特定年和月的日历:
```shell
cal {{月}} {{年}}
```
#### 显示指定年的复活节日期:
```shell
ncal -e {{年}}
```
{% endraw %}