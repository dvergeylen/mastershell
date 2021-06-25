---
layout: default
title: "boltctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="boltctl">
  <a href="/zh/linux/boltctl.html">boltctl</a> <a href="#boltctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 控制雷电 (thunderbolt) 设备。
> 更多信息：<https://manned.org/boltctl>.

#### 列出已连接并授权的设备：
```shell
boltctl
```
#### 列出已连接的设备，且包含未授权的设备：
```shell
boltctl list
```
#### 临时授权一个设备：
```shell
boltctl authorize {{设备uuid}}
```
#### 授权并记住一个设备：
```shell
boltctl enroll {{设备uuid}}
```
#### 取消一个设备的授权：
```shell
boltctl forget {{设备uuid}}
```
#### 显示一个设备的详细信息：
```shell
boltctl info {{设备uuid}}
```
{% endraw %}