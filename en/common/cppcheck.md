---
layout: default
title: "cppcheck"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cppcheck">
  <a href="/en/common/cppcheck.html">cppcheck</a> <a href="#cppcheck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A static analysis tool for C/C++ code.
> Instead of syntax errors, it focuses on the types of bugs that compilers normally do not detect.
> More information: <http://cppcheck.sourceforge.net>.

#### Recursively check the current directory, showing progress on the screen and logging error messages to a file:
```shell
cppcheck . 2> cppcheck.log
```
#### Recursively check a given directory, and don't print progress messages:
```shell
cppcheck --quiet {{path/to/directory}}
```
#### Check a given file, specifying which tests to perform (by default only errors are shown):
```shell
cppcheck --enable={{error|warning|style|performance|portability|information|all}} {{path/to/file.cpp}}
```
#### List available tests:
```shell
cppcheck --errorlist
```
#### Check a given file, ignoring specific tests:
```shell
cppcheck --suppress={{test_id1}} --suppress={{test_id2}} {{path/to/file.cpp}}
```
#### Check the current directory, providing paths for include files located outside it (e.g. external libraries):
```shell
cppcheck -I {{include/directory_1}} -I {{include/directory_2}} .
```
#### Check a Microsoft Visual Studio project (`*.vcxproj`) or solution (`*.sln`):
```shell
cppcheck --project={{path/to/project.sln}}
```
{% endraw %}