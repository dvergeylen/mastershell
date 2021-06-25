---
layout: default
title: "as"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="as">
  <a href="/zh/linux/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个可移植的 GUN 汇编器.
> 主要用于汇编`gcc`的输出，以供链接器`ld`使用.

#### 汇编一个文件，输出为 a.out:
```shell
as {{文件.s}}
```
#### 汇编文件，并指定输出文件:
```shell
as {{文件.s}} -o {{输出.o}}
```
#### 通过跳过空格和注释的预处理过程来更快的产生输出文件（只应该用于可信任的编译器的输出）:
```shell
as -f {{文件.s}}
```
#### 将给定路径添加到目录列表，来搜索.include 指令指定的文件:
```shell
as -I {{目录路径}} {{文件.s}}
```
{% endraw %}