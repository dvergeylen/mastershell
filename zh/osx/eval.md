---
layout: default
title: "eval"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="eval">
  <a href="/zh/osx/eval.html">eval</a> <a href="#eval"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在当前 shell 中以单个命令的形式执行参数，并返回其结果.

#### 使用 'foo' 做为参数调用 `echo`:
```shell
eval "{{echo foo}}"
```
#### 在当前 shell 程序中设置变量:
```shell
eval "{{foo=bar}}"
```
{% endraw %}