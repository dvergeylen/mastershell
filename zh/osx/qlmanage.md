---
layout: default
title: "qlmanage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qlmanage">
  <a href="/zh/osx/qlmanage.html">qlmanage</a> <a href="#qlmanage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> QuickLook 服务器工具.

#### 快速显示一个或多个文件:
```shell
qlmanage -p {{文件名}} {{文件名 2}}
```
#### 计算生成当前目录中所有 jpeg 文件的缩略图，300px 宽 png 格式，并将它们放在一个指定目录中:
```shell
qlmanage {{*.jpg}} -t -s {{300}} {{指定目录}}
```
#### 重置快速查看:
```shell
qlmanage -r
```
{% endraw %}