---
layout: default
title: "rmdir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rmdir">
  <a href="/zh/windows/rmdir.html">rmdir</a> <a href="#rmdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 删除一个目录和其中的内容.

#### 删除一个空目录:
```shell
rmdir {{目录的路径}}
```
#### 递归删除一个目录及其中的内容:
```shell
rmdir {{目录的路径}} /s
```
#### 在没有提示的情况下递归删除目录及其内容:
```shell
rmdir {{path/to/directory}} /s /q
```
{% endraw %}