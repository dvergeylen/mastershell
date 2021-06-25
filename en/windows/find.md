---
layout: default
title: "find"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="find">
  <a href="/en/windows/find.html">find</a> <a href="#find"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find a specified string in one or more files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/find>.

#### Find lines that contain a specified string:
```shell
find {{string}} {{path/to/file_or_directory}}
```
#### Display lines that do not contain the specified string:
```shell
find {{string}} {{path/to/file_or_directory}} /v
```
#### Display the count of lines that contain the specified string:
```shell
find {{string}} {{path/to/file_or_directory}} /c
```
#### Display line numbers with the list of lines:
```shell
find {{string}} {{path/to/file_or_directory}} /n
```
{% endraw %}