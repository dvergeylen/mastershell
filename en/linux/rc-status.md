---
layout: default
title: "rc-status"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rc-status">
  <a href="/en/linux/rc-status.html">rc-status</a> <a href="#rc-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show status info about runlevels.
> See also `openrc`.

#### Show a summary of services and their status:
```shell
rc-status
```
#### Include services in all runlevels in the summary:
```shell
rc-status --all
```
#### List services that have crashed:
```shell
rc-status --crashed
```
#### List manually started services:
```shell
rc-status --manual
```
#### List supervised services:
```shell
rc-status --supervised
```
#### Get the current runlevel:
```shell
rc-status --runlevel
```
#### List all runlevels:
```shell
rc-status --list
```
{% endraw %}