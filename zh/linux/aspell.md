---
layout: default
title: "aspell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aspell">
  <a href="/zh/linux/aspell.html">aspell</a> <a href="#aspell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 交互式拼写检查工具.

#### 为一个文件做拼写检查:
```shell
aspell check {{文件路径}}
```
#### 列出来自标准输入的拼写错误单词:
```shell
cat {{文件}} | aspell list
```
#### 列出可用的字典语言:
```shell
aspell dicts
```
#### 指定不同的语言（取 ISO 639 语言代码的 2 个字母）来运行 aspell:
```shell
aspell --lang={{cs}}
```
#### 列出来自标准输入的拼写错误单词，并且忽略个人单词列表中的单词:
```shell
cat {{文件}} | aspell --personal={{个人单词列表.pws}} {{列表}}
```
{% endraw %}