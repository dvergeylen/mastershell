---
layout: default
title: "cppclean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cppclean">
  <a href="/en/common/cppclean.html">cppclean</a> <a href="#cppclean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find unused code in C++ projects.
> More information: <https://github.com/myint/cppclean>.

#### Run in a project's directory:
```shell
cppclean {{path/to/project}}
```
#### Run on a project where the headers are in the `inc1/` and `inc2/` directories:
```shell
cppclean {{path/to/project}} --include-path={{inc1}} --include-path={{inc2}}
```
#### Run on a specific file `main.cpp`:
```shell
cppclean {{main.cpp}}
```
#### Run on the current directory, excluding the "build" directory:
```shell
cppclean {{.}} --exclude={{build}}
```
{% endraw %}