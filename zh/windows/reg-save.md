---
layout: default
title: "reg save"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-save">
  <a href="/zh/windows/reg-save.html">reg save</a> <a href="#reg-save"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将注册表键、子键的所有值保存到一个文件中.

#### 将注册表键、子键的所有值保存到一个文件中:
```shell
reg save {{键名}} {{文件的路径}}
```
#### 在没有提示的情况下强制覆盖现有文件:
```shell
reg save {{键名}} {{文件的路径}} /y
```
{% endraw %}