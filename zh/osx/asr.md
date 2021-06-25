---
layout: default
title: "asr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asr">
  <a href="/zh/osx/asr.html">asr</a> <a href="#asr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将磁盘映像还原（复制）到卷上.
> 命令名称是 Apple Software Restore 的缩写.

#### 将磁盘映像复制到目标卷:
```shell
sudo asr restore --source {{映像名}}.dmg --target {{卷路径}}
```
#### 在复制之前擦除目标卷:
```shell
sudo asr restore --source {{映像名}}.dmg --target {{卷路径}} --erase
```
#### 恢复后跳过验证步骤:
```shell
sudo asr restore --source {{映像名}}.dmg --target {{卷路径}} --noverify
```
#### 不使用中间磁盘映像直接复制卷中的数据:
```shell
sudo asr restore --source {{卷路径}} --target {{复制卷路径}}
```
{% endraw %}