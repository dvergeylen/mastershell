---
layout: default
title: "yank"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yank">
  <a href="/zh/osx/yank.html">yank</a> <a href="#yank"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从 stdin 读取输入并显示一个选择界面，该界面允许选择一个字段并将其复制到剪贴板.

#### 使用默认分隔符 (\f, \n, \r, \s, \t):
```shell
{{sudo dmesg}} | yank
```
#### 输入单行:
```shell
{{sudo dmesg}} | yank -l
```
#### 使用特定分 `=` 隔符输入:
```shell
{{echo hello=world}} | yank -d {{=}}
```
#### 只有与特定正则表达式匹配的内容才输入:
```shell
{{ps ux}} | yank -g "{{[0-9]+}}"
```
{% endraw %}