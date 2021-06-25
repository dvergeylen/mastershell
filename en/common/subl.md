---
layout: default
title: "subl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="subl">
  <a href="/en/common/subl.html">subl</a> <a href="#subl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sublime Text editor.
> More information: <https://www.sublimetext.com>.

#### Open the current directory in Sublime Text:
```shell
subl {{.}}
```
#### Open a file or directory in Sublime Text:
```shell
subl {{path/to/file_or_directory}}
```
#### Open a file and jump to a specific line number:
```shell
subl {{path/to/file}}:{{line_number}}
```
#### Open a file or directory in the currently open window:
```shell
subl -a {{path/to/file}}
```
#### Open a file or directory in a new window:
```shell
subl -n {{path/to/file}}
```
{% endraw %}