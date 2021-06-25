---
layout: default
title: "carthage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="carthage">
  <a href="/zh/osx/carthage.html">carthage</a> <a href="#carthage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cocoa 应用程序的依赖性管理工具

#### 下载 Cartfile 中提到的所有依赖项的最新版本，并编译它们:
```shell
carthage update
```
#### 仅针对 IOS 平台，升级依赖文件 :
```shell
carthage update --platform ios
```
#### 仅更新依赖，但不编译它们 :
```shell
carthage update --no-build
```
#### 下载并重新生成依赖项的当前版本（不更新它们）:
```shell
carthage bootstrap
```
#### 重新编译特定依赖项 :
```shell
carthage build {{依赖包}}
```
{% endraw %}