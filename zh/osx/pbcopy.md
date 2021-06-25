---
layout: default
title: "pbcopy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pbcopy">
  <a href="/zh/osx/pbcopy.html">pbcopy</a> <a href="#pbcopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将标准输出放入剪贴板（命令行里的 cmd + C).

#### 将文件的内容放入剪贴板:
```shell
pbcopy < {{文件}}
```
#### 将命令的执行结果放入剪贴板:
```shell
find . -type t -name "*.png" | pbcopy
```
{% endraw %}