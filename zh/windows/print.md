---
layout: default
title: "print"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="print">
  <a href="/zh/windows/print.html">print</a> <a href="#print"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将文本文件打印到打印机.

#### 将文本文件打印到默认的打印机:
```shell
print {{文件的路径}}
```
#### 将文本文件打印到指定的打印机:
```shell
print /d:{{打印机}} {{文件的路径}}
```
{% endraw %}