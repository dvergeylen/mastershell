---
layout: default
title: "ftype"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ftype">
  <a href="/zh/windows/ftype.html">ftype</a> <a href="#ftype"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或修改用于文件扩展名关联的文件类型.

#### 显示所有文件类型的列表:
```shell
ftype
```
#### 显示特定文件类型的关联程序:
```shell
ftype {{文件类型}}
```
#### 设置特定文件类型的关联程序:
```shell
ftype {{文件类型}}="{{可执行命令的路径}}"
```
{% endraw %}