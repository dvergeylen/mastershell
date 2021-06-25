---
layout: default
title: "brew cask"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="brew-cask">
  <a href="/zh/osx/brew-cask.html">brew cask</a> <a href="#brew-cask"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> macOS 上的应用程序包管理工具.

#### 模糊搜索可用命令行工具和软件包:
```shell
brew search {{软件名}}
```
#### 安装一个软件:
```shell
brew cask install {{软件名}}
```
#### 列出全部已安装软件:
```shell
brew cask list
```
#### 列出全部已安装的软件中，可以升级的:
```shell
brew cask outdated
```
#### 将一个已安装的软件升级到最新的版本:
```shell
brew cask upgrade {{软件名}}
```
#### 删除一个软件（仅通过 brew cask install 方式安装的）:
```shell
brew cask uninstall {{软件名}}
```
#### 卸载一个软件并删除相关的设置和文件:
```shell
brew cask zap {{软件名}}
```
#### 显示指定软件的相关信息:
```shell
brew cask info {{软件名}}
```
{% endraw %}