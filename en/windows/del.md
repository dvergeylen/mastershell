---
layout: default
title: "del"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="del">
  <a href="/en/windows/del.html">del</a> <a href="#del"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete one or more files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/del>.

#### Delete one or more space-separated files or patterns:
```shell
del {{file_pattern}}
```
#### Prompt for confirmation before deleting each file:
```shell
del {{file_pattern}} /p
```
#### Force the deletion of read-only files:
```shell
del {{file_pattern}} /f
```
#### Recursively delete file(s) from all subdirectories:
```shell
del {{file_pattern}} /s
```
#### Do not prompt when deleting files based on a global wildcard:
```shell
del {{file_pattern}} /q
```
#### Display the help and list available attributes:
```shell
del /?
```
#### Delete files based on specified attributes:
```shell
del {{file_pattern}} /a {{attribute}}
```
{% endraw %}