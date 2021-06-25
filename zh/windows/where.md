---
layout: default
title: "where"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="where">
  <a href="/zh/windows/where.html">where</a> <a href="#where"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示与搜索模式匹配的文件的位置.
> 在默认情况下，搜索是在当前目录和 PATH 环境变量指定的路径中执行的.

#### 显示匹配的文件的位置:
```shell
where {{文件模式}}
```
#### 显示匹配的文件的位置、大小和日期:
```shell
where /T {{文件模式}}
```
#### 在指定的路径下递归搜索要匹配的文件:
```shell
where /R {{目录的路径}} {{文件模式}}
```
#### 只返回退出代码，不显示匹配文件列表:
```shell
where /Q {{文件模式}}
```
{% endraw %}