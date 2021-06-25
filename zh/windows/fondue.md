---
layout: default
title: "fondue"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fondue">
  <a href="/zh/windows/fondue.html">fondue</a> <a href="#fondue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 可选 Windows 功能的命令行安装程序.

#### 启用一个指定的 Windows 功能:
```shell
fondue /enable-feature:{{功能}}
```
#### 向用户隐藏所有输出信息:
```shell
fondue /enable-feature:{{功能}} /hide-ux:all
```
#### 为错误报告指定调用者进程名称:
```shell
fondue /enable-feature:{{功能}} /caller-name:{{名称}}
```
{% endraw %}