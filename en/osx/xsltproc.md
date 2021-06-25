---
layout: default
title: "xsltproc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xsltproc">
  <a href="/en/osx/xsltproc.html">xsltproc</a> <a href="#xsltproc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transform XML with XSLT to produce output (usually HTML or XML).

#### Transform an XML file with a specific XSLT stylesheet:
```shell
xsltproc --output {{output.html}} {{stylesheet.xslt}} {{xmlfile.xml}}
```
#### Pass a value to a parameter in the stylesheet:
```shell
xsltproc --output {{output.html}} --stringparam {{name}} {{value}} {{stylesheet.xslt}} {{xmlfile.xml}}
```
{% endraw %}