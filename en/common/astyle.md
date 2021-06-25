---
layout: default
title: "astyle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="astyle">
  <a href="/en/common/astyle.html">astyle</a> <a href="#astyle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Source code indenter, formatter, and beautifier for the C, C++, C# and Java programming languages.
> Upon running, a copy of the original file is created with an ".orig" appended to the original file name.
> More information: <http://astyle.sourceforge.net/>.

#### Apply the default style of 4 spaces per indent and no formatting changes:
```shell
astyle {{source_file}}
```
#### Apply the java style with attached braces:
```shell
astyle --style=java {{path/to/file}}
```
#### Apply the allman style with broken braces:
```shell
astyle --style=allman {{path/to/file}}
```
#### Apply a custom indent using spaces. Choose between 2 and 20 spaces:
```shell
astyle --indent=spaces={{number_of_spaces}} {{path/to/file}}
```
#### Apply a custom indent using tabs. Choose between 2 and 20 tabs:
```shell
astyle --indent=tab={{number_of_tabs}} {{path/to/file}}
```
{% endraw %}