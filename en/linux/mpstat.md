---
layout: default
title: "mpstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mpstat">
  <a href="/en/linux/mpstat.html">mpstat</a> <a href="#mpstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report CPU statistics.

#### Display CPU statistics every 2 seconds:
```shell
mpstat {{2}}
```
#### Display 5 reports, one by one, at 2 second intervals:
```shell
mpstat {{2}} {{5}}
```
#### Display 5 reports, one by one, from a given processor, at 2 second intervals:
```shell
mpstat -P {{0}} {{2}} {{5}}
```
{% endraw %}