---
layout: default
title: "wacaw"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wacaw">
  <a href="/zh/osx/wacaw.html">wacaw</a> <a href="#wacaw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个用于 macOS 的小命令行工具，允许您从连接的摄像头捕获静止图片和视频

#### 从网络摄像机拍照:
```shell
wacaw {{文件名}}
```
#### 录制视频:
```shell
wacaw --video {{文件名}} -D {{录制多少秒}}
```
#### 用自定义分辨率拍照:
```shell
wacaw -x {{宽}} -y {{高}} {{文件名}}
```
#### 将刚拍摄的图像复制到剪贴板:
```shell
wacaw --to-clipboard
```
#### 可用设备列表:
```shell
wacaw -L
```
{% endraw %}