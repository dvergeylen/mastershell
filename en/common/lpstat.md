---
layout: default
title: "lpstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lpstat">
  <a href="/en/common/lpstat.html">lpstat</a> <a href="#lpstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show status information about printers.

#### List printers present on the machine and whether they are enabled for printing:
```shell
lpstat -p
```
#### Show the default printer:
```shell
lpstat -d
```
#### Display all available status information:
```shell
lpstat -t
```
#### Show a list of print jobs queued by the specified user:
```shell
lpstat -u {{user}}
```
{% endraw %}