---
layout: default
title: "flatpak"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="flatpak">
  <a href="/zh/linux/flatpak.html">flatpak</a> <a href="#flatpak"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 构建、安装和运行 Flatpak 应用和运行时。

#### 运行已安装应用：
```shell
flatpak run {{应用名}}
```
#### 从远程源安装应用：
```shell
flatpak install {{远程源名}} {{应用名}}
```
#### 列出所有应用和运行时：
```shell
flatpak list
```
#### 更新所有已安装的应用和运行时：
```shell
flatpak update
```
#### 添加远程源：
```shell
flatpak remote-add --if-not-exists {{远程源名}} {{远程源网址}}
```
#### 列出所有已配置的远程源：
```shell
flatpak remote-list
```
{% endraw %}