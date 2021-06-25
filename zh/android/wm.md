---
layout: default
title: "wm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wm">
  <a href="/zh/android/wm.html">wm</a> <a href="#wm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示关于 Android 设备屏幕的信息。
> 此命令只能通过 `adb shell` 使用。
> 更多信息见：<https://adbinstaller.com/commands/adb-shell-wm-5b672b17e7958178a2955538>.

#### 显示 Android 设备屏幕的物理尺寸：
```shell
wm {{size}}
```
#### 显示 Android 设备屏幕的物理密度：
```shell
wm {{density}}
```
{% endraw %}