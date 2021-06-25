---
layout: default
title: "vlc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vlc">
  <a href="/zh/common/vlc.html">vlc</a> <a href="#vlc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 跨平台多媒体播放器.
> 更多信息: <https://www.videolan.org/vlc/>.

#### 播放一个文件:
```shell
vlc {{文件名}}
```
#### 全屏播放:
```shell
vlc --fullscreen {{文件名}}
```
#### 静音播放:
```shell
vlc --no-audio {{文件名}}
```
#### 循环播放:
```shell
vlc --loop {{文件名}}
```
#### 播放网络连接:
```shell
vlc {{连接}}
```
{% endraw %}