---
layout: default
title: "7za"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="7za">
  <a href="/zh/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个高压缩率的文件归档器.
> `7z`的独立版本，支持的文档类型较少.

#### 归档一个文件或文件夹:
```shell
7za a {{归档文件.7z}} {{文件路径}}
```
#### 提取一个已存在的 7z 文件，并保持原来的目录结构:
```shell
7za x {{归档文件文件}}
```
#### 使用指定的类型来归档文件:
```shell
7za a -t{{zip|gzip|bzip2|tar|...}} {{归档文件}} {{文件路径}}
```
#### 列出可用的归档文件类型:
```shell
7za i
```
#### 列出一个归档文件的内容:
```shell
7za l {{归档文件}}
```
{% endraw %}