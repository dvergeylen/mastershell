---
layout: default
title: "pod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pod">
  <a href="/zh/osx/pod.html">pod</a> <a href="#pod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Swift 和 Objective-C Cocoa 项目的依赖关系管理.

#### 为当前项目初始化包含默认内容的 podfile:
```shell
pod init
```
#### 下载并安装 pod 文件中定义的所有 pod（以前未安装）:
```shell
pod install
```
#### 列出所有可用的 pod:
```shell
pod list
```
#### 显示过时的 pod（当前安装的 pod）:
```shell
pod outdated
```
#### 将当前安装的所有 pod 更新到其最新版本:
```shell
pod update
```
#### 将特定（以前安装的）pod 更新为其最新版本:
```shell
pod update {{pod_名}}
```
#### 从 Xcode 项目中删除 CocoaPods:
```shell
pod deintegrate {{xcode_项目}}
```
{% endraw %}