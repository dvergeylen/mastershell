---
layout: default
title: "chcpu"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chcpu">
  <a href="/en/linux/chcpu.html">chcpu</a> <a href="#chcpu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable/disable a system's CPUs.

#### Disable CPUs via a list of CPU ID numbers:
```shell
chcpu -d {{1,3}}
```
#### Enable a set of CPUs via a range of CPU ID numbers:
```shell
chcpu -e {{1-10}}
```
{% endraw %}