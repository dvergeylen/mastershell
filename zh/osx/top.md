---
layout: default
title: "top"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="top">
  <a href="/zh/osx/top.html">top</a> <a href="#top"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示运行进程的动态实时信息.

#### 执行 top 命令，界面中提供所有选项:
```shell
top
```
#### 按内部内存大小排序进程（默认顺序 - 进程 ID):
```shell
top -o mem
```
#### 首先按 CPU 启动顺序排序进程，然后按运行时间排序:
```shell
top -o cpu -O time
```
#### 只显示给定用户拥有的进程:
```shell
top -user {{用户名}}
```
#### 获取有关交互式命令的帮助（我测试并没看到这个功能）:
```shell
?
```
{% endraw %}