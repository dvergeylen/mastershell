---
layout: default
title: "chflags"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chflags">
  <a href="/zh/osx/chflags.html">chflags</a> <a href="#chflags"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 更改文件或文件夹的标志.

#### 给文件设置 hidden（隐藏） 标签:
```shell
chflags {{hidden}} {{文件路径}}
```
#### 取消文件的 hidden 标签:
```shell
chflags {{hidden}} {{文件路径}}
```
#### 递归地给文件夹中每个文件设置 uchg 标志:
```shell
chflags -R {{uchg}} {{文件夹路径}}
```
#### 递归地撤销文件夹中每个文件设置的 uchg 标志:
```shell
chflags -R {{nouchg}} {{文件夹路径}}
```
{% endraw %}