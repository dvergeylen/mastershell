---
layout: default
title: "z"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="z">
  <a href="/zh/common/z.html">z</a> <a href="#z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 记录被使用次数最多的目录并允许在它们之间以字符串或正则表达式来进行匹配和跳转.
> 更多信息：<https://github.com/rupa/z>.

#### 跳转到一个名字带有 "foo" 的文件夹:
```shell
z {{foo}}
```
#### 跳转到一个名字带有 "foo" 并且后面带有 "bar" 的文件夹（例：`fooesbar`):
```shell
z {{foo}} {{bar}}
```
#### 跳转到名字带有 "foo" 并且拥有最高访问次数的文件夹:
```shell
z -r {{foo}}
```
#### 跳转到最近使用的名字带有 "foo" 的文件夹:
```shell
z -t {{foo}}
```
#### 列出在 `z` 的数据库中名字带有 "foo" 的文件夹:
```shell
z -l {{foo}}
```
#### 将当前文件夹从 `z`的数据库中移除:
```shell
z -x .
```
{% endraw %}