---
layout: default
title: "ftp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ftp">
  <a href="/zh/windows/ftp.html">ftp</a> <a href="#ftp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在本地和远程 FTP 服务器之间交互式传输文件.

#### 交互式连接一个远程的 FTP 服务:
```shell
ftp {{主机名}}
```
#### 匿名登录:
```shell
ftp -A {{主机名}}
```
#### 初始连接时禁用自动登录:
```shell
ftp -n {{主机名}}
```
#### 运行包含 FTP 命令列表的文件:
```shell
ftp -s:{{文件的路径}} {{主机名}}
```
#### 下载多个文件 （通配符表达式）:
```shell
mget {{*.png}}
```
#### 上传多个文件 （通配符表达式）:
```shell
mput {{*.zip}}
```
#### 在远程服务器上删除多个文件:
```shell
mdelete {{*.txt}}
```
#### 显示详细的帮助:
```shell
ftp --help
```
{% endraw %}