---
layout: default
title: "in2csv"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="in2csv">
  <a href="/en/common/in2csv.html">in2csv</a> <a href="#in2csv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converts various tabular data formats into CSV.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/in2csv.html>.

#### Convert an XLS file to CSV:
```shell
in2csv {{data.xls}}
```
#### Convert a DBF file to a CSV file:
```shell
in2csv {{data.dbf}} > {{data.csv}}
```
#### Convert a specific sheet from an XLSX file to CSV:
```shell
in2csv --sheet={{sheet_name}} {{data.xlsx}}
```
#### Pipe a JSON file to in2csv:
```shell
cat {{data.json}} | in2csv -f json > {{data.csv}}
```
{% endraw %}