---
layout: default
title: "mpv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mpv">
  <a href="/zh/common/mpv.html">mpv</a> <a href="#mpv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个基于 MPlayer 的音频/视频播放器.
> 更多信息: <https://mpv.io>.

#### 播放一个音频或视频文件:
```shell
mpv {{文件名}}
```
#### 往后/往前 跳跃5秒:
```shell
LEFT <or> RIGHT
```
#### 往后/往前 跳跃一分钟:
```shell
DOWN <or> UP
```
#### 减少/增加 10% 播放速度:
```shell
[ <or> ]
```
#### 以指定速度播放文件 (0.01 到 100, 默认是 1):
```shell
mpv --speed {{速度}} {{文件名}}
```
#### 用 `mpv.conf` 中指定的一个用户配制播放文件:
```shell
mpv --profile {{配制名称}} {{文件名}}
```
#### 播放摄像头或其他设备的输出:
```shell
mpv /dev/{{video0}}
```
{% endraw %}