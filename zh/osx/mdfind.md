---
layout: default
title: "mdfind"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mdfind">
  <a href="/zh/osx/mdfind.html">mdfind</a> <a href="#mdfind"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 列出与给定查询匹配的文件.

#### 按文件名查找文件:
```shell
mdfind -name {{文件}}
```
#### 按内容查找文件:
```shell
mdfind {{查找的字符串}}
```
#### 在给定目录中查找包含字符串的文件:
```shell
mdfind -onlyin {{目录}} {{字符串}}
```
{% endraw %}