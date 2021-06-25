---
layout: default
title: "adb"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="adb">
  <a href="/en/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge: communicate with an Android emulator instance or connected Android devices.
> More information: <https://developer.android.com/studio/command-line/adb>.

#### Check whether the adb server process is running and start it:
```shell
adb start-server
```
#### Terminate the adb server process:
```shell
adb kill-server
```
#### Start a remote shell in the target emulator/device instance:
```shell
adb shell
```
#### Push an Android application to an emulator/device:
```shell
adb install -r {{path/to/file.apk}}
```
#### Copy a file/directory from the target device:
```shell
adb pull {{path/to/device_file_or_directory}} {{path/to/local_destination_directory}}
```
#### Copy a file/directory to the target device:
```shell
adb push {{path/to/local_file_or_directory}} {{path/to/device_destination_directory}}
```
#### Get a list of connected devices:
```shell
adb devices
```
{% endraw %}