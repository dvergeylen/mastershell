---
layout: default
title: "taskkill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="taskkill">
  <a href="/zh/windows/taskkill.html">taskkill</a> <a href="#taskkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 按进程 id 或进程名终止进程.

#### 通过进程 id 终止进程:
```shell
taskkill /pid {{进程 id}}
```
#### 通过进程名终止进程:
```shell
taskkill /im {{进程名}}
```
#### 强制终止一个指定的进程:
```shell
taskkill /pid {{进程名}} /f
```
#### 终止一个进程及其子进程:
```shell
taskkill /im {{进程名}} /t
```
#### 终止远程计算机上的进程:
```shell
taskkill /pid {{进程 id}} /s {{远程主机名}}
```
#### 显示命令的帮助信息:
```shell
taskkill /?
```
{% endraw %}