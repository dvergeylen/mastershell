---
layout: default
title: "xcodebuild"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xcodebuild">
  <a href="/zh/osx/xcodebuild.html">xcodebuild</a> <a href="#xcodebuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 构建 Xcode 项目.

#### 构建工作区:
```shell
xcodebuild -workspace {{工作区名.工作区}} -scheme {{主题名}} -configuration {{配置名}} clean build SYMROOT={{SYMROOT_路径}}
```
#### 构建项目:
```shell
xcodebuild -target {{目标名}} -configuration {{配置名}} clean build SYMROOT={{SYMROOT_路径}}
```
#### 显示 SDK:
```shell
xcodebuild -showsdks
```
{% endraw %}