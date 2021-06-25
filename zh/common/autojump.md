---
layout: default
title: "autojump"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autojump">
  <a href="/zh/common/autojump.html">autojump</a> <a href="#autojump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 快速跳转，访问次数最多的文件夹优先.
> 使用j、jc、jo作为别名.
> 更多信息: <https://github.com/wting/autojump>.

#### 跳转到包含指定通配符的目录:
```shell
j {{通配符表达式}}
```
#### 跳转到包含指定通配符的目录的下一级:
```shell
jc {{通配符表达式}}
```
#### 使用系统文件管理器，打开指定的目录:
```shell
jo {{通配符表达式}}
```
#### 从autojump数据库中删除不存在的目录:
```shell
j --purge
```
#### 展示autojump数据库数据:
```shell
j -s
```
{% endraw %}