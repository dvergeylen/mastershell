---
layout: default
title: "7zr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7zr">
  <a href="/zh/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个高压缩率的文件归档器.
> `7z`的独立版本，只支持 .7z 文件.

#### 归档一个文件或文件夹:
```shell
7zr a {{归档文件.7z}} {{文件路径}}
```
#### 提取一个已存在的 7z 文件，并保持原来的目录结构:
```shell
7zr x {{归档文件.7z}}
```
#### 列出一个归档文件的内容:
```shell
7zr l {{归档文件.7z}}
```
{% endraw %}