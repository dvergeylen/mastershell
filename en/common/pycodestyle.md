---
layout: default
title: "pycodestyle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pycodestyle">
  <a href="/en/common/pycodestyle.html">pycodestyle</a> <a href="#pycodestyle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to check Python code against PEP 8 style conventions.
> More information: <https://pycodestyle.readthedocs.io>.

#### Check the style of a single file:
```shell
pycodestyle {{file.py}}
```
#### Check the style of multiple files:
```shell
pycodestyle {{file1.py}} {{file2.py}} {{file3.py}}
```
#### Show only the first occurrence of an error:
```shell
pycodestyle --first {{file.py}}
```
#### Show the source code for each error:
```shell
pycodestyle --show-source {{file.py}}
```
#### Show the specific PEP 8 text for each error:
```shell
pycodestyle --show-pep8 {{file.py}}
```
{% endraw %}