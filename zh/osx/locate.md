---
layout: default
title: "locate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="locate">
  <a href="/zh/osx/locate.html">locate</a> <a href="#locate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 快速查找文件名.

#### 在数据库中查找关键字。注意：数据库定期重新更新（通常每周或每天）:
```shell
locate {{关键字}}
```
#### 按文件名查找文件（不包含填充字符的模式被解释为 `*关键字*`）:
```shell
locate */{{文件名}}
```
#### 重新建立文件数据索引数据库。如果要查找最近添加的文件，则需要执行此操作:
```shell
sudo /usr/libexec/locate.updatedb
```
{% endraw %}