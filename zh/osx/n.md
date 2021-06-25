---
layout: default
title: "n"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="n">
  <a href="/zh/osx/n.html">n</a> <a href="#n"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于管理多个节点版本的工具.

#### 安装给定版本的节点。如果版本已经安装，它将被激活:
```shell
n {{版本}}
```
#### 显示已安装的版本并以交互方式激活其中一个版本:
```shell
n
```
#### 删除一个版本:
```shell
n rm {{版本}}
```
#### 使用给定版本执行文件:
```shell
n use {{版本}} {{文件.js}}
```
#### 输出指定版本的二进制:
```shell
n bin {{版本}}
```
{% endraw %}