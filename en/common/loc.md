---
layout: default
title: "loc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="loc">
  <a href="/en/common/loc.html">loc</a> <a href="#loc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool written in Rust that counts lines of code.
> More information: <https://github.com/cgag/loc>.

#### Print lines of code in the current directory:
```shell
loc
```
#### Print lines of code in the target directory:
```shell
loc {{path/to/directory}}
```
#### Print lines of code with stats for individual files:
```shell
loc --files
```
#### Print lines of code without .gitignore (etc.) files (e.g. two -u flags will additionally count hidden files and dirs):
```shell
loc -u
```
{% endraw %}