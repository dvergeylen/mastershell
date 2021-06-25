---
layout: default
title: "zypper"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zypper">
  <a href="/zh/linux/zypper.html">zypper</a> <a href="#zypper"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SUSE & openSUSE 的软件包管理工具。

#### 同步可用的软件包和版本列表：
```shell
zypper refresh
```
#### 安装一个新的软件包：
```shell
zypper install {{软件包}}
```
#### 移除一个软件包：
```shell
zypper remove {{软件包}}
```
#### 将已安装的软件包升级到最新的可用版本：
```shell
zypper update
```
#### 通过关键字搜索软件包：
```shell
zypper search {{关键字}}
```
{% endraw %}