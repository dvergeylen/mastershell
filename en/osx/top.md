---
layout: default
title: "top"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="top">
  <a href="/en/osx/top.html">top</a> <a href="#top"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display dynamic real-time information about running processes.

#### Start top, all options are available in the interface:
```shell
top
```
#### Start top sorting processes by internal memory size (default order - process ID):
```shell
top -o mem
```
#### Start top sorting processes first by CPU, then by running time:
```shell
top -o cpu -O time
```
#### Start top displaying only processes owned by given user:
```shell
top -user {{user_name}}
```
#### Get help about interactive commands:
```shell
?
```
{% endraw %}