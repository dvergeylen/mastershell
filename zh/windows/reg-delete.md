---
layout: default
title: "reg delete"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-delete">
  <a href="/zh/windows/reg-delete.html">reg delete</a> <a href="#reg-delete"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从注册表中删除键和值.

#### 删除一个指定的键:
```shell
reg delete {{键名}}
```
#### 删除键中指定的值:
```shell
reg delete {{键名}} /v {{值}}
```
#### 递归删除指定键下所有的值:
```shell
reg delete {{键名}} /va
```
#### 在没有提示的情况下递归删除键中所有的值:
```shell
reg delete {{键名}} /f /va
```
{% endraw %}