---
layout: default
title: "vmstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vmstat">
  <a href="/en/linux/vmstat.html">vmstat</a> <a href="#vmstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report information about processes, memory, paging, block IO, traps, disks and CPU activity.
> More information: <https://manned.org/vmstat>.

#### Display virtual memory statistics:
```shell
vmstat
```
#### Display reports every 2 seconds for 5 times:
```shell
vmstat {{2}} {{5}}
```
{% endraw %}