---
layout: default
title: "input"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="input">
  <a href="/zh/android/input.html">input</a> <a href="#input"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将事件代码或触摸屏手势发送到 Android 设备。
> 此命令只能通过 `adb shell` 使用。
> 更多信息见：<https://developer.android.com/reference/android/view/KeyEvent.html#constants_1>.

#### 将单个字符的事件代码发送到 Android 设备：
```shell
input keyevent {{event_code}}
```
#### 将文本发送到Android设备（`%s` 代表空格）：
```shell
input text "{{text}}"
```
#### 将轻触发送到 Android 设备：
```shell
input tap {{x_pos}} {{y_pos}}
```
#### 将滑动手势发送到 Android 设备：
```shell
input swipe {{x_start}} {{y_start}} {{x_end}} {{y_end}} {{duration_in_ms}}
```
#### 使用滑动手势将长按发送到 Android 设备：
```shell
input swipe {{x_pos}} {{y_pos}} {{x_pos}} {{y_pos}} {{duration_in_ms}}
```
{% endraw %}