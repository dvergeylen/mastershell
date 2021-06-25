---
layout: default
title: "pm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pm">
  <a href="/zh/android/pm.html">pm</a> <a href="#pm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示关于 Android 设备上的应用程序的信息。
> 更多信息见：<https://developer.android.com/studio/command-line/adb#pm>.

#### 打印所有已安装应用程序的列表：
```shell
pm list packages
```
#### 打印所有已安装的系统应用程序的列表：
```shell
pm list packages -s
```
#### 打印所有已安装的第三方应用程序的列表：
```shell
pm list packages -3
```
#### 打印与指定关键字匹配的应用程序列表：
```shell
pm list packages {{关键词}}
```
#### 打印指定应用的 APK 的路径：
```shell
pm path {{应用名}}
```
{% endraw %}