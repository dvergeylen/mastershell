---
layout: default
title: "cpuid"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cpuid">
  <a href="/zh/linux/cpuid.html">cpuid</a> <a href="#cpuid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示有关所有 CPU 的详细信息.

#### 显示所有 CPU 的信息:
```shell
cpuid
```
#### 仅显示当前 CPU 的信息:
```shell
cpuid -1
```
#### 显示原始十六进制信息，不进行解码:
```shell
cpuid -r
```
{% endraw %}