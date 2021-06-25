---
layout: default
title: "aria2c"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aria2c">
  <a href="/zh/common/aria2c.html">aria2c</a> <a href="#aria2c"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 快速下载工具.
> 支持 HTTP(S), FTP, SFTP, BitTorrent, and Metalink.

#### 下载一个 URI 到文件:
```shell
aria2c {{url}}
```
#### 从多个源处下载一个资源:
```shell
aria2c {{url_1}} {{url_2}}
```
#### 通过保存在一个文件中的 URL 列表来下载资源:
```shell
aria2c -i {{文件名}}
```
#### 使用多个连接下载资源:
```shell
aria2c -s {{连接数量}} {{url}}
```
#### 通过带用户名密码验证的 FTP 协议下载资源:
```shell
aria2c --ftp-user={{用户名}} --ftp-passwd={{密码}} {{url}}
```
#### 限制下载速度 (bytes/s):
```shell
aria2c --max-download-limit={{速度}} {{url}}
```
{% endraw %}