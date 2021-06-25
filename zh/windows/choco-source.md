---
layout: default
title: "choco source"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-source">
  <a href="/zh/windows/choco-source.html">choco source</a> <a href="#choco-source"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 管理包的源.

#### 列出当前可用的源:
```shell
choco source list
```
#### 添加一个新的包源:
```shell
choco source add --name {{名称}} --source {{url}}
```
#### 添加包含凭据的新包源:
```shell
choco source add --name {{名称}} --source {{url}} --user {{用户名}} --password {{密码}}
```
#### 使用客户端证书添加新的包源:
```shell
choco source add --name {{名称}} --source {{url}} --cert {{证书的路径}}
```
#### 启用一个包源:
```shell
choco source enable --name {{名称}}
```
#### 禁用一个包源:
```shell
choco source disable --name {{名称}}
```
#### 移除一个包源:
```shell
choco source remove --name {{名称}}
```
{% endraw %}