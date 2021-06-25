---
layout: default
title: "auracle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="auracle">
  <a href="/zh/linux/auracle.html">auracle</a> <a href="#auracle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用来和 Arch Linux 用户仓库交互的命令行工具，这个仓库通常被称作 AUR。
> 更多信息：<https://github.com/falconindy/auracle>.

#### 显示符合一个正则表达式的 AUR 包：
```shell
auracle search '{{regular_expression}}'
```
#### 显示 AUR 包列表的包信息，包名以一个单独的空格分隔：
```shell
auracle info {{package1}} {{package2}}
```
#### 显示 AUR 包列表的 `PKGBUILD` 文件（编译信息），包名以一个单独的空格分隔：
```shell
auracle show {{package1}} {{package2}}
```
#### 显示已安装 AUR 包的更新：
```shell
auracle outdated
```
{% endraw %}