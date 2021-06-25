---
layout: default
title: "sdiff"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sdiff">
  <a href="/en/common/sdiff.html">sdiff</a> <a href="#sdiff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare the differences between and optionally merge 2 files.

#### Compare 2 files:
```shell
sdiff {{path/to/file1}} {{path/to/file2}}
```
#### Compare 2 files, ignoring all tabs and whitespace:
```shell
sdiff -W {{path/to/file1}} {{path/to/file2}}
```
#### Compare 2 files, ignoring whitespace at the end of lines:
```shell
sdiff -Z {{path/to/file1}} {{path/to/file2}}
```
#### Compare 2 files in a case-insensitive manner:
```shell
sdiff -i {{path/to/file1}} {{path/to/file2}}
```
#### Compare and then merge, writing the output to a new file:
```shell
sdiff -o {{path/to/merged_file}} {{path/to/file1}} {{path/to/file2}}
```
{% endraw %}