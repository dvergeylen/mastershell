---
layout: default
title: "clip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clip">
  <a href="/zh/windows/clip.html">clip</a> <a href="#clip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将输入的内容复制到 Windows 的剪贴板.

#### 用管道将命令的输出内容复制到 Windows 剪贴板:
```shell
{{dir}} | clip
```
#### 将一个文件中的内容复制到 Windows 剪贴板:
```shell
clip < {{文件的路径}}
```
{% endraw %}