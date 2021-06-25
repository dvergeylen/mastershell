---
layout: default
title: "reg restore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-restore">
  <a href="/zh/windows/reg-restore.html">reg restore</a> <a href="#reg-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从备份文件中恢复键和值.
> 参见 `reg-save` 来获取更多的信息.

#### 使用备份文件中的数据覆盖指定的键:
```shell
reg restore {{键名}} {{文件路径}}
```
{% endraw %}