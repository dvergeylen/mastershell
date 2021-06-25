---
layout: default
title: "android"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#am">am</a>
* <a href="#bugreport">bugreport</a>
* <a href="#cmd">cmd</a>
* <a href="#dalvikvm">dalvikvm</a>
* <a href="#dumpsys">dumpsys</a>
* <a href="#getprop">getprop</a>
* <a href="#input">input</a>
* <a href="#logcat">logcat</a>
* <a href="#pm">pm</a>
* <a href="#settings">settings</a>
* <a href="#wm">wm</a>

{% raw %}
<h2 id="am">
  <a href="/zh/android/am.html">am</a> <a href="#am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android 活动管理器。
> 更多信息见：<https://developer.android.com/studio/command-line/adb#am>.

#### 启动一个指定的活动：
```shell
am start -n {{com.android.settings/.Settings}}
```
#### 启动一个活动并将数据传递给它：
```shell
am start -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
#### 启动与特定操作和类别匹配的活动：
```shell
am start -a {{android.intent.action.MAIN}} -c {{android.intent.category.HOME}}
```
#### 将意图转换为 URI：
```shell
am to-uri -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
{% endraw %}{% raw %}
<h2 id="bugreport">
  <a href="/zh/android/bugreport.html">bugreport</a> <a href="#bugreport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示安卓的 Bug 报告。
> 该命令只能通过 `adb shell` 使用。
> 更多信息：<https://android.googlesource.com/platform/frameworks/native/+/master/cmds/bugreport/>.

#### 显示 Android 设备的完整错误报告：
```shell
bugreport
```
{% endraw %}{% raw %}
<h2 id="cmd">
  <a href="/zh/android/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android 服务管理器。
> 更多信息见： <https://cs.android.com/android/platform/superproject/+/master:frameworks/native/cmds/cmd/>.

#### 列出所有正在运行的服务：
```shell
cmd -l
```
#### 调用指定服务：
```shell
cmd {{alarm}}
```
#### 调用服务同时传递参数：
```shell
cmd {{vibrator}} {{vibrate 300}}
```
{% endraw %}{% raw %}
<h2 id="dalvikvm">
  <a href="/zh/android/dalvikvm.html">dalvikvm</a> <a href="#dalvikvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Java 虚拟机。
> 更多信息见：<https://source.android.com/devices/tech/dalvik>.

#### 启动一个 Java 程序：
```shell
dalvikvm -classpath {{path/to/file.jar}} {{classname}}
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="logcat">
  <a href="/zh/android/logcat.html">logcat</a> <a href="#logcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 转储系统消息日志。
> 更多信息见：https://developer.android.com/studio/command-line/logcat>.

#### 显示系统日志：
```shell
logcat
```
#### 将系统日志写入文件：
```shell
logcat -f {{文件路径}}
```
#### 显示与正则表达式匹配的行：
```shell
logcat --regex {{正则表达式}}
```
{% endraw %}{% raw %}
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
{% endraw %}{% raw %}
<h2 id="settings">
  <a href="/zh/android/settings.html">settings</a> <a href="#settings"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 获取关于 Android OS 的信息。
> 更多信息见：https://adbinstaller.com/commands/adb-shell-settings-5b670d5ee7958178a2955536>.

#### 在 `全局` 命名空间中显示环境变量列表：
```shell
settings list {{global}}
```
#### 获取指定环境变量的值：
```shell
settings get {{global}} {{airplane_mode_on}}
```
#### 设置指定环境变量的值：
```shell
settings put {{system}} {{screen_brightness}} {{42}}
```
#### 删除指定环境变量：
```shell
settings delete {{secure}} {{screensaver_enabled}}
```
{% endraw %}{% raw %}
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