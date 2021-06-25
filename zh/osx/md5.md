---
layout: default
title: "md5"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="md5">
  <a href="/zh/osx/md5.html">md5</a> <a href="#md5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 计算 MD5 加密和校验.

#### 计算一个文件的 MD5 校验值:
```shell
md5 {{文件名}}
```
#### 计算多个文件的 MD5 校验值:
```shell
md5 {{文件名 1}} {{文件名 2}}
```
#### 仅输出 MD5 校验值（无文件名）:
```shell
md5 -q {{文件名}}
```
#### 打印给定字符串的 MD5 校验值:
```shell
md5 -s {{字符串}}
```
{% endraw %}