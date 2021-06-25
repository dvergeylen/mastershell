---
layout: default
title: "apt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt">
  <a href="/zh/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 基于 Debian 的发行版上的软件包管理工具.
> 更多信息： <https://manpages.debian.org/latest/apt/apt.8.html>.

#### 更新可用软件包及其版本列表（推荐在运行其他 apt 命令前首先运行该命令）:
```shell
sudo apt update
```
#### 查找指定软件包:
```shell
apt search {{软件包}}
```
#### 显示关于指定软件包的信息:
```shell
apt show {{软件包}}
```
#### 安装指定软件包或将指定软件包更新到最新版本:
```shell
sudo apt install {{软件包}}
```
#### 移除指定软件包（使用`purge`可以同时移除其配置文件）:
```shell
sudo apt remove {{软件包}}
```
#### 将所有已安装软件包更新到最新可用版本:
```shell
sudo apt upgrade
```
{% endraw %}