---
layout: default
title: "join"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="join">
  <a href="/en/common/join.html">join</a> <a href="#join"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Join lines of two sorted files on a common field.
> More information: <https://www.gnu.org/software/coreutils/join>.

#### Join two files on the first (default) field:
```shell
join {{file1}} {{file2}}
```
#### Join two files using a comma (instead of a space) as the field separator:
```shell
join -t {{','}} {{file1}} {{file2}}
```
#### Join field3 of file1 with field1 of file2:
```shell
join -1 {{3}} -2 {{1}} {{file1}} {{file2}}
```
#### Produce a line for each unpairable line for file1:
```shell
join -a {{1}} {{file1}} {{file2}}
```
{% endraw %}