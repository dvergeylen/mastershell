---
layout: default
title: "where"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="where">
  <a href="/en/windows/where.html">where</a> <a href="#where"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the location of files that match the search pattern.
> Defaults to current work directory and paths in the PATH environment variable.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/where>.

#### Display the location of file pattern:
```shell
where {{file_pattern}}
```
#### Display the location of file pattern including file size and date:
```shell
where /T {{file_pattern}}
```
#### Recursively search for file pattern at specified path:
```shell
where /R {{path/to/directory}} {{file_pattern}}
```
#### Display only the error code for the location of file pattern:
```shell
where /Q {{file_pattern}}
```
{% endraw %}