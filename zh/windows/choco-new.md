---
layout: default
title: "choco new"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-new">
  <a href="/zh/windows/choco-new.html">choco new</a> <a href="#choco-new"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 生成新的包规范文件.

#### 创建一个新的包框架:
```shell
choco new {{包名}}
```
#### 创建一个新的指定版本的包:
```shell
choco new {{包名}} --version {{版本号}}
```
#### 创建一个新的包并指定维护者的名字:
```shell
choco new {{包名}} --maintainer {{维护者名字}}
```
#### 在指定目录下创建新的包:
```shell
choco new {{包名}} --output-directory {{指定的目录路径}}
```
#### 创建一个新的包并指定其 32 位版和 64 位版的安装 URL:
```shell
choco new {{package_name}} url="{{url}}" url64="{{url}}"
```
{% endraw %}