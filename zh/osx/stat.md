---
layout: default
title: "stat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stat">
  <a href="/zh/osx/stat.html">stat</a> <a href="#stat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示文件状态.

#### 显示文件属性，如大小、权限、创建和访问日期等:
```shell
stat {{文件}}
```
#### 与上面相同，但更详细（更类似于 Linux 的 `stat`）:
```shell
stat -x {{文件}}
```
#### 只显示文件权限:
```shell
stat -f %Mp%Lp {{文件}}
```
#### 显示文件的所有者和所属组:
```shell
stat -f "%Su %Sg" {{文件}}
```
#### 以字节为单位显示文件的大小:
```shell
stat -f "%z %N" {{文件}}
```
{% endraw %}