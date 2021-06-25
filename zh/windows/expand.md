---
layout: default
title: "expand"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="expand">
  <a href="/zh/windows/expand.html">expand</a> <a href="#expand"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 解压一个或多个 cab 文件.

#### 将单文件 cab 文件解压到指定目录:
```shell
expand {{cab 文件路径}} {{指定的目录}}
```
#### 列出 cab 文件中的所有文件:
```shell
expand {{cab 文件路径}} {{指定的目录}} -d
```
#### 从 cab 文件中解压所有的文件:
```shell
expand {{cab 文件路径}} {{指定的目录}} -f:*
```
#### 从 cab 文件中解压一个特定的文件:
```shell
expand {{cab 文件路径}} {{指定的目录}} -f:{{文件名}}
```
#### 解压缩时忽略目录结构，并将它们添加到单个目录中:
```shell
expand {{cab 文件路径}} {{指定的目录}} -i
```
{% endraw %}