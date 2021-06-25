---
layout: default
title: "ps"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ps">
  <a href="/en/common/ps.html">ps</a> <a href="#ps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Information about running processes.

#### List all running processes:
```shell
ps aux
```
#### List all running processes including the full command string:
```shell
ps auxww
```
#### Search for a process that matches a string:
```shell
ps aux | grep {{string}}
```
#### List all processes of the current user in extra full format:
```shell
ps --user $(id -u) -F
```
#### List all processes of the current user as a tree:
```shell
ps --user $(id -u) f
```
#### Get the parent pid of a process:
```shell
ps -o ppid= -p {{pid}}
```
#### Sort processes by memory consumption:
```shell
ps --sort size
```
{% endraw %}