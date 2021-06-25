---
layout: default
title: "lscpu"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lscpu">
  <a href="/en/linux/lscpu.html">lscpu</a> <a href="#lscpu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays information about the CPU architecture.

#### Display information about all CPUs:
```shell
lscpu
```
#### Display information in a table:
```shell
lscpu --extended
```
#### Display only information about offline CPUs in a table:
```shell
lscpu --extended --offline
```
{% endraw %}