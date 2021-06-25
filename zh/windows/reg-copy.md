---
layout: default
title: "reg copy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-copy">
  <a href="/zh/windows/reg-copy.html">reg copy</a> <a href="#reg-copy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 复制注册表中的键和值.

#### 将注册表键复制到新的注册表位置:
```shell
reg copy {{旧键名}} {{新键名}}
```
#### 递归将注册表键复制到新的注册表位置:
```shell
reg copy {{旧键名}} {{新键名}} /s
```
#### 在没有提示的情况下强制复制注册表键:
```shell
reg copy {{旧键名}} {{新键名}} /f
```
{% endraw %}