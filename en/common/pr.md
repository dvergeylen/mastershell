---
layout: default
title: "pr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pr">
  <a href="/en/common/pr.html">pr</a> <a href="#pr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Paginate or columnate files for printing.
> More information: <https://www.gnu.org/software/coreutils/pr>.

#### Print multiple files with a default header and footer:
```shell
pr {{file1}} {{file2}} {{file3}}
```
#### Print with a custom centered header:
```shell
pr -h "{{header}}" {{file1}} {{file2}} {{file3}}
```
#### Print with numbered lines and a custom date format:
```shell
pr -n -D "{{format}}" {{file1}} {{file2}} {{file3}}
```
#### Print all files together, one in each column, without a header or footer:
```shell
pr -m -T {{file1}} {{file2}} {{file3}}
```
#### Print, beginning at page 2 up to page 5, with a given page length (including header and footer):
```shell
pr +{{2}}:{{5}} -l {{page_length}} {{file1}} {{file2}} {{file3}}
```
#### Print with an offset for each line and a truncating custom page width:
```shell
pr -o {{offset}} -W {{width}} {{file1}} {{file2}} {{file3}}
```
{% endraw %}