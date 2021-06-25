---
layout: default
title: "fc-list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fc-list">
  <a href="/zh/linux/fc-list.html">fc-list</a> <a href="#fc-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 列出系统上安装的可用字体。

#### 返回系统中已安装字体的列表：
```shell
fc-list
```
#### 返回具有给定名称的已安装字体的列表：
```shell
fc-list | grep '{{DejaVu Serif}}'
```
#### 返回系统中已安装字体的数量：
```shell
fc-list | wc -l
```
{% endraw %}