---
layout: default
title: "port"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="port">
  <a href="/zh/osx/port.html">port</a> <a href="#port"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> macOS 包管理器软件（类似 brew).

#### 搜索包:
```shell
port search {{搜索的包名}}
```
#### 安装软件包:
```shell
sudo port install {{报名}}
```
#### 列出已安装的软件包:
```shell
port installed
```
#### 更新 port 自身，并获取可用包的最新列表:
```shell
sudo port selfupdate
```
#### 升级过时的软件包:
```shell
sudo port upgrade outdated
```
#### 删除已安装的软件包的旧版本:
```shell
sudo port uninstall inactive
```
{% endraw %}