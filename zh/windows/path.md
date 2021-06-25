---
layout: default
title: "path"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="path">
  <a href="/zh/windows/path.html">path</a> <a href="#path"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或设置可执行文件的搜索路径.

#### 显示当前的路径:
```shell
path
```
#### 将路径设置为一个或多个以分号分隔的目录:
```shell
path {{目录的路径 1[; 目录的路径 2]}}
```
#### 将新的目录添加到源路径后:
```shell
path {{目录的路径}};%path%
```
#### 将命令提示符设置为仅搜索当前目录中的可执行文件:
```shell
path ;
```
{% endraw %}