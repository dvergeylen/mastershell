---
layout: default
title: "pyflakes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pyflakes">
  <a href="/en/common/pyflakes.html">pyflakes</a> <a href="#pyflakes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Checks Python source code files for errors.
> More information: <https://pypi.org/project/pyflakes>.

#### Check a single Python file:
```shell
pyflakes check {{path/to/file}}.py
```
#### Check Python files in a specific directory:
```shell
pyflakes checkPath {{path/to/directory}}
```
#### Check Python files in a directory recursively:
```shell
pyflakes checkRecursive {{path/to/directory}}
```
#### Check all Python files found in multiple directories:
```shell
pyflakes iterSourceCode {{path/to/directory_1}} {{path/to/directory_2}}
```
{% endraw %}