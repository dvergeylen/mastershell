---
layout: default
title: "adb reverse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-reverse">
  <a href="/en/common/adb-reverse.html">adb reverse</a> <a href="#adb-reverse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Reverse: reverse socket connections from an Android emulator instance or connected Android devices.
> More information: <https://developer.android.com/studio/command-line/adb>.

#### List all reverse socket connections from emulators and devices:
```shell
adb reverse --list
```
#### Reverse a TCP port from an emulator or device to localhost:
```shell
adb reverse tcp:{{remote_port}} tcp:{{local_port}}
```
#### Remove a reverse socket connections from an emulator or device:
```shell
adb reverse --remove tcp:{{remote_port}}
```
#### Remove all reverse socket connections from all emulators and devices:
```shell
adb reverse --remove-all
```
{% endraw %}