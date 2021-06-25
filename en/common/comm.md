---
layout: default
title: "comm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="comm">
  <a href="/en/common/comm.html">comm</a> <a href="#comm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Select or reject lines common to two files. Both files must be sorted.
> More information: <https://www.gnu.org/software/coreutils/comm>.

#### Produce three tab-separated columns: lines only in first file, lines only in second file and common lines:
```shell
comm {{file1}} {{file2}}
```
#### Print only lines common to both files:
```shell
comm -12 {{file1}} {{file2}}
```
#### Print only lines common to both files, reading one file from stdin:
```shell
cat {{file1}} | comm -12 - {{file2}}
```
#### Get lines only found in first file, saving the result to a third file:
```shell
comm -23 {{file1}} {{file2}} > {{file1_only}}
```
#### Print lines only found in second file, when the files aren't sorted:
```shell
comm -13 <(sort {{file1}}) <(sort {{file2}})
```
{% endraw %}