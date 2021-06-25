---
layout: default
title: "column"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="column">
  <a href="/en/common/column.html">column</a> <a href="#column"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Format standard input or a file into multiple columns.
> Columns are filled before rows; the default separator is a whitespace.
> More information: <https://manned.org/column>.

#### Format the output of a command for a 30 characters wide display:
```shell
printf "header1 header2\nbar foo\n" | column --output-width {{30}}
```
#### Split columns automatically and auto-align them in a tabular format:
```shell
printf "header1 header2\nbar foo\n" | column --table
```
#### Specify the column delimiter character for the `--table` option (e.g. "," for csv) (defaults to whitespace):
```shell
printf "header1,header2\nbar,foo\n" | column --table --separator {{,}}
```
#### Fill rows before filling columns:
```shell
printf "header1\nbar\nfoobar\n" | column --output-width {{30}} --fillrows
```
{% endraw %}