---
layout: default
title: "netstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="netstat">
  <a href="/zh/osx/netstat.html">netstat</a> <a href="#netstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示与网络相关的信息，如打开的连接、打开的套接字端口等.
> 更多信息: <https://www.unix.com/man-page/osx/1/netstat>.

#### 列出所有端口:
```shell
netstat -a
```
#### 列出所有被侦听端口:
```shell
netstat -l
```
#### 列出侦听的 TCP 端口:
```shell
netstat -t
```
#### 显示监听给定协议监听的 PID 和程序名:
```shell
netstat -p {{协议}}
```
#### 打印路由表:
```shell
netstat -nr
```
{% endraw %}