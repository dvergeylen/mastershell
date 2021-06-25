---
layout: default
title: "uname"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="uname">
  <a href="/zh/osx/uname.html">uname</a> <a href="#uname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打印当前计算机及其上运行的操作系统的详细信息.
> 注意：有关操作系统的其他信息，请尝试使用 `sw-vers` 命令.

#### 打印硬件相关：架构信息和处理器:
```shell
uname -mp
```
#### 打印软件相关信息：操作系统、版本号和版本:
```shell
uname -srv
```
#### 打印系统的节点名称（主机名）:
```shell
uname -n
```
#### 打印所有可用的系统信息（硬件、软件、节点名）:
```shell
uname -a
```
{% endraw %}