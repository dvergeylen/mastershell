---
layout: default
title: "svcs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="svcs">
  <a href="/en/sunos/svcs.html">svcs</a> <a href="#svcs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List information about running services.
> More information: <https://www.unix.com/man-page/linux/1/svcs>.

#### List all running services:
```shell
svcs
```
#### List services that are not running:
```shell
svcs -vx
```
#### List information about a service:
```shell
svcs apache
```
#### Show location of service log file:
```shell
svcs -L apache
```
#### Display end of a service log file:
```shell
tail $(svcs -L apache)
```
{% endraw %}