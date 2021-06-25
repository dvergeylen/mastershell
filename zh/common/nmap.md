---
layout: default
title: "nmap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nmap">
  <a href="/zh/common/nmap.html">nmap</a> <a href="#nmap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 网络探索工具和安全/端口扫描程序。
> 仅当以特权运行 Nmap 时，某些功能才激活。
> 更多信息见: <https://nmap.org>.

#### 检查IP地址是否可用，并猜测远程主机的操作系统：
```shell
nmap -O {{IP 或者 主机名}}
```
#### 尝试确定指定的主机是否启动以及它们的名称是什么：
```shell
nmap -sn {{IP 或者 主机名}} {{可选的其它地址}}
```
#### 像上面一样，如果主机启动了，还可以运行默认的1000端口TCP扫描：
```shell
nmap {{IP 或者 主机名}} {{可选的其它地址}}
```
#### 也可以启用脚本，服务检测，操作系统指纹识别和跟踪路由：
```shell
nmap -A {{一个地址 或者 多个地址}}
```
#### 假设网络连接良好并加快执行速度：
```shell
nmap -T4 {{一个地址 或者 多个地址}}
```
#### 扫描端口的特定列表（使用 `-p` 参数覆盖所有端口，如 `-p 1-65535`，也可以明确指定几个端口，如 `-p 3306,3307,3308`）：
```shell
nmap -p {{端口1, 端口2, ..., 端口N}} {{一个地址 或者 多个地址}}
```
#### 执行 TCP 和 UDP 扫描（`-sU` 只用 UDP 扫描，`-sZ` 用 SCTP 扫描，`-sO` 用于 IP 扫描）：
```shell
nmap -sSU {{一个地址 或者 多个地址}}
```
#### 使用默认 NSE 脚本执行针对该主机地址的完整端口、服务、版本检测扫描，以确定弱点和信息：
```shell
nmap -sC -sV {{一个地址 或者 多个地址}}
```
{% endraw %}