---
layout: default
title: "xmlto"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xmlto">
  <a href="/en/common/xmlto.html">xmlto</a> <a href="#xmlto"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apply an XSL stylesheet to an XML document.
> More information: <https://pagure.io/xmlto>.

#### Convert a DocBook XML document to PDF format:
```shell
xmlto {{pdf}} {{document.xml}}
```
#### Convert a DocBook XML document to HTML format and store the resulting files in a separate directory:
```shell
xmlto -o {{path/to/html_files}} {{html}} {{document.xml}}
```
#### Convert a DocBook XML document to a single HTML file:
```shell
xmlto {{html-nochunks}} {{document.xml}}
```
#### Specify a stylesheet to use while converting a DocBook XML document:
```shell
xmlto -x {{stylesheet.xsl}} {{output_format}} {{document.xml}}
```
{% endraw %}