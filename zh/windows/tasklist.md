---
layout: default
title: "tasklist"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tasklist">
  <a href="/zh/windows/tasklist.html">tasklist</a> <a href="#tasklist"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示本地或远程计算机上当前正在运行的进程的列表.

#### 显示当前正在运行的进程:
```shell
tasklist
```
#### 使用指定的格式显示当前进程列表:
```shell
tasklist /fo {{table|list|csv}}
```
#### 已匹配的方式 (.exe, .dll) 显示当前运行的进程:
```shell
tasklist /m {{匹配模式}}
```
#### 显示在远程计算机上运行的进程:
```shell
tasklist /s {{远程主机名}} /u {{用户名}} /p {{密码}}
```
#### 显示每个进程中的服务信息:
```shell
tasklist /svc
```
{% endraw %}