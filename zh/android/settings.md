---
layout: default
title: "settings"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
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
{% endraw %}