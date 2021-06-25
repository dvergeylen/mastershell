---
layout: default
title: "axel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="axel">
  <a href="/zh/common/axel.html">axel</a> <a href="#axel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一款下载加速器.
> 支持HTTP, HTTPS, 和 FTP.
> 更多信息: <https://github.com/axel-download-accelerator/axel>.

#### 链接下载:
```shell
axel {{超链接}}
```
#### 链接下载，指定文件名:
```shell
axel {{超链接}} -o {{文件名称}}
```
#### 多连接数下载:
```shell
axel -n {{连接数量}} {{超链接}}
```
#### 查询镜像:
```shell
axel -S {{镜像数量}} {{超链接}}
```
#### 限制下载速度 (字节bite每秒):
```shell
axel -s {{字节数}} {{超链接}}
```
{% endraw %}