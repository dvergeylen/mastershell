---
layout: default
title: "hexdump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hexdump">
  <a href="/zh/osx/hexdump.html">hexdump</a> <a href="#hexdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个 ASCII、十进制、十六进制、八进制转换查看工具.

#### 打印文件的十六进制表示形式:
```shell
hexdump {{文件}}
```
#### 以十六进制显示输入偏移量，并在最后两列中显示其 ASCII 表示形式:
```shell
hexdump -C {{文件}}
```
#### 显示文件的十六进制表示，但只解释输入的 N 个字节:
```shell
hexdump -C -n{{字节数}} {{文件}}
```
{% endraw %}