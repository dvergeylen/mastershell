---
layout: default
title: "defaults"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="defaults">
  <a href="/zh/osx/defaults.html">defaults</a> <a href="#defaults"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 读取和写入 macOS 应用程序的用户配置.

#### 读取应用程序选项的系统默认值:
```shell
defaults read {{应用名}} {{选项}}
```
#### 读取应用程序选项的默认值:
```shell
defaults read -app {{应用名}} {{选项}}
```
#### 写入应用程序选项的默认值:
```shell
defaults write {{应用名}} {{选项}} {{- 类型}} {{值}}
```
#### 加速任务控制界面弹出动画 （时间设置为 0.1):
```shell
defaults write com.apple.Dock expose-animation-duration -float 0.1
```
#### 删除应用程序的所有默认值:
```shell
defaults delete {{应用名}}
```
{% endraw %}