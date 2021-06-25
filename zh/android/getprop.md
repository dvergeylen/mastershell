---
layout: default
title: "getprop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="getprop">
  <a href="/zh/android/getprop.html">getprop</a> <a href="#getprop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示关于 Android 系统属性的信息。
> 更多信息见：<https://manned.org/getprop>.

#### 显示关于 Android 系统属性的信息：
```shell
getprop
```
#### 显示关于指定属性的信息：
```shell
getprop {{prop}}
```
#### 显示 SDK API 级别：
```shell
getprop {{ro.build.version.sdk}}
```
#### 显示 Android 版本：
```shell
getprop {{ro.build.version.release}}
```
#### 显示 Android 设备型号：
```shell
getprop {{ro.vendor.product.model}}
```
#### 显示 OEM 解锁状态：
```shell
getprop {{ro.oem_unlock_supported}}
```
#### 显示 Android WiFi 卡的 MAC 地址：
```shell
getprop {{ro.boot.wifimacaddr}}
```
{% endraw %}