---
layout: default
title: "xed"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xed">
  <a href="/zh/osx/xed.html">xed</a> <a href="#xed"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用 Xcode 打开要编辑的文件.

#### 用 Xcode 打开文件 :
```shell
xed {{文件名}}
```
#### 在 Xcode 中打开文件，如果不存在则创建:
```shell
xed -c {{文件名}}
```
#### 在 Xcode 中打开一个文件并跳转到第 75 行:
```shell
xed -l 75 {{文件名}}
```
{% endraw %}