---
layout: default
title: "duti"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="duti">
  <a href="/zh/osx/duti.html">duti</a> <a href="#duti"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 macOS 上为文档类型和网页设置默认打开的应用程序.

#### 将 Safari 设置为 HTML 文档的默认打开程序:
```shell
duti -s {{com.apple.Safari}} {{public.html}} all
```
#### 将 vlc 设置为扩展名为.m4v 的文件的默认查看器:
```shell
duti -s {{org.videolan.vlc}} {{m4v}} viewer
```
#### 将 Finder 设置为 ftp:// URL 访问的应用:
```shell
duti -s {{com.apple.Finder}} {{ftp}}
```
#### 显示有关给定扩展名的默认应用程序的信息:
```shell
duti -x {{ext}}
```
#### 显示给定的 UTI 对应默认的处理程序:
```shell
duti -d {{uti}}
```
#### 显示给定 UTI 对应所有的处理程序:
```shell
duti -l {{uti}}
```
{% endraw %}