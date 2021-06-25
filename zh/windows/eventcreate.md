---
layout: default
title: "eventcreate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eventcreate">
  <a href="/zh/windows/eventcreate.html">eventcreate</a> <a href="#eventcreate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在事件日志中创建自定义条目.
> 事件 ID 可以是 1 到 1000 之间的任意数值.

#### 在日志中创建一个具有给定 id（1-1000）的新事件:
```shell
eventcreate /t {{success|error|warning|information}} /id {{id}} /d "{{消息}}"
```
#### 在特定事件日志中创建事件:
```shell
eventcreate /l {{日志名}} /t {{类型}} /id {{id}} /d "{{消息}}"
```
#### 为新创建的事件指定来源:
```shell
eventcreate /so {{来源名}} /t {{类型}} /id {{id}} /d "{{消息}}"
```
#### 在远程计算机的事件日志中创建事件:
```shell
eventcreate /s {{主机名}} /u {{用户名}} /p {{密码}} /t {{类型}} /id {{id}} /d "{{消息}}"
```
{% endraw %}