---
layout: default
title: "asdf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asdf">
  <a href="/zh/common/asdf.html">asdf</a> <a href="#asdf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 可扩展的包版本管理器，支持Nodejs,Ruby,Elixir,Erlang等.
> 更多信息: <https://asdf-vm.com>.

#### 可用插件清单:
```shell
asdf plugin-list-all
```
#### 安装插件:
```shell
asdf plugin-add {{插件名}}
```
#### 软件包的可用版本清单:
```shell
asdf list-all {{软件包名}}
```
#### 安装指定版本的软件包:
```shell
asdf install {{软件包名}} {{版本}}
```
#### 设置软件包的全局安装版本:
```shell
asdf global {{软件包名}} {{版本}}
```
#### 设置软件包的本地版本:
```shell
asdf local {{软件包名}} {{版本}}
```
{% endraw %}