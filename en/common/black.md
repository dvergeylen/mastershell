---
layout: default
title: "black"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="black">
  <a href="/en/common/black.html">black</a> <a href="#black"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A Python auto code formatter.
> More information: <https://github.com/psf/black>.

#### Auto-format a file or entire directory:
```shell
black {{path/to/file_or_directory}}
```
#### Format the code passed in as a string:
```shell
black -c {{path/to/file_or_directory}}
```
#### Output a diff for each file on stdout:
```shell
black --diff {{path/to/file_or_directory}}
```
#### Return the status without writing the files back:
```shell
black --check {{path/to/file_or_directory}}
```
#### Auto-format a file or directory emitting exclusively error messages to stderr:
```shell
black --quiet {{path/to/file_or_directory}}
```
{% endraw %}