---
layout: default
title: "addr2line"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="addr2line">
  <a href="/zh/linux/addr2line.html">addr2line</a> <a href="#addr2line"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将二进制文件地址转换成文件名和行数。

#### 显示可执行文件的指令地址对应源代码的文件名和行数：
```shell
addr2line --exe={{可执行文件路径}} {{地址}}
```
#### 显示函数名、文件名和行数：
```shell
addr2line --exe={{可执行文件路径}} --functions {{地址}}
```
#### 将 c++ 代码函数名符号重组：
```shell
addr2line --exe={{可执行文件地址}} --functions --demangle {{地址}}
```
{% endraw %}