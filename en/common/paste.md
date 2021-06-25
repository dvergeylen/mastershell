---
layout: default
title: "paste"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="paste">
  <a href="/en/common/paste.html">paste</a> <a href="#paste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Merge lines of files.
> More information: <https://www.gnu.org/software/coreutils/paste>.

#### Join all the lines into a single line, using TAB as delimiter:
```shell
paste -s {{file}}
```
#### Join all the lines into a single line, using the specified delimiter:
```shell
paste -s -d {{delimiter}} {{file}}
```
#### Merge two files side by side, each in its column, using TAB as delimiter:
```shell
paste {{file1}} {{file2}}
```
#### Merge two files side by side, each in its column, using the specified delimiter:
```shell
paste -d {{delimiter}} {{file1}} {{file2}}
```
#### Merge two files, with lines added alternatively:
```shell
paste -d '\n' {{file1}} {{file2}}
```
{% endraw %}