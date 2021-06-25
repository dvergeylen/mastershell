---
layout: default
title: "ar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ar">
  <a href="/zh/common/ar.html">ar</a> <a href="#ar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建，修改，提取库文件 (`.a`, `.so`, `.o`).
> 更多信息： <https://manned.org/ar>.

#### 从库文件中提取全部成员:
```shell
ar -x {{a 文件}}
```
#### 列出库文件中的成员:
```shell
ar -t {{a 文件}}
```
#### 替换或添加文件到库文件:
```shell
ar -r {{要被添加内容的 a 文件}} {{o 文件 1}} {{o 文件 2}} {{o 文件 3}}
```
#### 插入对象文件索引（相当于使用`ranlib`):
```shell
ar -s {{a 文件}}
```
#### 使用文件和附带的目标文件索引创建存档:
```shell
ar -rs {{a 文件}} {{o 文件 1}} {{o 文件 2}} {{o 文件 3}}
```
{% endraw %}