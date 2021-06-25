---
layout: default
title: "scc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scc">
  <a href="/en/common/scc.html">scc</a> <a href="#scc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool written in Go that counts lines of code.
> More information: <https://github.com/boyter/scc>.

#### Print lines of code in the current directory:
```shell
scc
```
#### Print lines of code in the target directory:
```shell
scc {{path/to/directory}}
```
#### Display output for every file:
```shell
scc --by-file
```
#### Display output using a specific output format (defaults to `tabular`):
```shell
scc --format {{tabular|wide|json|csv|cloc-yaml|html|html-table}}
```
#### Only count files with specific file extensions:
```shell
scc --include-ext {{go, java, js}}
```
#### Exclude directories from being counted:
```shell
scc --exclude-dir {{.git,.hg}}
```
#### Display output and sort by column (defaults to by files):
```shell
scc --sort {{files|name|lines|blanks|code|comments|complexity}}
```
#### Print help for scc:
```shell
scc -h
```
{% endraw %}