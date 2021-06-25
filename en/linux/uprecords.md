---
layout: default
title: "uprecords"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uprecords">
  <a href="/en/linux/uprecords.html">uprecords</a> <a href="#uprecords"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays a summary of historical uptime records.

#### Display a summary of the top 10 historical uptime records:
```shell
uprecords
```
#### Display the top 25 records:
```shell
uprecords -m {{25}}
```
#### Display the downtime between reboots instead of the kernel version:
```shell
uprecords -d
```
#### Show the most recent reboots:
```shell
uprecords -B
```
#### Don't truncate information:
```shell
uprecords -w
```
{% endraw %}