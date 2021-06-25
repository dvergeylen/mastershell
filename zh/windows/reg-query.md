---
layout: default
title: "reg query"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-query">
  <a href="/zh/windows/reg-query.html">reg query</a> <a href="#reg-query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示注册表中键和子键的值.

#### 显示一个键中的所有值:
```shell
reg query {{键名}}
```
#### 显示键中指定的值:
```shell
reg query {{键名}} /v {{值}}
```
#### 显示指定键和其子键中的所有的值:
```shell
reg query {{键名}} /s
```
#### 搜索与特定模式匹配的键和值:
```shell
reg query {{键名}} /f "{{查询语句}}"
```
#### 显示与指定数据类型匹配的键的值:
```shell
reg query {{键名}} /t {{类型}}
```
{% endraw %}