---
layout: default
title: "archey"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="archey">
  <a href="/zh/osx/archey.html">archey</a> <a href="#archey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 漂亮地显示简单系统信息工具.

#### 显示系统信息（彩色的）:
```shell
archey
```
#### 显示系统信息（单色的）:
```shell
archey --nocolor
```
#### 显示系统信息，使用 MacPorts（命令行软件安装管理工具 port) 来替代 Homebrew（另一种更常用的 mac 命令行软件安装管理工具）:
```shell
archey --macports
```
#### 显示系统信息，但不进行 IP 地址获取和验证:
```shell
archey --offline
```
{% endraw %}