---
layout: default
title: "indent"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="indent">
  <a href="/en/common/indent.html">indent</a> <a href="#indent"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change the appearance of a C/C++ program by inserting or deleting whitespace.
> More information: <https://www.gnu.org/software/indent/>.

#### Format C/C++ source according to the Linux style guide, automatically back up the original files, and replace with the indented versions:
```shell
indent --linux-style {{path/to/source.c}} {{path/to/another_source.c}}
```
#### Format C/C++ source according to the GNU style, saving the indented version to a different file:
```shell
indent --gnu-style {{path/to/source.c}} -o {{path/to/indented_source.c}}
```
#### Format C/C++ source according to the style of Kernighan & Ritchie (K&R), no tabs, 3 spaces per indent, and wrap lines at 120 characters:
```shell
indent --k-and-r-style --indent-level3 --no-tabs --line-length120 {{path/to/source.c}} -o {{path/to/indented_source.c}}
```
{% endraw %}