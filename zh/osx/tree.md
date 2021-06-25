---
layout: default
title: "tree"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tree">
  <a href="/zh/osx/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 以树的形式显示当前目录的内容.

#### 显示深度达到 “级数” 级的文件和目录（其中 1 表示当前目录）:
```shell
tree -L {{级数}}
```
#### 只显示目录:
```shell
tree -d
```
#### 同时显示隐藏文件:
```shell
tree -a
```
#### 打印没有缩进行的树，显示完整路径（使用`-N`不转义空格和特殊字符）:
```shell
tree -i -f
```
#### 以可读格式打印每个文件节点的大小，目录显示其累积大小（类似在`du`命令中所示）:
```shell
tree -s -h --du
```
#### 使用通配符（glob）模式在树层次结构中查找文件，并删除不包含匹配文件的目录:
```shell
tree -P '{{*.txt}}' --prune
```
#### 在树层次结构中查找目录，删除不属于所需目录的目录:
```shell
tree -P {{文件夹名}} --matchdirs --prune
```
{% endraw %}