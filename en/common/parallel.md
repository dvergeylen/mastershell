---
layout: default
title: "parallel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="parallel">
  <a href="/en/common/parallel.html">parallel</a> <a href="#parallel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run commands on multiple CPU cores.
> More information: <https://www.gnu.org/software/parallel>.

#### Gzip several files at once, using all cores:
```shell
parallel gzip ::: {{file1}} {{file2}} {{file3}}
```
#### Read arguments from stdin, run 4 jobs at once:
```shell
ls *.txt | parallel -j4 gzip
```
#### Convert JPG images to PNG using replacement strings:
```shell
parallel convert {} {.}.png ::: *.jpg
```
#### Parallel xargs, cram as many args as possible onto one command:
```shell
{{args}} | parallel -X {{command}}
```
#### Break stdin into ~1M blocks, feed each block to stdin of new command:
```shell
cat {{big_file.txt}} | parallel --pipe --block 1M {{command}}
```
#### Run on multiple machines via SSH:
```shell
parallel -S {{machine1}},{{machine2}} {{command}} ::: {{arg1}} {{arg2}}
```
{% endraw %}