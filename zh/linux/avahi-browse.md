---
layout: default
title: "avahi-browse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="avahi-browse">
  <a href="/zh/linux/avahi-browse.html">avahi-browse</a> <a href="#avahi-browse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示通过 mDNS/DNS-SD 暴露在本地网络的服务和主机。
> Avahi 与苹果设备的 Bonjour (Zeroconf) 兼容。
> 更多信息：<https://www.avahi.org/>.

#### 列出本地网络中的所有服务和他们的地址与端口，忽略他们本地的地址和端口：
```shell
avahi-browse --all --resolve --ignore-local
```
#### 列出所有的域名：
```shell
avahi-browse --browse-domains
```
#### 只搜索一个特定的域名：
```shell
avahi-browse --all --domain={{domain}}
```
{% endraw %}