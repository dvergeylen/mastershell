---
layout: default
title: "ipconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ipconfig">
  <a href="/zh/windows/ipconfig.html">ipconfig</a> <a href="#ipconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示和管理 Windows 的网络配置.

#### 显示网络适配器列表:
```shell
ipconfig
```
#### 显示网络适配器的详细列表:
```shell
ipconfig /all
```
#### 为一个网络适配器重新获取 IP 地址:
```shell
ipconfig /renew {{适配器}}
```
#### 为一个网络适配器释放 IP 地址:
```shell
ipconfig /release {{适配器}}
```
#### 清除所有 DNS 缓存:
```shell
ipconfig /flushdns
```
{% endraw %}