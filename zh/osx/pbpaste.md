---
layout: default
title: "pbpaste"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pbpaste">
  <a href="/zh/osx/pbpaste.html">pbpaste</a> <a href="#pbpaste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将剪贴板的内容发送到标准输出（命令行）.

#### 将剪贴板的内容写入文件:
```shell
pbpaste > {{文件}}
```
#### 将剪贴板的内容用作命令的输入:
```shell
pbpaste | grep foo
```
{% endraw %}