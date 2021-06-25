---
layout: default
title: "comp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="comp">
  <a href="/zh/windows/comp.html">comp</a> <a href="#comp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 比较两个文件或文件集的内容.
> 使用通配符 (*) 来比较文件集.

#### 交互式比较文件:
```shell
comp
```
#### 比较两个指定的文件:
```shell
comp {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 比较两个文件集:
```shell
comp {{目录 1/*}} {{目录 2/*}}
```
#### 以十进制格式显示差异:
```shell
comp /d {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 以 ASCII 字符显示差异:
```shell
comp /a {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 显示不同的行数:
```shell
comp /l {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 比较文件时不区分大小写:
```shell
comp /c {{文件 1 的路径}} {{文件 2 的路径}}
```
#### 只比较每个文件前 5 行的内容:
```shell
comp /n={{5}} {{文件 1 的路径}} {{文件 2 的路径}}
```
{% endraw %}