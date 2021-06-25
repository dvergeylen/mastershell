---
layout: default
title: "xsv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xsv">
  <a href="/en/common/xsv.html">xsv</a> <a href="#xsv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CSV command-line toolkit written in Rust.
> More information: <https://github.com/BurntSushi/xsv>.

#### Inspect the headers of a file:
```shell
xsv headers {{path/to/file.csv}}
```
#### Count the number of entries:
```shell
xsv count {{path/to/file.csv}}
```
#### Get an overview of the shape of entries:
```shell
xsv stats {{path/to/file.csv}} | xsv table
```
#### Select a few columns:
```shell
xsv select {{column_a,column_b}} {{path/to/file.csv}}
```
#### Show 10 random entries:
```shell
xsv sample {{10}} {{path/to/file.csv}}
```
#### Join a column from one file to another:
```shell
xsv join --no-case {{column_a}} {{path/to/file/a.csv}} {{column_b}} {{path/to/file/b.csv}} | xsv table
```
{% endraw %}