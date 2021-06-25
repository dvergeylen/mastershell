---
layout: default
title: "dumpsys"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dumpsys">
  <a href="/zh/android/dumpsys.html">dumpsys</a> <a href="#dumpsys"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 提供关于 Android 系统服务的信息。
> 此命令只能通过 `adb shell` 使用。
> 更多信息见：https://developer.android.com/studio/command-line/dumpsys>.

#### 获取所有系统服务的诊断输出：
```shell
dumpsys
```
#### 获取指定系统服务的诊断输出：
```shell
dumpsys {{服务}}
```
#### 列出 `dumpsys` 可以提供的所有服务信息：
```shell
dumpsys -l
```
#### 列出服务的指定服务参数：
```shell
dumpsys {{服务}} -h
```
#### 从诊断输出中排除指定服务：
```shell
dumpsys --skip {{服务}}
```
#### 指定超时时间，以秒为单位（默认为 10s）：
```shell
dumpsys -t {{秒数}}
```
{% endraw %}