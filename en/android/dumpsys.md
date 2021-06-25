---
layout: default
title: "dumpsys"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dumpsys">
  <a href="/en/android/dumpsys.html">dumpsys</a> <a href="#dumpsys"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Provide information about Android system services.
> This command can only be used through `adb shell`.
> More information: <https://developer.android.com/studio/command-line/dumpsys>.

#### Get diagnostic output for all system services:
```shell
dumpsys
```
#### Get diagnostic output for a specific system service:
```shell
dumpsys {{service}}
```
#### List all services `dumpsys` can give information about:
```shell
dumpsys -l
```
#### List service-specific arguments for a service:
```shell
dumpsys {{service}} -h
```
#### Exclude a specific service from the diagnostic output:
```shell
dumpsys --skip {{service}}
```
#### Specify a timeout period in seconds (defaults to 10s):
```shell
dumpsys -t {{seconds}}
```
{% endraw %}