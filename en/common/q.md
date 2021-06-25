---
layout: default
title: "q"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="q">
  <a href="/en/common/q.html">q</a> <a href="#q"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute SQL-like queries on .csv and .tsv files.
> More information: <https://harelba.github.io/q>.

#### Query `.csv` file by specifying the delimiter as ',':
```shell
q -d',' "SELECT * from {{path/to/file}}"
```
#### Query `.tsv` file:
```shell
q -t "SELECT * from {{path/to/file}}"
```
#### Query file with header row:
```shell
q -d{{delimiter}} -H "SELECT * from {{path/to/file}}"
```
#### Read data from stdin; '-' in the query represents the data from stdin:
```shell
{{output}} | q "select * from -"
```
#### Join two files (aliased as `f1` and `f2` in the example) on column `c1`, a common column:
```shell
q "SELECT * FROM {{path/to/file}} f1 JOIN {{path/to/other_file}} f2 ON (f1.c1 = f2.c1)"
```
#### Format output using an output delimiter with an output header line (note: command will output column names based on the input file header or the column aliases overridden in the query):
```shell
q -D{{delimiter}} -O "SELECT {{column}} as {{alias}} from {{path/to/file}}"
```
{% endraw %}