---
layout: default
title: "reg export"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-export">
  <a href="/zh/windows/reg-export.html">reg export</a> <a href="#reg-export"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将指定的子键和值导出到文件中.

#### 导出指定键下所有的子键和值:
```shell
reg export {{键名}} {{导出文件的路径.reg}}
```
#### 在没有提示的情况下强制覆盖现有文件:
```shell
reg export {{键名}} {{导出文件的路径.reg}} /y
```
{% endraw %}