---
layout: default
title: "assoc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="assoc">
  <a href="/zh/windows/assoc.html">assoc</a> <a href="#assoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或修改文件扩展名关联.

#### 显示所有当前文件扩展名关联的列表:
```shell
assoc
```
#### 显示指定扩展名的关联文件类型:
```shell
assoc {{.txt}}
```
#### 将文件扩展名与特定的文件类型关联:
```shell
assoc {{.txt}}={{txtfile}}
```
{% endraw %}