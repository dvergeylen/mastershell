---
layout: default
title: "ag"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ag">
  <a href="/zh/common/ag.html">ag</a> <a href="#ag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Silver Searcher. 类似 ack, 但是更快.
> 更多信息: <https://github.com/ggreer/the_silver_searcher>.

#### 寻找内容包含"小明"的文件，并列出所在的行数:
```shell
ag {{小明}}
```
#### 在指定目录中寻找内容包含"foo"的文件:
```shell
ag {{小明}} {{指定的目录}}
```
#### 寻找内容包含"foo"的文件，但只列出文件名:
```shell
ag -l {{小明}}
```
#### 忽略大小写，寻找内容包含"ABC"的文件，并只输出匹配的内容，而非整行:
```shell
ag -i -o {{ABC}}
```
#### 在文件名包含"小红"的文件中寻找"小明":
```shell
ag {{小明}} -G {{小红}}
```
#### 使用正则表达式来匹配文件内容:
```shell
ag '{{^ba(r|z)$}}'
```
#### 输出文件名包含"小明"的文件名:
```shell
ag -g {{小明}}
```
{% endraw %}