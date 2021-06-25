---
layout: default
title: "arp-scan"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="arp-scan">
  <a href="/zh/linux/arp-scan.html">arp-scan</a> <a href="#arp-scan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 发送 ARP 数据包到特定主机（指定 IP 地址或主机名），来扫描本地网络.

#### 扫描当前本地网络:
```shell
arp-scan --localnet
```
#### 扫描带有自定义位掩码的 IP 网络:
```shell
arp-scan {{192.168.1.1}}/{{24}}
```
#### 扫描自定义范围内的 IP 网络:
```shell
arp-scan {{127.0.0.0}}-{{127.0.0.31}}
```
#### 扫描带有自定义子网掩码的 IP 网络:
```shell
arp-scan {{10.0.0.0}}:{{255.255.255.0}}
```
{% endraw %}