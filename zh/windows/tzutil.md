---
layout: default
title: "tzutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tzutil">
  <a href="/zh/windows/tzutil.html">tzutil</a> <a href="#tzutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于显示或配置系统时区的工具.

#### 获取当前的时区:
```shell
tzutil /g
```
#### 显示可用的时区列表:
```shell
tzutil /l
```
#### 将系统时区设置为特定值:
```shell
tzutil /s {{时区 id}}
```
{% endraw %}