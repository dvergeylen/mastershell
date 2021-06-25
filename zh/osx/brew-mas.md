---
layout: default
title: "brew mas"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew-mas">
  <a href="/zh/osx/brew-mas.html">brew mas</a> <a href="#brew-mas"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mas 是一个简单的 Mac App Store 命令行界面.

#### 按应用名称搜索 Mac App Store 并返回匹配的标识符:
```shell
mas search {{应用名}}
```
#### 安装或更新以前购买的应用程序:
```shell
mas install {{应用名}} {{应用 ID}}
```
#### 显示所有已安装的应用程序及其应用 ID:
```shell
mas list
```
#### 列出等待更新的已安装应用:
```shell
mas outdated
```
#### 升级所有可升级的应用:
```shell
mas upgrade
```
#### 升级指定的应用:
```shell
mas upgrade {{应用 ID}}
```
{% endraw %}