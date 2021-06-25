---
layout: default
title: "shutdown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shutdown">
  <a href="/zh/windows/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于关闭，重新启动或注销计算机的工具.

#### 关闭当前的计算机:
```shell
shutdown /s
```
#### 重启当前的计算机:
```shell
shutdown /r
```
#### 休眠当前的计算机:
```shell
shutdown /h
```
#### 注销当前的计算机:
```shell
shutdown /l
```
#### 指定在关闭之前等待的时间（以秒为单位）:
```shell
shutdown /s /t {{秒}}
```
#### 指定一个关机的理由:
```shell
shutdown /s /c "{{理由}}"
```
#### 在超时之前取消关机指令:
```shell
shutdown /a
```
#### 关闭远程的计算机:
```shell
shutdown /m {{\\ 主机名}}
```
{% endraw %}