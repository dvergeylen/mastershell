---
layout: default
title: "doskey"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="doskey">
  <a href="/zh/windows/doskey.html">doskey</a> <a href="#doskey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理宏，Windows 命令和命令行.

#### 列出可用的宏:
```shell
doskey /macros
```
#### 创建一个新的宏:
```shell
doskey {{宏的名称}} = "{{命令}}"
```
#### 为指定可执行文件创建新的宏:
```shell
doskey /exename={{可执行文件名}} {{宏的名称}} = "{{命令}}"
```
#### 删除一个宏:
```shell
doskey {{宏的名称}} =
```
#### 列出所有储存在内存中的命令:
```shell
doskey /history
```
#### 将宏保存到文件以便于移植:
```shell
doskey /macros > {{保存宏的文件名}}
```
#### 从文件中加载宏:
```shell
doskey /macrofile = {{保存宏的文件名}}
```
{% endraw %}