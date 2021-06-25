---
layout: default
title: "ctags"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ctags">
  <a href="/en/common/ctags.html">ctags</a> <a href="#ctags"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generates an index (or tag) file of language objects found in source files for many popular programming languages.
> More information: <https://ctags.io/>.

#### Generate tags for a single file, and output them to a file named "tags" in the current directory, overwriting the file if it exists:
```shell
ctags {{path/to/file}}
```
#### Generate tags for all files in the current directory, and output them to a specific file, overwriting the file if it exists:
```shell
ctags -f {{filename}} *
```
#### Generate tags for all files in the current directory and all subdirectories:
```shell
ctags --recurse
```
{% endraw %}