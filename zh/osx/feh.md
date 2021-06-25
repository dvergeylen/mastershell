---
layout: default
title: "feh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="feh">
  <a href="/zh/osx/feh.html">feh</a> <a href="#feh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 轻量级图像查看工具.

#### 查看本地图像或使用 URL:
```shell
feh {{图片路径}}
```
#### 递归查看图像:
```shell
feh --recursive {{图片路径}}
```
#### 使用无边框窗口查看图像:
```shell
feh --borderless {{图片路径}}
```
#### 在浏览完最后一个图像之后退出:
```shell
feh --cycle-once {{图片路径}}
```
#### 设置幻灯片放映周期延迟时间（秒）:
```shell
feh --slideshow-delay {{秒}} {{图片路径}}
```
#### 设置墙纸（居中、填充、最大化、缩放或平铺）:
```shell
feh --bg-{{center|fill|max|scale|tile}} {{图片路径}}
```
{% endraw %}