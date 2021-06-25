---
layout: default
title: "emulator"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="emulator">
  <a href="/en/common/emulator.html">emulator</a> <a href="#emulator"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manager Android emulators from the command-line.
> More information: <https://developer.android.com/studio/run/emulator-commandline>.

#### Display the help:
```shell
emulator -help
```
#### Start an Android emulator device:
```shell
emulator -avd {{name}}
```
#### Display the webcams on your development computer that are available for emulation:
```shell
emulator -avd {{name}} -webcam-list
```
#### Start an emulator overriding the facing back camera setting (use `-camera-front` for front camera):
```shell
emulator -avd {{name}} -camera-back {{none|emulated|webcamN}}
```
#### Start an emulator, with a maximum network speed:
```shell
emulator -avd {{name}} -netspeed {{gsm|hscsd|gprs|edge|hsdpa|lte|evdo|full}}
```
#### Start an emulator with network latency:
```shell
emulator -avd {{name}} -netdelay {{gsm|hscsd|gprs|edge|hsdpa|lte|evdo|none}}
```
#### Start an emulator, making all TCP connections through a specified HTTP/HTTPS proxy (port number is required):
```shell
emulator -avd {{name}} -http-proxy {{http://example.com:80}}
```
#### Start an emulator with a given SD card partition image file:
```shell
emulator -avd {{name}} -sdcard {{path/to/sdcard.img}}
```
{% endraw %}