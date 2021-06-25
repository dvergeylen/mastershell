---
layout: default
title: "cpuid"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cpuid">
  <a href="/en/linux/cpuid.html">cpuid</a> <a href="#cpuid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display detailed information about all CPUs.

#### Display information for all CPUs:
```shell
cpuid
```
#### Display information only for the current CPU:
```shell
cpuid -1
```
#### Display raw hex information with no decoding:
```shell
cpuid -r
```
{% endraw %}