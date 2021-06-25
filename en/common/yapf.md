---
layout: default
title: "yapf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yapf">
  <a href="/en/common/yapf.html">yapf</a> <a href="#yapf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python style guide checker.
> More information: <https://github.com/google/yapf>.

#### Display a diff of the changes that would be made, without making them (dry-run):
```shell
yapf --diff {{path/to/file}}
```
#### Format the file in-place and display a diff of the changes:
```shell
yapf --diff --in-place {{path/to/file}}
```
#### Recursively format all Python files in a directory, concurrently:
```shell
yapf --recursive --in-place --style {{pep8}} --parallel {{path/to/directory}}
```
{% endraw %}