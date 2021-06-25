---
layout: default
title: "subst"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="subst">
  <a href="/zh/windows/subst.html">subst</a> <a href="#subst"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将路径与虚拟驱动器号关联.

#### 列出已激活的关联:
```shell
subst
```
#### 添加一个关联:
```shell
subst {{Z:}} {{C:\Python2.7}}
```
#### 删除一个关联:
```shell
subst {{Z:}} /d
```
{% endraw %}