---
layout: default
title: "aria2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aria2">
  <a href="/zh/common/aria2.html">aria2</a> <a href="#aria2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个轻量级多协议和多源命令行下载工具
> 支持 HTTP, HTTPS, FTP, SFTP, BitTorrent and Metalink.
> 主页：<https://aria2.github.io/>.

#### 下载一个网络资源:
```shell
aria2c {{http://example.org/myLinux.iso}}
```
#### 从多个源处下载一个资源:
```shell
aria2c {{http://mirror1.org/myLinux.iso}} {{http://mirror2.org/myLinux.iso}}
```
#### 使用两个连接下载资源:
```shell
aria2c -x{{2}} {{http://example.org/myLinux.iso}}
```
#### 从 Metalink URI 中下载资源:
```shell
aria2c {{http://example.org/myLinux.metalink}}
```
#### 从 BitTorrent URI 中下载资源:
```shell
aria2c {{http://example.org/myLinux.torrent}}
```
#### 从 BitTorrent Magnet URI 中下载资源:
```shell
aria2c {{'magnet:?xt=urn:btih:248D0A1CD08284299DE78D5C1ED359BB46717D8C'}}
```
#### 从一个文件中下载资源:
```shell
aria2c -i {{uris.txt}}
```
{% endraw %}