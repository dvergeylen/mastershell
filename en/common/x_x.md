---
layout: default
title: "x_x"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="x_x">
  <a href="/en/common/x_x.html">x_x</a> <a href="#x_x"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View Excel and CSV files from the command-line.
> More information: <https://github.com/kristianperkins/x_x>.

#### View an XLSX or CSV file:
```shell
x_x {{file.xlsx|file.csv}}
```
#### View an XLSX or CSV file, using the first row as table headers:
```shell
x_x -h {{0}} {{file.xlsx|file.csv}}
```
#### View a CSV file with unconventional delimiters:
```shell
x_x --delimiter={{';'}} --quotechar={{'|'}} {{file.csv}}
```
{% endraw %}