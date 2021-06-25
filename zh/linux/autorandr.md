---
layout: default
title: "autorandr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autorandr">
  <a href="/zh/linux/autorandr.html">autorandr</a> <a href="#autorandr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 自动调节屏幕布局。

#### 保存当前屏幕布局：
```shell
autorandr -s {{配置文件名}}
```
#### 显示保存的配置：
```shell
autorandr
```
#### 切换设置：
```shell
autorandr -l {{配置文件名}}
```
#### 设置默认设置：
```shell
autorandr -d {{配置文件名}}
```
{% endraw %}