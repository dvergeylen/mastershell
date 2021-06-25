---
layout: default
title: "look"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="look">
  <a href="/zh/osx/look.html">look</a> <a href="#look"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 查找已排序的文件行（注意，必须是已排序的文件）.

#### 它开始寻找一个给定的前缀:
```shell
look {{前缀}} {{文件}}
```
#### 查找行，忽略大小写:
```shell
look -f {{前缀}} {{文件}}
```
{% endraw %}