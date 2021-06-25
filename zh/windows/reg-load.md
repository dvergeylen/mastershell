---
layout: default
title: "reg load"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-load">
  <a href="/zh/windows/reg-load.html">reg load</a> <a href="#reg-load"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将保存的子键加载到不同的子键中.
> This is intended for troubleshooting and temporary keys.

#### 将备份文件加载到指定的键中:
```shell
reg load {{键名}} {{文件的路径}}
```
{% endraw %}