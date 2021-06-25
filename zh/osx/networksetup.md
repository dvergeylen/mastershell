---
layout: default
title: "networksetup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="networksetup">
  <a href="/zh/osx/networksetup.html">networksetup</a> <a href="#networksetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 网络系统首选项配置工具.

#### 列出可用的网络服务源（以太网、Wi-Fi、蓝牙等）:
```shell
networksetup -listallnetworkservices
```
#### 显示特定网络设备的配置信息:
```shell
networksetup -getinfo "{{Wi-Fi}}"
```
#### 获取当前连接的 Wi-Fi 网络名称（Wi-Fi 设备通常为 en0 或 en1）:
```shell
networksetup -getairportnetwork {{en0}}
```
#### 连接到给定的 Wi-Fi 网络 Connect to a particular Wi-Fi network:
```shell
networksetup -setairportnetwork {{en0}} "{{无线网 SSID}}" {{密码}}
```
{% endraw %}