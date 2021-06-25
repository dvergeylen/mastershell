---
layout: default
title: "ac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ac">
  <a href="/zh/linux/ac.html">ac</a> <a href="#ac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打印用户连接时长数据。

#### 以小时为单位打印当前用户连接时间：
```shell
ac
```
#### 以小时为单位打印所有用户连接时间：
```shell
ac --individual-totals
```
#### 以小时为单位打印特定用户连接时间：
```shell
ac --individual-totals {{用户名}}
```
#### 以小时为单位打印特定用户每天连接时间：
```shell
ac --daily-totals --individual-totals {{用户名}}
```
#### 显示附加明细：
```shell
ac --compatibility
```
{% endraw %}