---
layout: default
title: "xmllint"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xmllint">
  <a href="/en/common/xmllint.html">xmllint</a> <a href="#xmllint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> XML parser and linter that supports XPath, a syntax for navigating XML trees.

#### Return all nodes (tags) named "foo":
```shell
xmllint --xpath "//{{foo}}" {{source_file.xml}}
```
#### Return the contents of the first node named "foo" as a string:
```shell
xmllint --xpath "string(//{{foo}})" {{source_file.xml}}
```
#### Return the href attribute of the second anchor element in an html file:
```shell
xmllint --html --xpath "string(//a[2]/@href)" webpage.xhtml
```
#### Return human-readable (indented) XML from file:
```shell
xmllint --format {{source_file.xml}}
```
#### Check that a XML file meets the requirements of its DOCTYPE declaration:
```shell
xmllint --valid {{source_file.xml}}
```
#### Validate XML against DTD schema hosted online:
```shell
xmllint --dtdvalid {{URL}} {{source_file.xml}}
```
{% endraw %}