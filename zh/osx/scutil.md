---
layout: default
title: "scutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scutil">
  <a href="/zh/osx/scutil.html">scutil</a> <a href="#scutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理系统配置参数.
> 设置配置时必须是 root 权限.

#### 显示 DNS 配置:
```shell
scutil --dns
```
#### 显示代理配置:
```shell
scutil --proxy
```
#### 获取计算机名称:
```shell
scutil --get ComputerName
```
#### 设置计算机名称:
```shell
sudo scutil --set ComputerName {{我的计算机名}}
```
#### 获取主机名 ( HostName ):
```shell
scutil --get HostName
```
#### 设置主机名:
```shell
scutil --set HostName {{hostname}}
```
{% endraw %}