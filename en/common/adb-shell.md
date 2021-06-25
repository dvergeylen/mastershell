---
layout: default
title: "adb shell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-shell">
  <a href="/en/common/adb-shell.html">adb shell</a> <a href="#adb-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Shell: Run remote shell commands on an Android emulator instance or connected Android devices.
> More information: <https://developer.android.com/studio/command-line/adb>.

#### Start a remote interactive shell on the emulator/device:
```shell
adb shell
```
#### Get all the properties from emulator or device:
```shell
adb shell getprop
```
#### Revert all runtime permissions to their default:
```shell
adb shell pm reset-permissions
```
#### Revoke a dangerous permission for an application:
```shell
adb shell pm revoke {{package}} {{permission}}
```
#### Trigger a key event:
```shell
adb shell input keyevent {{keycode}}
```
#### Clear the data of an application on an emulator or device:
```shell
adb shell pm clear {{package}}
```
#### Start an activity on emulator/device:
```shell
adb shell am start -n {{package}}/{{activity}}
```
#### Start the home activity on an emulator or device:
```shell
adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN
```
{% endraw %}