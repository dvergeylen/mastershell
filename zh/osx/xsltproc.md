---
layout: default
title: "xsltproc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xsltproc">
  <a href="/zh/osx/xsltproc.html">xsltproc</a> <a href="#xsltproc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用 XSLT 转换 XML 以生成输出（通常是 HTML 或 XML ）.

#### 使用特定的 XSLT 样式表转换 XML 文件:
```shell
xsltproc --output {{输出.html}} {{样式表.xslt}} {{xml 文件.xml}}
```
#### 将值传递给样式表中的参数:
```shell
xsltproc --output {{输出.html}} --stringparam {{键名}} {{值}} {{样式表.xslt}} {{xml 文件.xml}}
```
{% endraw %}