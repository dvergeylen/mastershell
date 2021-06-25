---
layout: default
title: "reg add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-add">
  <a href="/zh/windows/reg-add.html">reg add</a> <a href="#reg-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将新的键值添加到注册表中.

#### 添加一个新的注册表键:
```shell
reg add {{键名}}
```
#### 在指定的键下添加新值:
```shell
reg add {{键名}} /v {{值}}
```
#### Add a new value with specific data:
```shell
reg add {{键名}} /d {{数据}}
```
#### 向具有特定数据类型的键添加新值:
```shell
reg add {{键名}} /t {{类型}}
```
#### 在没有提示的情况下强制覆盖现有的注册表值:
```shell
reg add {{键名}} /f
```
{% endraw %}