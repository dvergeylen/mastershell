---
layout: default
title: "compgen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="compgen">
  <a href="/zh/osx/compgen.html">compgen</a> <a href="#compgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于在 bash 中自动完成的内置命令，按两次 tab 键即可调用该命令.

#### 显示所有可以执行的命令:
```shell
compgen -c
```
#### 列出所有别名:
```shell
compgen -a
```
#### 列出所有可以运行的函数:
```shell
compgen -A function
```
#### 列出所有 shell 的保留关键字:
```shell
compgen -k
```
#### 查看以 'ls' 开头的所有可用命令和别名:
```shell
compgen -ac {{ls}}
```
{% endraw %}