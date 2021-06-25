---
layout: default
title: "cmd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmd">
  <a href="/zh/windows/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windows 命令解释器.

#### 开启一个新的命令行实例:
```shell
cmd
```
#### 运行指定的命令然后退出:
```shell
cmd /c "{{命令}}"
```
#### 执行一个指定的命令，之后进入一个交互式 shell:
```shell
cmd /k "{{命令}}"
```
#### 不显示命令的输出结果:
```shell
cmd /q
```
#### 启用或禁用命令扩展:
```shell
cmd /e:{{on|off}}
```
#### 启用或禁用文件和目录名的自动补全:
```shell
cmd /f:{{on|off}}
```
#### 启用或禁用环境变量扩展:
```shell
cmd /v:{{on|off}}
```
#### 强制输出内容使用 Unicode 编码:
```shell
cmd /u
```
{% endraw %}