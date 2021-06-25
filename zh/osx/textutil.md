---
layout: default
title: "textutil"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="textutil">
  <a href="/zh/osx/textutil.html">textutil</a> <a href="#textutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于操作各种格式的文本文件.

#### 显示有关 `foo.rtf` 的信息:
```shell
textutil -info {{foo.rtf}}
```
#### 将 `foo.rtf` 转换为 `foo.html`:
```shell
textutil -convert {{html}} {{foo.rtf}}
```
#### 将带格式的 rtf 文本转换为普通 txt 文本:
```shell
textutil {{foo.rtf}} -convert {{txt}}
```
#### 将 `foo.txt` 转换为 `foo.rtf`, 字体使用 Times 字号 10:
```shell
textutil -convert {{rtf}} -font {{Times}} -fontsize {{10}} {{foo.txt}}
```
#### 加载当前目录中的所有 RTF 文件，连接其内容，并将结果作为 `index.html` 写入，HTML 标题设置为"多个文件":
```shell
textutil -cat {{html}} -title "多个文件" -output {{index.html}} *.rtf
```
{% endraw %}