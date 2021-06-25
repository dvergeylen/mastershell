---
layout: default
title: "softwareupdate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="softwareupdate">
  <a href="/zh/osx/softwareupdate.html">softwareupdate</a> <a href="#softwareupdate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 通过命令行更新 macOS 应用商店中应用程序的工具.

#### 列出所有可用的更新:
```shell
softwareupdate -l
```
#### 下载并安装所有更新:
```shell
softwareupdate -ia
```
#### 下载并安装所有推荐的更新:
```shell
softwareupdate -ir
```
#### 下载并安装特定的应用程序:
```shell
softwareupdate -i {{更新应用程序名}}
```
{% endraw %}