---
layout: default
title: "brew"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew">
  <a href="/zh/osx/brew.html">brew</a> <a href="#brew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> macOS 上的软件包管理工具.

#### 搜索可用的命令行和软件安装包:
```shell
brew search {{软件名}}
```
#### 安装最新版本的命令行软件 （使用 `--devel` 可以指定安装更新的开发版）:
```shell
brew install {{软件名}}
```
#### 列出已（通过 brew) 安装的命令行工具:
```shell
brew list
```
#### 升级已安装的命令行软件（如果未给出命令行软件名称，则升级所有已安装的软件）:
```shell
brew upgrade {{软件名}}
```
#### 从 GitHub 上升级 brew 和软件库到最新:
```shell
brew update
```
#### 显示有关指定软件的信息（版本，安装路径，依赖关系等）:
```shell
brew info {{软件名}}
```
#### 检查本地 Homebrew 安装是否存在潜在问题，并给出一些解决建议:
```shell
brew doctor
```
#### 启动通过 brew 安装的服务，如 nginx,mysql 等。启动后还会自动随开机启动，直到你选择 stop 停止.（缺点是如果发生错误，它也会返回成功，而不是报错）:
```shell
brew services {{start|stop|restart}} {{软件名}}
```
{% endraw %}