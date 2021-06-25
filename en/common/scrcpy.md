---
layout: default
title: "scrcpy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scrcpy">
  <a href="/en/common/scrcpy.html">scrcpy</a> <a href="#scrcpy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display and control your Android device on a desktop.
> More information: <https://github.com/Genymobile/scrcpy>.

#### Display a mirror of a connected device:
```shell
scrcpy
```
#### Display a mirror of a specific device based on its ID or IP address (find it under the `adb devices` command):
```shell
scrcpy --serial {{0123456789abcdef|192.168.0.1:5555}}
```
#### Start display in fullscreen mode:
```shell
scrcpy --fullscreen
```
#### Rotate the display screen. Each incremental value adds a 90 degree counterclockwise rotation:
```shell
scrcpy --rotation {{0|1|2|3}}
```
#### Show touches on physical device:
```shell
scrcpy --show-touches
```
#### Record display screen:
```shell
scrcpy --record {{path/to/file.mp4}}
```
#### Set target directory for pushing files to device by drag and drop (non-APK):
```shell
scrcpy --push-target {{path/to/directory}}
```
{% endraw %}