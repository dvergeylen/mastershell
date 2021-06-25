---
layout: default
title: "pdfgrep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdfgrep">
  <a href="/zh/osx/pdfgrep.html">pdfgrep</a> <a href="#pdfgrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 PDF 文件中搜索文本.

#### 在 PDF 中查找与关键词匹配的行:
```shell
pdfgrep {{关键词}} {{文件.pdf}}
```
#### 包含每个匹配行的文件名和页码:
```shell
pdfgrep --with-filename --page-number {{关键词}} {{文件.pdf}}
```
#### 对以 "foo" 开头关键词搜索，返回前 3 个匹配项，不区分大小写:
```shell
pdfgrep --max-count {{3}} --ignore-case {{'^foo'}} {{文件.pdf}}
```
#### 在当前目录中扩展名为.pdf 的文件中递归查找关键词:
```shell
pdfgrep --recursive {{关键词}}
```
#### 在与当前目录中特定文件名 "*book.pdf" 匹配的文件上递归查找关键词:
```shell
pdfgrep --recursive --include {{'*book.pdf'}} {{关键词}}
```
{% endraw %}