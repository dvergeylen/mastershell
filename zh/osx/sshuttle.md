---
layout: default
title: "sshuttle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sshuttle">
  <a href="/zh/osx/sshuttle.html">sshuttle</a> <a href="#sshuttle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 通过 ssh 连接传输流量的透明代理服务器.
> 不需要管理员或远程 ssh 服务器上的任何特殊设置.

#### 通过远程 ssh 服务器转发所有 IPv4 TCP 流量:
```shell
sshuttle --remote={{用户名}}@{{服务器名}} {{0.0.0.0/0}}
```
#### 转发所有 IPv4 TCP 和 DNS 流量:
```shell
sshuttle --dns --remote={{用户名}}@{{服务器名}} {{0.0.0.0/0}}
```
#### 使用 tproxy 方法转发所有 IPv4 和 IPv6 流量:
```shell
sudo sshuttle --method=tproxy --remote={{用户名}}@{{服务器名}} {{0.0.0.0/0}} {{::/0}} --exclude={{你本地 IP 地址}} --exclude={{SSH 服务器的 IP 地址}}
```
{% endraw %}