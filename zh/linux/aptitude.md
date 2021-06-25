---
layout: default
title: "aptitude"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aptitude">
  <a href="/zh/linux/aptitude.html">aptitude</a> <a href="#aptitude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian 和 Ubuntu 上的软件包管理工具.
> 更多信息： <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

#### 同步可用软件包及其版本列表，在运行后续 aptitude 命令前，应该首先运行该命令:
```shell
aptitude update
```
#### 安装一个新的软件包及其依赖项:
```shell
aptitude install {{软件包}}
```
#### 查找软件包:
```shell
aptitude search {{软件包}}
```
#### 移除一个软件包并移除所有依赖它的软件包:
```shell
aptitude remove {{软件包}}
```
#### 更新已安装软件包到最新版本:
```shell
aptitude upgrade
```
#### 更新已安装的软件包（类似于`aptitude upgrade`命令）， 移除过时的软件包并安装额外的软件包以满足新的软件包依赖项:
```shell
aptitude full-upgrade
```
{% endraw %}