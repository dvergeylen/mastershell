---
layout: default
title: "gcov"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gcov">
  <a href="/en/linux/gcov.html">gcov</a> <a href="#gcov"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Code coverage analysis and profiling tool that discovers untested parts of a program.
> Also displays a copy of source code annotated with execution frequencies of code segments.
> More information: <https://gcc.gnu.org/onlinedocs/gcc/Invoking-Gcov.html>.

#### Generate a coverage report named `file.cpp.gcov`:
```shell
gcov {{path/to/file.cpp}}
```
#### Write individual execution counts for every basic block:
```shell
gcov --all-blocks {{path/to/file.cpp}}
```
#### Write branch frequencies to the output file and print summary information to stdout as a percentage:
```shell
gcov --branch-probabilities {{path/to/file.cpp}}
```
#### Write branch frequencies as the number of branches taken, rather than the percentage:
```shell
gcov --branch-counts {{path/to/file.cpp}}
```
#### Do not create a `gcov` output file:
```shell
gcov --no-output {{path/to/file.cpp}}
```
#### Write file level as well as function level summaries:
```shell
gcov --function-summaries {{path/to/file.cpp}}
```
{% endraw %}