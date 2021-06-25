---
layout: default
title: "as"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="as">
  <a href="/zh/osx/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 便携式 GNU 汇编程序.
> 主要用于汇编 `gcc` 的输出以供 `ld` 使用

#### 汇编文件，将输出写入 a.out:
```shell
as {{文件.s}}
```
#### 将输出汇编到给定文件:
```shell
as {{文件.s}} -o {{输出.o}}
```
#### 通过跳过空白和注释预处理来更快地生成输出.（应该只用于受信任的编译器）:
```shell
as -f {{文件.s}}
```
#### 在目录列表中包含一个给定路径，以搜索 .include 指令中指定的文件:
```shell
as -I {{目标文件夹}} {{文件.s}}
```
{% endraw %}