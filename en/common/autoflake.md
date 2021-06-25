---
layout: default
title: "autoflake"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autoflake">
  <a href="/en/common/autoflake.html">autoflake</a> <a href="#autoflake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to remove unused imports and variables from Python code.
> More information: <https://github.com/myint/autoflake>.

#### Remove unused variables from a single file and display the diff:
```shell
autoflake --remove-unused-variables {{file.py}}
```
#### Remove unused imports from multiple files and display the diffs:
```shell
autoflake --remove-all-unused-imports {{file1.py}} {{file2.py}} {{file3.py}}
```
#### Remove unused variables from a file, overwriting the file:
```shell
autoflake --remove-unused-variables --in-place {{file.py}}
```
#### Remove unused variables recursively from all files in a directory, overwriting each file:
```shell
autoflake --remove-unused-variables --in-place --recursive {{path/to/directory}}
```
{% endraw %}