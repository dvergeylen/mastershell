---
layout: default
title: "fastboot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fastboot">
  <a href="/en/common/fastboot.html">fastboot</a> <a href="#fastboot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Communicate with connected Android devices when in bootloader mode (the one place `adb` doesn't work).
> More information: <https://android.googlesource.com/platform/system/core/+/master/fastboot/#fastboot>.

#### Unlock the bootloader:
```shell
fastboot oem unlock
```
#### Relock the bootloader:
```shell
fastboot oem lock
```
#### Reboot the device from fastboot mode into fastboot mode again:
```shell
fastboot reboot bootloader
```
#### Flash a given image:
```shell
fastboot flash {{file.zip}}
```
#### Flash a custom recovery image:
```shell
fastboot flash recovery {{file.img}}
```
#### Display connected devices:
```shell
fastboot devices
```
#### Display all information of a device:
```shell
fastboot getvar all
```
{% endraw %}