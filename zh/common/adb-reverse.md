---
layout: default
title: "adb reverse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-reverse">
  <a href="/zh/common/adb-reverse.html">adb reverse</a> <a href="#adb-reverse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 安卓调试桥-反射: 反向映射安卓模拟器实例或者已连接的实体设备的套接字连接.
> 更多信息: <https://developer.android.com/studio/command-line/adb>.

#### 列出所有来自模拟器和设备的映射连接
```shell
adb reverse —list
```
#### 将TCP端口从安卓模拟器或设备中映射到localhost:
```shell
adb reverse tcp:{{远程端口}} tcp:{{本地端口}}
```
#### 从安卓模拟器或设备移除一个反向socket连接:
```shell
adb reverse --remove tcp:{{远程端口}}
```
#### 从安卓模拟器或设备移除所有反向socket连接:
```shell
adb reverse --remove-all
```
{% endraw %}