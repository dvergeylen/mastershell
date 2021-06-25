---
layout: default
title: "more"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="more">
  <a href="/zh/windows/more.html">more</a> <a href="#more"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 分页显示标准输入或文件的输出.

#### 分页显示标准输入的输出:
```shell
{{echo test}} | more
```
#### 分页显示一个或多个文件的内容:
```shell
more {{文件的路径}}
```
#### 将制表符转换为指定的空格数:
```shell
more {{文件的路径}} /t{{空格数}}
```
#### 显示内容前先清屏:
```shell
more {{文件的路径}} /c
```
#### 从第 5 行开始显示输出:
```shell
more {{文件的路径}} +{{5}}
```
#### 启用扩展交互模式（请参阅使用帮助）:
```shell
more {{文件的路径}} /e
```
#### 显示全部帮助信息:
```shell
more /?
```
{% endraw %}