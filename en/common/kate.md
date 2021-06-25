---
layout: default
title: "kate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kate">
  <a href="/en/common/kate.html">kate</a> <a href="#kate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> KDE Text Editor.
> More information: <https://kate-editor.org/>.

#### Launch Kate and open specific files:
```shell
kate {{path/to/file1}} {{path/to/file2}}
```
#### Open a remote document in Kate:
```shell
kate {{https://example.com/path/to/file}}
```
#### Launch Kate, creating a new instance even if one is already open:
```shell
kate --new
```
#### Open a file in Kate with the cursor at the specific line:
```shell
kate --line {{line_number}} {{path/to/file}}
```
#### Open a file in Kate with the cursor at the specific line and column:
```shell
kate --line {{line_number}} --column {{column_number}} {{path/to/file}}
```
#### Launch Kate, creating a new temporary file with contents read from stdin:
```shell
cat {{path/to/file}} | kate --stdin
```
#### Display help:
```shell
kate --help
```
{% endraw %}