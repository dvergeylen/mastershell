---
layout: default
title: "wsl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wsl">
  <a href="/zh/windows/wsl.html">wsl</a> <a href="#wsl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从命令行管理适用于 Linux 的 Windows 子系统.
> 更多信息: <https://docs.microsoft.com/windows/wsl/reference>.

#### 启动 Linux Shell（在默认发行版中）:
```shell
wsl {{shell_命令}}
```
#### 在不使用 Shell 的情况下运行 Linux 命令:
```shell
wsl --exec {{命令}} {{命令参数}}
```
#### 指定特定的发行版:
```shell
wsl --distribution {{发行版}} {{shell_命令}}
```
#### 列出所有可用发行版:
```shell
wsl --list
```
#### 将发行版导出到 .tar 文件:
```shell
wsl --export {{发行版}} {{路径/distro_fs.tar}}
```
#### 从 .tar 文件导入发行版:
```shell
wsl --import {{发行版}} {{路径/安装位置}} {{路径/distro_fs.tar}}
```
#### 更改指定发行版的版本:
```shell
wsl --set-version {{发行版}} {{版本}}
```
#### 关闭适用于 Linux 的 Windows 子系统:
```shell
wsl --shutdown
```
{% endraw %}