---
layout: default
title: "cut"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cut">
  <a href="/en/common/cut.html">cut</a> <a href="#cut"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cut out fields from stdin or files.
> More information: <https://www.gnu.org/software/coreutils/cut>.

#### Cut out the first sixteen characters of each line of stdin:
```shell
cut -c {{1-16}}
```
#### Cut out the first sixteen characters of each line of the given files:
```shell
cut -c {{1-16}} {{file}}
```
#### Cut out everything from the 3rd character to the end of each line:
```shell
cut -c {{3-}}
```
#### Cut out the fifth field of each line, using a colon as a field delimiter (default delimiter is tab):
```shell
cut -d'{{:}}' -f{{5}}
```
#### Cut out the 2nd and 10th fields of each line, using a semicolon as a delimiter:
```shell
cut -d'{{;}}' -f{{2,10}}
```
#### Cut out the fields 3 through to the end of each line, using a space as a delimiter:
```shell
cut -d'{{ }}' -f{{3-}}
```
{% endraw %}