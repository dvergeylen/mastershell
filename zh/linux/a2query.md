---
layout: default
title: "a2query"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="a2query">
  <a href="/zh/linux/a2query.html">a2query</a> <a href="#a2query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上查看 Apache 运行配置。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2query.1.html>.

#### 列出启用的 Apache 模块：
```shell
sudo a2query -m
```
#### 查看某个模块是否已安装：
```shell
sudo a2query -m {{模块名}}
```
#### 列出已启用的虚拟主机：
```shell
sudo a2query -s
```
#### 显示已启用的多进程模块：
```shell
sudo a2query -M
```
#### 显示 Apache 版本：
```shell
sudo a2query -v
```
{% endraw %}