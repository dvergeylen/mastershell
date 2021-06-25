---
layout: default
title: "adb install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb-install">
  <a href="/en/common/adb-install.html">adb install</a> <a href="#adb-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Install: Push packages to an Android emulator instance or connected Android devices.
> More information: <https://developer.android.com/studio/command-line/adb>.

#### Push an Android application to an emulator/device:
```shell
adb install {{path/to/file.apk}}
```
#### Reinstall an existing app, keeping its data:
```shell
adb install -r {{path/to/file.apk}}
```
#### Grant all permissions listed in the app manifest:
```shell
adb install -g {{path/to/file.apk}}
```
#### Quickly update an installed package by only updating the parts of the APK that changed:
```shell
adb install --fastdeploy {{path/to/file.apk}}
```
{% endraw %}