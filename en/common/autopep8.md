---
layout: default
title: "autopep8"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autopep8">
  <a href="/en/common/autopep8.html">autopep8</a> <a href="#autopep8"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Format Python code according to the PEP 8 style guide.
> More information: <https://github.com/hhatto/autopep8>.

#### Format a file to stdout, with a custom maximum line length:
```shell
autopep8 {{path/to/file.py}} --max-line-length {{length}}
```
#### Format a file, displaying a diff of the changes:
```shell
autopep8 --diff {{path/to/file}}
```
#### Format a file in-pace and save the changes:
```shell
autopep8 --in-place {{path/to/file.py}}
```
#### Recursively format all files in a directory in-place and save changes:
```shell
autopep8 --in-place --recursive {{path/to/directory}}
```
{% endraw %}