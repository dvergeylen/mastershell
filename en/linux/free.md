---
layout: default
title: "free"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="free">
  <a href="/en/linux/free.html">free</a> <a href="#free"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display amount of free and used memory in the system.

#### Display system memory:
```shell
free
```
#### Display memory in Bytes/KB/MB/GB:
```shell
free -{{b|k|m|g}}
```
#### Display memory in human readable units:
```shell
free -h
```
#### Refresh the output every 2 seconds:
```shell
free -s {{2}}
```
{% endraw %}