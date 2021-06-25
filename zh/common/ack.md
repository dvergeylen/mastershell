---
layout: default
title: "ack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ack">
  <a href="/zh/common/ack.html">ack</a> <a href="#ack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个类似 grep 的搜索工具，为程序员优化.

#### 寻找包含"小明"的文件:
```shell
ack {{小明}}
```
#### 在给定文件类型中寻找包含"小明"的文件:
```shell
ack --ruby {{小明}}
```
#### 计算匹配到"小明"的总次数:
```shell
ack -ch {{小明}}
```
#### 列出内容包含"小明"的文件的文件名，并显示在每个文件中匹配的次数:
```shell
ack -cl {{小明}}
```
{% endraw %}